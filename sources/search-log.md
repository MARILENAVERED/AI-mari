# Search Log

Reproducible record of every search run performed by `literature-scout`.

---

## Run 1 (superseded — see Runs 3-6)

- **Date:** 2026-09-08
- **Query:** `EGFR mutation subtype treatment response acquired resistance NSCLC 2023 2024 PubMed`
- **Tool/database:** Hosted web search (general)
- **Filters:** None
- **Results returned:** 8 links surfaced
- **Notes:** Verification via WebFetch to pubmed.ncbi.nlm.nih.gov, eutils.ncbi.nlm.nih.gov, api.openalex.org, and other domains failed with `EGRESS_BLOCKED` in this environment. All candidates from this run were recorded `Unverified (verification blocked)`. **Superseded**: once the `mcp__PubMed__*` tools became available (Runs 3-6), the relevant candidates were re-verified through PubMed directly and re-recorded with `Verified` status where confirmed (see `sources/records/2023-ou-real-world-exon20-outcomes.md` and `sources/records/2022-kwon-exon20-meta-analysis.md`, upgraded from Unverified to Verified).

## Run 2 (superseded — see Runs 3-6)

- **Date:** 2026-09-08
- **Query:** `EGFR exon 20 insertion NSCLC clinical outcomes 2023 2024 site:pubmed.ncbi.nlm.nih.gov`
- **Tool/database:** Hosted web search (general), `site:` scoped
- **Filters:** `site:pubmed.ncbi.nlm.nih.gov`
- **Results returned:** 8 links surfaced
- **Notes:** Same verification failure as Run 1. A follow-up unstructured web-search-only pass (targeting acquired resistance and compound mutations) produced 5 more candidates, all likewise left `Unverified (verification blocked)`; those exploratory web-search candidates were **not** individually re-verified or carried forward — Runs 3-6 below re-ran clean, structured PubMed searches instead of trying to patch the old snippet-based candidate list.

## Run 3

- **Date:** 2026-09-08
- **Query:** `EGFR mutation subtype treatment response non-small cell lung cancer` (2022-2026, sorted by publication date)
- **Tool/database:** `mcp__PubMed__search_articles` (PubMed, via MCP — no longer subject to the WebFetch egress block)
- **Filters:** Date range 2022/01/01-2026/12/31 (publication date)
- **Results returned:** 15 of 159 total matches returned
- **Notes:** Broad pass on general subtype/treatment-response. Most on-topic hits were reviews (excluded from the evidence table per `research-question.md`'s preference for primary clinical studies) or not subtype-stratified. One included: PMID 42218657 (afatinib vs. osimertinib, uncommon EGFR mutations, real-world).

## Run 4

- **Date:** 2026-09-08
- **Query:** `EGFR exon 20 insertion NSCLC clinical outcomes` (2022-2026, sorted by publication date)
- **Tool/database:** `mcp__PubMed__search_articles`
- **Filters:** Date range 2022/01/01-2026/12/31
- **Results returned:** 10 of 137 total matches returned
- **Notes:** Targeted pass on the exon 20 insertion subtype. Included: PMID 42216441 (amivantamab, Italian ATLAS registry) and PMID 42239888 (mobocertinib, ctDNA resistance mechanisms). Cross-checked two candidates originally surfaced only via web search in Run 1/2 directly against PubMed metadata: PMID 37744306 and PMID 35621011 — both independently confirmed and upgraded to `Verified`.

## Run 5

- **Date:** 2026-09-08
- **Query:** `EGFR acquired resistance osimertinib mutation subtype NSCLC` (2022-2026, sorted by publication date)
- **Tool/database:** `mcp__PubMed__search_articles`
- **Filters:** Date range 2022/01/01-2026/12/31
- **Results returned:** 10 of 10 total matches returned
- **Notes:** Targeted pass on acquired-resistance mechanisms. Included: PMID 41790029 (ORCHARD phase II, resistance genomic profiling), PMID 42502985 ("Rebiopsy on Osi" real-world multicenter study), PMID 39694766 (PD-L1/T790M translational study, subtype-stratified by initial mutation). Excluded a case report (PMID 42466433, isolated C797S) per exclusion criteria — other resistance-mechanism evidence for this population already included.

## Run 6

- **Date:** 2026-09-08
- **Query:** `EGFR compound mutations non-small cell lung cancer clinical outcomes` (2022-2026, sorted by publication date)
- **Tool/database:** `mcp__PubMed__search_articles`
- **Filters:** Date range 2022/01/01-2026/12/31
- **Results returned:** 10 of 268 total matches returned
- **Notes:** Targeted pass on compound EGFR mutations. Included: PMID 42191070 (PACC/compound-mutation landscape and TKI-generation responsiveness, 15,851-sample cohort). Several other hits in this pass (MARIPOSA endpoint analysis PMID 42492306, VEGFA/VEGFR2 study PMID 42231027, LAURA safety analysis PMID 42296617) were excluded at intake — reviewed via `get_article_metadata`/abstract and found to report pooled EGFR-mutant outcomes without subtype-level stratification, per the exclusion criterion in `research-question.md`.

## Verification method (Runs 3-6)

Every candidate above was verified via `mcp__PubMed__get_article_metadata`
against its PMID — this returns PubMed's own authoritative record (title,
full author list, journal, year, volume/issue/pages, DOI, PMCID), not a
search snippet or AI-generated summary. No candidate in Runs 3-6 required
fallback to WebFetch/WebSearch for verification.

## Summary

- Total unique candidates evaluated across all runs: 15 (9 passed forward
  as `Verified`, 1 case report excluded at intake, 3 pooled/non-subtype
  studies excluded at intake, 2 superseded web-search-only candidates from
  Run 2 not re-verified/not carried forward).
- Passed forward to `evidence-reviewer`: 9, all `Verified`, 0 `Partial`,
  0 `Unverified`.
