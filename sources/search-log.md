# Search Log

Reproducible record of every search run performed by `literature-scout`.

---

## Run 1

- **Date:** 2026-09-08
- **Query:** `EGFR mutation subtype treatment response acquired resistance NSCLC 2023 2024 PubMed`
- **Tool/database:** Hosted web search (general), results dominated by
  pubmed.ncbi.nlm.nih.gov and pmc.ncbi.nlm.nih.gov listings
- **Filters:** None applied at the tool level (no native date/study-type
  filter available); recency implied via query terms only
- **Results returned:** 8 links surfaced
- **Notes:** Broad discovery pass per `research-question.md` scope
  (EGFR-mutant NSCLC, treatment response, resistance, subtype-level data,
  2022–2026). Follow-up verification via direct WebFetch to
  pubmed.ncbi.nlm.nih.gov, eutils.ncbi.nlm.nih.gov, api.openalex.org,
  openalex.org, and a publisher domain (esmoopen.com) **all failed** with
  `EGRESS_BLOCKED` — this environment's network egress proxy blocks those
  domains outright (confirmed by also testing an unrelated domain,
  en.wikipedia.org, which was blocked identically). **Bibliographic
  verification against a primary source could not be performed in this
  environment.** See `sources/records/` — all candidates from this run are
  therefore recorded as `Unverified (verification blocked)`, not `Verified`,
  per the anti-fabrication rule.

## Run 2

- **Date:** 2026-09-08
- **Query:** `EGFR exon 20 insertion NSCLC clinical outcomes 2023 2024 site:pubmed.ncbi.nlm.nih.gov`
- **Tool/database:** Hosted web search (general), scoped with `site:` to
  PubMed listings
- **Filters:** `site:pubmed.ncbi.nlm.nih.gov`; recency via query terms
- **Results returned:** 8 links surfaced
- **Notes:** Targeted pass on the exon 20 insertion subtype (an
  uncommon/rare EGFR subtype named explicitly in `research-question.md`).
  Same verification failure as Run 1 — see above.

## Run 3

- **Date:** 2026-09-08
- **Query:** `EGFR acquired resistance mechanisms osimertinib NSCLC mutation subtype 2024 2025`
- **Tool/database:** Hosted web search (general); results dominated by
  pubmed.ncbi.nlm.nih.gov, pmc.ncbi.nlm.nih.gov, and oaepublish.com listings
- **Filters:** None applied at the tool level; recency implied via query
  terms only
- **Results returned:** 7 links surfaced
- **Notes:** Targeted pass on the acquired-resistance-mechanism arm of the
  research question (not previously targeted directly in Runs 1–2, which
  focused on general subtype/treatment-response and exon 20 specifically).
  Surfaced subtype-specific resistance classifications (e.g., PACC subtype:
  G719X, S768I, C797S) tying directly to `research-question.md` scope.
  Re-confirmed environment egress restriction is not limited to
  pubmed/OpenAlex: WebFetch to www.oaepublish.com and pmc.ncbi.nlm.nih.gov
  also returned `EGRESS_BLOCKED`. Bibliographic verification against a
  primary source could not be performed. Both new candidates from this run
  recorded as `Unverified (verification blocked)` — see
  `sources/records/2025-osimertinib-acquired-resistance-review.md` and
  `sources/records/2025-heterogeneous-resistance-first-line-osimertinib.md`.

## Run 4

- **Date:** 2026-09-08
- **Query:** `EGFR compound mutations NSCLC clinical outcomes 2024 2025 PFS OS`
- **Tool/database:** Hosted web search (general); results included
  pmc.ncbi.nlm.nih.gov, sciencedirect.com, ncbi.nlm.nih.gov/pmc, and
  onlinelibrary.wiley.com listings
- **Filters:** None applied at the tool level; recency implied via query
  terms only
- **Results returned:** 8 links surfaced
- **Notes:** Targeted pass on compound EGFR mutations and uncommon-subtype
  clinical outcome data (PFS/OS), an arm of the research question not yet
  directly searched in Runs 1–3. Surfaced a multicenter retrospective study
  on compound mutations, a multicenter real-world study on later-generation
  TKIs for uncommon mutations, a broad high-impact review (CA: A Cancer
  Journal for Clinicians), and a single-patient case report. The case report
  was excluded at intake per `research-question.md` exclusion criteria
  (case reports excluded unless no other evidence exists on that rare
  subtype — other multicenter evidence on compound mutations was found in
  the same pass). Attempted WebFetch verification against
  www.sciencedirect.com and acsjournals.onlinelibrary.wiley.com (in addition
  to previously-tested ncbi.nlm.nih.gov domains) — both also returned
  `EGRESS_BLOCKED`, confirming the restriction is a blanket network egress
  block in this environment, not specific to PubMed/OpenAlex. Remaining new
  candidates from this run recorded as `Unverified (verification blocked)`
  — see `sources/records/2025-compound-egfr-mutations-clinical-outcomes.md`,
  `sources/records/2025-later-generation-tkis-uncommon-mutations.md`, and
  `sources/records/2025-personalized-care-egfr-mutant-nsclc-review.md`.
