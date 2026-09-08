# Search Log

Append-only log of every search run performed by `literature-scout`. Never edit or delete prior entries — append new ones below.

---

## Run 1 — 2026-09-08

- **Query:** `EGFR mutation subtype treatment response NSCLC tyrosine kinase inhibitor`
- **Tool/database:** PubMed (`mcp__PubMed__search_articles`)
- **Filters applied:** Publication date 2022/01/01–2026/12/31; no language/study-type filter applied at search stage (applied at intake screening instead)
- **Results returned:** 80 total hits; first 20 reviewed
- **Notes:** Broad arm-1 search covering EGFR subtype + treatment response generally. Reviewed top 20 PMIDs by relevance. Of these, verified/screened in detail: 42218657 (included), 42466433 (excluded — case report, other evidence exists), 42453333 (included — review of co-mutations and TKI response), 42361448 (excluded — pooled EGFR-mutant, no subtype breakdown; stratified by TP53 instead), 42628527 (excluded — preclinical only), 42492466 (excluded — subtype only as non-adjusted exploratory subgroup). Remaining PMIDs in the top-20 not pursued to metadata verification because a smaller, higher-relevance/higher-quality set had already accumulated (quality-over-quantity per instructions); can be revisited if evidence-reviewer identifies a gap.

## Run 2 — 2026-09-08

- **Query:** `EGFR exon 20 insertion NSCLC treatment outcomes`
- **Tool/database:** PubMed (`mcp__PubMed__search_articles`)
- **Filters applied:** Publication date 2022/01/01–2026/12/31
- **Results returned:** 137 total hits; first 20 reviewed
- **Notes:** Arm-2 search (exon 20 insertion specifically). Strong yield for this arm. Verified/screened: 42512396 (included — review), 42291370 (included — CNS/molecular landscape cohort), 42239888 (included — ctDNA resistance to mobocertinib), 42216441 (included — amivantamab ATLAS registry), 42212913 (included — NEJM sunvozertinib phase 3 RCT), 41971937 (excluded — n=6 case series, stronger evidence already captured), 41816478 (excluded — broad multi-gene perioperative review, scope mismatch), 41585239 (excluded — single-patient case report, other evidence exists), 41659272 (excluded — single-patient case report, other evidence exists on subtype), 41273219 (included — afatinib resistance mechanisms by subtype, EGFR/ERBB2).

## Run 3 — 2026-09-08

- **Query:** `EGFR uncommon mutation G719X L861Q S768I NSCLC osimertinib`
- **Tool/database:** PubMed (`mcp__PubMed__search_articles`)
- **Filters applied:** Publication date 2022/01/01–2026/12/31
- **Results returned:** 16 total hits (all returned)
- **Notes:** Arm-2/3 search targeting specific uncommon EGFR point-mutation subtypes. Verified/screened: 41967619 (included — comprehensive atypical-mutation review), 42320198 (included — de novo/acquired compound mutations, UCSD+GENIE), 41139406 (included — later-generation TKI outcomes in uncommon mutations, multicenter). Remaining older/lower-priority hits in this result set (2022-2024 dated) not pursued given sufficient high-relevance yield already achieved for the uncommon-subtype arm; available for follow-up if evidence-reviewer requests deeper coverage.

## Run 4 — 2026-09-08

- **Query:** `acquired resistance mechanism EGFR mutation subtype NSCLC osimertinib`
- **Tool/database:** PubMed (`mcp__PubMed__search_articles`)
- **Filters applied:** Publication date 2022/01/01–2026/12/31
- **Results returned:** 5 total hits (all returned)
- **Notes:** Arm-3 search (acquired resistance by subtype). Narrow, well-targeted query. Verified/screened all 5: 42466433 (excluded, dup with Run 1 — case report), 42170254 (excluded — pooled resistance-mechanism review, no subtype breakdown), 41675516 (excluded — off-scope triple-positive EGFR/ALK/PD-L1 case report), 38382773 (included — review tying resistance mechanisms to subtype heterogeneity), 34309914 (excluded — pre-dates 2022 date range and off-scope on leptomeningeal metastasis focus, no subtype breakdown).

## Run 5 — 2026-09-08

- **Query:** `EGFR compound mutation NSCLC clinical outcome TKI`
- **Tool/database:** PubMed (`mcp__PubMed__search_articles`)
- **Filters applied:** Publication date 2022/01/01–2026/12/31
- **Results returned:** 116 total hits; first 20 reviewed
- **Notes:** Arm-4 search (compound mutations). Top hit 42320198 (dup with Run 3, already included) confirmed as the strongest compound-mutation candidate. 42218657 also surfaced here (dup with Run 1, already included — has compound-mutation subgroup findings). Given the compound-mutation arm was already well covered by 42320198 and 41139406 from other runs, and that a 12-candidate, quality-focused set had been reached, the remaining 18 PMIDs in this batch were not individually pursued to full metadata verification. Available for a follow-up pass if evidence-reviewer or orchestrator determines additional compound-mutation-specific coverage is needed.

---

## Summary across all runs

- Unique PMIDs verified via `get_article_metadata` against PubMed's authoritative record: 24
- Passed forward to evidence-reviewer (Verified/Partial, on-scope): 12
- Excluded at intake (with reasons recorded in each record file): 12

## Post-hoc scope correction — 2026-09-08

`research-question.md` was updated to explicitly exclude narrative reviews
(non-systematic, no stated search methodology) as evidence, resolving an
ambiguity evidence-reviewer had flagged. Three previously-forwarded
records — PMID-38382773 (Ferro et al.), PMID-41967619 (Spitaleri et al.),
PMID-42512396 (Zullo & Remon) — are narrative reviews and are reclassified
from "Pass forward to evidence-reviewer" to "Excluded at intake" per this
updated criterion. Their underlying bibliographic verification is
unaffected (still Verified) — only their evidentiary disposition changes.

Records with disposition "Pass forward to evidence-reviewer" after this
correction: 9 (12 originally forwarded, minus the 3 reclassified reviews).
Of those 9, PMID-42453333 (Jing et al.) had already been excluded by
evidence-reviewer in its first screening pass (co-mutation-focused, not
EGFR-subtype-stratified) — its own source-record disposition line was
never updated at the time, which was corrected on 2026-09-08 for
bookkeeping accuracy. Net records actually eligible for evidence
extraction after both corrections: 8 — matching the 8 rows in
`outputs/evidence-table.md`.
