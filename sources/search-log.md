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
