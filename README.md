# AI-mari

project-patho

A biomedical literature review agent for clinical and basic biomedical
research. It searches peer-reviewed literature, screens it against
explicit criteria, extracts structured evidence, critically appraises
study quality, and produces a referenced evidence synthesis — with
bibliographic verification as a hard requirement at every stage.

## How it works

Three subagents run in a fixed pipeline, coordinated by `CLAUDE.md` (the
orchestrator). There is no separate "manager" agent — `CLAUDE.md` owns
sequencing, QC gates, and escalation.

```
research-question.md  →  literature-scout  →  evidence-reviewer  →  research-writer
                              │                      │                     │
                        sources/records/*.md   outputs/evidence-table.md  outputs/research-report.md
                        sources/search-log.md
```

1. **`literature-scout`** ([.claude/agents/literature-scout.md](.claude/agents/literature-scout.md)) —
   discovers candidate papers relevant to `research-question.md`, verifies
   their bibliographic metadata against primary sources (PubMed, OpenAlex,
   publisher pages — never a search snippet or AI-generated summary alone),
   and writes one source record per candidate to `sources/records/`. Every
   search run is logged in `sources/search-log.md`.

2. **`evidence-reviewer`** ([.claude/agents/evidence-reviewer.md](.claude/agents/evidence-reviewer.md)) —
   applies the inclusion/exclusion criteria from `research-question.md`,
   records exclusion reasons, extracts structured evidence from included
   studies, appraises design/quality/bias, and populates
   `outputs/evidence-table.md`.

3. **`research-writer`** ([.claude/agents/research-writer.md](.claude/agents/research-writer.md)) —
   writes `outputs/research-report.md` using only the evidence table and
   verified source records. Every substantive claim is cited; evidence,
   interpretation, and uncertainty are kept visibly distinct; no new
   studies are introduced at this stage.

Between each handoff, `CLAUDE.md` enforces a QC gate (valid metadata →
traceable evidence-table rows → traceable citations → represented
limitations/uncertainty) before work moves forward, and defines when to
stop and ask the user instead of proceeding (ambiguous scope, contradictory
criteria, unreachable sources, high verification-failure rate, or evidence
that materially conflicts).

## Getting started

1. Fill in [`research-question.md`](research-question.md) — the single
   source of truth for scope, criteria, study types, date range, and any
   topic-specific constraints. It uses a flexible framework (PICO is
   supported but not required).
2. Run the pipeline via `CLAUDE.md`, which delegates to the three
   subagents in order.
3. Review the canonical markdown outputs —
   [`outputs/evidence-table.md`](outputs/evidence-table.md) and
   [`outputs/research-report.md`](outputs/research-report.md) — these are
   the source of truth throughout the process.
4. Once all QC gates pass, `outputs/evidence-table.xlsx` and
   `outputs/research-report.docx` are generated as final export formats
   (never edited directly, always regenerated from the markdown).

## Anti-fabrication guarantee

No paper, author, journal, identifier, or finding is ever invented or
inferred. If bibliographic details can't be verified against a primary
source, the paper is flagged or excluded — never guessed. See `CLAUDE.md`
for the full set of anti-fabrication rules enforced across all three
subagents.

## Known limitation

Bibliographic verification requires outbound access to sources like
PubMed, OpenAlex, and publisher sites. In network-restricted environments
(e.g. sandboxed sessions with a locked-down egress proxy), `literature-scout`
will correctly refuse to mark candidates `Verified` rather than trust
unverifiable search summaries — this shows up as papers stuck at
`Unverified (verification blocked)` in `sources/records/`. Run in an
environment with the necessary outbound access for real evidence synthesis
work.
