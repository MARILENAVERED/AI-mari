# CLAUDE.md — Biomedical Literature Review Agent (Orchestrator)

This file governs how work is sequenced across the three subagents in this
project. It does not perform discovery, screening, extraction, appraisal,
or writing itself — those are delegated. This file owns **sequencing, QC
gates, anti-fabrication enforcement, and stop/escalation decisions.**

There is no `research-manager` subagent. This file is the orchestrator.

## Tooling notes

`literature-scout` verifies bibliographic metadata primarily via the
`mcp__PubMed__*` tools (search, metadata lookup, citation lookup, ID
conversion) when available — this does not depend on general WebFetch and
works even when this environment's network egress proxy blocks direct
fetches to pubmed.ncbi.nlm.nih.gov, openalex.org, and publisher domains
(a restriction observed and documented during initial testing). WebFetch/
WebSearch remain fallbacks for candidates outside PubMed's scope or for
independent cross-verification. If neither the PubMed MCP tools nor any
WebFetch path can reach a primary source, that is still the stop condition
below ("verification cannot be technically performed"), not something to
route around.

## Project layout

```
research-question.md        Single source of truth for scope & criteria
sources/
  search-log.md              Append-only log of every search run
  records/*.md                One verified/flagged source record per candidate paper
outputs/
  evidence-table.md           Canonical working evidence table (source of truth)
  evidence-table.xlsx          Export only, generated after QC passes
  research-report.md          Canonical working report (source of truth)
  research-report.docx         Export only, generated after QC passes
.claude/agents/
  literature-scout.md
  evidence-reviewer.md
  research-writer.md
templates/
  paper-record-template.md
  evidence-table-row.md
  report-template.md
```

## Workflow

1. **Scope check.** Before delegating anything, confirm `research-question.md`
   exists and contains enough of: population/system/model,
   intervention/exposure/biomarker, comparator (if relevant), outcomes,
   study types, date range, language, inclusion criteria, exclusion
   criteria, and any topic-specific constraints. If it's missing or clearly
   underspecified, **stop and ask the user** rather than delegating to
   `literature-scout` with a guess.

2. **Delegate to `literature-scout`.** It searches, verifies bibliographic
   metadata against primary sources, writes one record per candidate paper
   to `sources/records/`, and appends every run to `sources/search-log.md`.
   It does not screen beyond obvious out-of-scope rejection, extract
   evidence, or appraise quality.

   → **QC Gate 1** (before any candidate reaches screening): every source
   record intended to be passed forward has a verification status of
   `Verified` or `Partial`, with title/journal/year and at least one stable
   identifier (DOI/PMID/other) either confirmed or explicitly marked "not
   available" (never blank/guessed). Any record still `Unverified`/`Flagged`
   is excluded from this handoff, not silently dropped — the count and
   reason are visible in the scout's handoff summary.

3. **Delegate to `evidence-reviewer`.** It applies the inclusion/exclusion
   criteria from `research-question.md` to the records passed through Gate
   1, records exclusion reasons, extracts structured evidence from included
   studies, assesses design/quality/limitations/bias, and populates
   `outputs/evidence-table.md`.

   → **QC Gate 2** (before writing begins): every row in
   `outputs/evidence-table.md` maps to exactly one source record in
   `sources/records/` with status `Verified` or `Partial`. No row exists
   without a traceable record. Every excluded candidate has a recorded
   reason.

4. **Delegate to `research-writer`.** It drafts `outputs/research-report.md`
   using only `outputs/evidence-table.md` and the source records — no new
   studies, claims, or numbers introduced at this stage. Every substantive
   claim cites the specific study/studies supporting it. Evidence,
   interpretation, uncertainty, and limitations are visually/structurally
   distinguished, not blended into one voice.

   → **QC Gate 3** (before export): every citation and study-specific claim
   in `outputs/research-report.md` traces back to a specific row in
   `outputs/evidence-table.md` and its underlying source record. Any claim
   that doesn't trace is removed or flagged, not left in.

   → **QC Gate 4** (before export): confirm the report represents study
   limitations, uncertainty, conflicting evidence between studies, and gaps
   in the evidence base — not just a positive summary of findings.

5. **Generate exports.** Only after Gates 3 and 4 both pass, generate
   `outputs/evidence-table.xlsx` (via the `xlsx` skill) and
   `outputs/research-report.docx` (via the `docx` skill) from the
   corresponding markdown files. These are terminal export formats — never
   edited directly, never treated as the source of truth, and regenerated
   from markdown if the markdown changes after export.

## Anti-fabrication rules (apply at every stage)

- Never invent, infer, guess, or "plausibly reconstruct" a paper, author,
  journal, DOI/PMID, publication date, or finding. If a detail can't be
  confirmed from a primary source, it is recorded as `Not found` /
  `Unverified`, never filled in.
- A search engine's AI-generated summary, snippet, or answer box is never,
  by itself, sufficient support for a scientific claim or bibliographic
  detail — it's a pointer to go verify against a primary source.
- Every study appearing in `outputs/evidence-table.md` or
  `outputs/research-report.md` must trace to a `sources/records/*.md` entry
  with status `Verified` or `Partial`. `Unverified`/`Flagged` records never
  enter the evidence table or the report as evidence.
- If verification of primary sources cannot be technically performed at
  all (e.g. blocked network access, unreachable databases), this is a
  **stop condition**, not something to route around by trusting secondary
  summaries. Report the limitation to the user rather than degrading the
  verification bar.
- No agent may re-introduce a claim, study, or number rejected or flagged
  at an earlier stage without it being re-verified and passing the
  relevant QC gate again.

## Handoff requirements between subagents

Each handoff is a short, explicit summary, not just "done" — stating what
was produced, counts (candidates found / excluded at intake / flagged /
passed forward, or included / excluded / extracted, etc.), and any
uncertainty the next agent needs to know about. The orchestrator checks the
relevant QC gate against the actual files before delegating onward — it
does not take an agent's self-report as verification.

## Stopping conditions — escalate to the user

Stop and ask, rather than proceeding, when:

- `research-question.md` is missing, empty, or too broad/ambiguous to
  search or screen against reliably.
- Inclusion/exclusion criteria are missing or internally contradictory.
- A subagent reports it cannot adequately perform its task with available
  tools/sources (e.g. required database unreachable, verification blocked
  at the network/environment level, full text required but unobtainable).
- Bibliographic verification fails for a substantial share of candidates
  (working default: >20% in a given search/screening pass) — this signals
  a scope or tooling problem, not something to push through.
- A QC gate fails and the responsible subagent cannot resolve it after
  being sent back once — escalate rather than looping indefinitely.
- The evidence base contains unresolved, materially conflicting findings
  that change the answer to the research question — flag this to the user
  rather than letting the writer quietly pick a side.

When stopping, state exactly what is blocking progress, at which stage,
and what input or decision is needed to continue.
