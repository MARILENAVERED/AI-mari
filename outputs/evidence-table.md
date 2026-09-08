# Evidence Table

Screened against `research-question.md` (updated 2026-09-08, excluding narrative
reviews as evidence). Source: PubMed (`mcp__PubMed__get_article_metadata`,
cross-checked against `sources/records/*.md`). All records below carried
verification status `Verified` or `Partial` and disposition "Pass forward to
evidence-reviewer" at intake — no Gate 1 violations found in this batch.

**Screened:** 8 candidate records (plus 3 previously-forwarded records now
reclassified as excluded at intake per the updated study-type criterion — see
Excluded section).
**Included:** 8
**Excluded:** 3 (all narrative reviews, excluded at intake — see below)

---

## Included studies

### Shigematsu et al., 2025 — Later-generation EGFR-TKIs for uncommon EGFR mutations (multicenter real-world)

| Field | Value |
|---|---|
| Source record | `sources/records/PMID-41139406.md` |
| Study design | Retrospective multicenter cohort (real-world), Kaplan-Meier/log-rank/Cox regression analysis |
| Population / system / sample | Adult NSCLC patients with uncommon EGFR mutations (G719X, L861Q, S768I, compound mutations), diagnosed 2014–2019 at Keio University Hospital and affiliated hospitals; common mutations and exon 20 insertions excluded unless part of a compound mutation |
| Intervention / exposure / comparator | Later-generation (2nd/3rd-gen) vs. earlier/no later-generation EGFR-TKI use; subtype-stratified (G719X, L861Q, S768I, compound) |
| Outcomes / endpoints | Overall survival (OS); treatment duration by subtype/agent (swimmer plots); multivariate prognostic factors |
| Sample size | n = 35 |
| Key findings | 71% of patients eventually received a later-generation TKI; later-generation TKI use associated with significantly longer OS (47.7 vs. 15.5 months; p = 0.0177). Non-use of later-generation TKI, liver metastases, and poor performance status were independent poor prognostic factors (multivariate). Afatinib showed favorable treatment duration specifically in G719X and compound-mutation subgroups. |
| Quality / limitations | Small sample (n=35) limits subgroup precision and generalizability; retrospective, non-randomized (confounding by indication likely — patients selected for later-generation TKIs may differ systematically); single-country/two-institution network; no formal comparator arm for subtype-specific HRs beyond descriptive treatment-duration comparisons; abstract does not report ORR or PFS by subtype, only OS and treatment duration. |
| Notes on conflict with other studies | Complementary to PMID-42218657 (Nagano et al.) on afatinib's favorable performance in compound-mutation subgroups; both support afatinib as relatively favorable for compound mutations, though via different comparators (later- vs. earlier-generation TKI here, vs. afatinib-vs-osimertinib head-to-head there). |
| Exclusion reason (if excluded instead) | N/A — included |

### Lin et al., 2025 — Novel resistance mechanisms to afatinib by genomic features

| Field | Value |
|---|---|
| Source record | `sources/records/PMID-41273219.md` |
| Study design | Retrospective genomic cohort study (targeted NGS, baseline and post-progression paired samples) |
| Population / system / sample | 37 NSCLC patients with EGFR- or ERBB2-activating mutations receiving first-line afatinib. **Note: only the EGFR-mutated subgroup is in scope; the ERBB2-mutated subgroup is excluded from EGFR-specific extraction per the source record's own relevance note.** |
| Intervention / exposure / comparator | First-line afatinib; EGFR-mutated vs. ERBB2-mutated comparison; exon 20 insertion vs. other EGFR subtypes for primary resistance |
| Outcomes / endpoints | Progression-free survival (PFS); genomic resistance mechanisms (primary and acquired) |
| Sample size | n = 37 (EGFR- and ERBB2-mutated combined; EGFR-only subset size not separately reported in abstract) |
| Key findings | PFS on first-line afatinib was longer in EGFR-mutated than ERBB2-mutated patients (HR = 0.35, 95% CI 0.15–0.79, p = 0.008). Primary resistance was associated with EGFR exon 20 insertion (p = 0.011), higher tumor mutational burden (p = 0.009), and higher APOBEC signature (p = 0.012) — these were enriched in the ERBB2-mutated cohort. Baseline EGFR exon 19 deletion plus higher chromosomal instability/age-related mutational signatures were associated with development of known acquired-resistance mechanisms (T790M, MET amplification). |
| Quality / limitations | Small combined sample (n=37) with mixed EGFR/ERBB2 populations, further reducing EGFR-specific subgroup size and statistical power; retrospective; abstract-level detail does not break out EGFR-only PFS or subtype-specific (e.g., exon19del vs. exon20ins) HRs separately from the EGFR-vs-ERBB2 comparison — this is a limitation of what full-text-level detail is available at the abstract level and should be flagged as such rather than presented as complete evidence. |
| Notes on conflict with other studies | None identified directly; provides mechanistic (genomic) resistance detail complementary to the more clinically-oriented resistance data in Kim et al. (PMID-42239888, mobocertinib/ctDNA) and Lu et al. (PMID-42320198, compound mutations/C797S). |
| Exclusion reason (if excluded instead) | N/A — included |

### Zhou et al., 2026 — First-line sunvozertinib vs. chemotherapy in EGFR exon 20 insertion NSCLC (WU-KONG28, phase 3 RCT)

| Field | Value |
|---|---|
| Source record | `sources/records/PMID-42212913.md` |
| Study design | Phase 3, international, randomized controlled trial (1:1, open-label per abstract; blinded independent central review of primary endpoint); crossover permitted after progression |
| Population / system / sample | Adults with advanced nonsquamous NSCLC harboring EGFR exon 20 insertion mutations |
| Intervention / exposure / comparator | First-line sunvozertinib vs. chemotherapy (carboplatin-pemetrexed) |
| Outcomes / endpoints | Primary: PFS (blinded independent central review). Secondary: OS, investigator-assessed PFS, ORR, change in tumor size, duration of response, safety |
| Sample size | n = 324 (163 sunvozertinib, 161 chemotherapy) |
| Key findings | Median PFS 10.3 vs. 7.5 months (HR 0.65, 95% CI 0.50–0.85, P<0.001) favoring sunvozertinib. 12-month PFS: 46.1% vs. 26.7%. ORR: 58.9% vs. 31.1%. Median best tumor-size reduction: −42.1% vs. −24.7%. Median duration of response: 11.2 vs. 7.1 months. OS data immature (38.9% maturity) at time of report. Grade ≥3 adverse events: 75.5% (sunvozertinib) vs. 56.7% (chemotherapy); no treatment-related deaths attributed to sunvozertinib. |
| Quality / limitations | Highest design strength in this evidence set (randomized, phase 3, blinded independent central review of primary endpoint) — strong internal validity for the exon 20 insertion population. Industry-funded (Dizal Pharmaceuticals); OS immature, so long-term survival benefit not yet established; higher grade ≥3 AE rate with sunvozertinib is a tolerability trade-off; crossover design may attenuate any eventual OS difference. |
| Notes on conflict with other studies | Provides first-line RCT-level efficacy benchmark against which the real-world amivantamab data (Passiglia et al., PMID-42216441, later-line/real-world population) and mobocertinib ctDNA data (Kim et al., PMID-42239888) should be read as later-line, non-randomized, and not directly comparable on trial phase or line of therapy — research-writer should not present these as head-to-head equivalent evidence. |
| Exclusion reason (if excluded instead) | N/A — included |

### Passiglia et al., 2026 — Amivantamab in EGFR exon 20 insertion NSCLC (Italian ATLAS real-world registry)

| Field | Value |
|---|---|
| Source record | `sources/records/PMID-42216441.md` |
| Study design | Multicenter, retrospective, observational real-world registry study |
| Population / system / sample | Advanced NSCLC patients with EGFR exon 20 insertion mutations enrolled in the Italian ATLAS registry, Jan–Dec 2024 |
| Intervention / exposure / comparator | Single-agent amivantamab (in subsequent treatment lines, after first-line chemotherapy ± immunotherapy) |
| Outcomes / endpoints | ORR, disease control rate (DCR), PFS, OS, intracranial response/PFS in patients with brain metastasis, treatment-related adverse events (TRAEs) |
| Sample size | n = 119 total registry population; 64/119 received amivantamab |
| Key findings | Among amivantamab-treated patients: ORR 37.5%, DCR 66.2%, median PFS 9.6 months, median OS 16.9 months. Among 23 patients with brain metastasis: 13% partial intracranial response, 43.5% stable disease, intracranial median PFS 11.6 months. TRAEs any grade 68.8%, grade 3–4 10.9% (most common: skin rash 56%/G3 9.4%, asthenia 9%, peripheral edema 8%, infusion-related reactions 9.4%/G3 1.5%). Authors describe results as confirming the efficacy/safety profile seen in the CHRYSALIS trial in a heavily pretreated real-world population. |
| Quality / limitations | Real-world retrospective design without a concurrent comparator arm (no internal control group for amivantamab efficacy claims); single-country (Italy); later-line, heavily pretreated population, not directly comparable to first-line RCT data; potential selection bias in which patients received amivantamab (64/119) vs. other subsequent therapies. |
| Notes on conflict with other studies | Not in direct conflict, but represents a different line of therapy and design (real-world, later-line) from the first-line RCT in Zhou et al. (PMID-42212913) — writer should not conflate the two ORR/PFS figures as measuring the same population or setting. |
| Exclusion reason (if excluded instead) | N/A — included |

### Nagano et al., 2026 — Afatinib vs. osimertinib for uncommon EGFR mutations (real-world, 29-hospital Japan)

| Field | Value |
|---|---|
| Source record | `sources/records/PMID-42218657.md` |
| Study design | Multicenter retrospective cohort study; inverse probability of treatment weighting (IPTW) used to adjust for baseline imbalances (not a randomized comparison) |
| Population / system / sample | Advanced/recurrent non-squamous NSCLC with uncommon EGFR mutations (excluding exon 20 insertions and de novo T790M), first-line afatinib or osimertinib, Jan 2015–Jan 2024, 29 hospitals in Japan |
| Intervention / exposure / comparator | First-line afatinib (n=95) vs. osimertinib (n=67), IPTW-adjusted comparison; subgroup analysis by mutation subtype (L861X, compound mutations) |
| Outcomes / endpoints | Time to treatment failure (TTF), overall survival (OS), response rate, adverse events requiring dose reduction; outcomes of subsequent ICI-based regimens in a 56-patient subset |
| Sample size | n = 162 (afatinib 95, osimertinib 67) |
| Key findings | No significant difference in weighted TTF (HR 1.04, 95% CI 0.61–1.77) or OS (HR 1.34, 95% CI 0.73–2.44) between afatinib and osimertinib overall. Afatinib associated with higher response rates but more frequent adverse events requiring dose reduction. Subgroup analysis suggested osimertinib favored L861X mutations while afatinib favored compound mutations. Among 56 patients receiving subsequent systemic therapy, ICI+platinum doublet vs. platinum doublet alone showed comparable outcomes. |
| Quality / limitations | Retrospective, non-randomized (IPTW mitigates but does not eliminate confounding by indication); subgroup analyses (by mutation subtype) are almost certainly underpowered given n=162 split across afatinib/osimertinib and further split by subtype — abstract does not report subgroup sample sizes or formal interaction p-values, so subtype-specific claims (L861X/compound) should be treated as hypothesis-generating, not definitive; single-country (Japan). |
| Notes on conflict with other studies | Directly complementary to Shigematsu et al. (PMID-41139406): both point to afatinib performing relatively well in compound-mutation subgroups, using different comparators. No direct conflict identified, but the head-to-head "no significant overall difference between afatinib and osimertinib" finding here should be read alongside the subtype-specific afatinib benefit reported in Shigematsu et al., since the two studies examine overlapping but not identical subtype populations and comparators — writer should represent this as consistent-but-not-identical evidence, not merge the findings. |
| Exclusion reason (if excluded instead) | N/A — included |

### Kim et al., 2026 — Paired ctDNA analysis of resistance mechanisms to mobocertinib in EGFR exon 20 insertion NSCLC

| Field | Value |
|---|---|
| Source record | `sources/records/PMID-42239888.md` |
| Study design | Single-center, prospective, observational study with paired pre-/post-treatment ctDNA sequencing |
| Population / system / sample | 22 patients with EGFR exon 20 insertion-positive NSCLC treated with mobocertinib |
| Intervention / exposure / comparator | Mobocertinib (EGFR exon 20 inhibitor); subgroup comparison by prior amivantamab exposure (n=14) and by insertion-site location (helical region vs. other) |
| Outcomes / endpoints | ORR, DCR, PFS, duration of response, ctDNA-defined resistance mechanisms |
| Sample size | n = 22 |
| Key findings | ORR 59%, DCR 82%, median PFS 5.6 months (95% CI 3.5–9.3). In the 14 patients with prior amivantamab exposure: ORR 57.1%, median duration of response and PFS 5.1 and 5.8 months respectively. Better responses in helical-region insertions; baseline ctDNA absence correlated with favorable outcomes. Resistance mechanisms were diverse: EGFR amplification, RTK/RAS pathway alterations, and rarer events (gene fusion, small-cell transformation). |
| Quality / limitations | Very small sample (n=22, with a 14-patient sub-subgroup) — limits statistical reliability of subgroup (insertion-site, prior-amivantamab) comparisons; single-center; observational, no comparator arm for efficacy claims; generalizability to broader exon 20 insertion population is uncertain given single-center Korean cohort. |
| Notes on conflict with other studies | Efficacy figures (ORR 59%, mPFS 5.6 months) for mobocertinib in a later-line, single-center population are not directly comparable to the first-line RCT efficacy of sunvozertinib (PMID-42212913) or the real-world amivantamab data (PMID-42216441) — different agents, lines of therapy, and populations; should not be presented as comparative agent-vs-agent evidence. |
| Exclusion reason (if excluded instead) | N/A — included |

### Reyes et al., 2026 — CNS disease patterns and molecular landscape in EGFR exon 20 insertion NSCLC

| Field | Value |
|---|---|
| Source record | `sources/records/PMID-42291370.md` |
| Study design | Retrospective cohort study, single large institution and network sites |
| Population / system / sample | 80 patients with NSCLC and EGFR exon 20 insertion mutations, 2014–2024 |
| Intervention / exposure / comparator | Exposure of interest: CNS progression status and TP53 co-mutation status (not a treatment intervention study) |
| Outcomes / endpoints | Overall survival stratified by CNS progression and by TP53 co-mutation status; CNS/leptomeningeal disease incidence |
| Sample size | n = 80 |
| Key findings | 36.25% of patients had CNS progression; 7.5% had leptomeningeal disease. Median OS similar regardless of CNS progression (45.3 months with progression vs. 47.8 months without; HR 1.21, 95% CI 0.66–2.23, P=0.54 — not statistically significant). Co-occurring TP53 mutation was associated with numerically lower median OS (31.6 vs. 47.8 months; HR 1.79, 95% CI 0.89–3.60, P=0.11 — not statistically significant). |
| Quality / limitations | Both key survival comparisons reported are statistically non-significant (wide confidence intervals crossing 1, p>0.05) — these are hypothesis-generating/descriptive findings, not confirmed prognostic associations, and should be represented as such rather than as established effects; retrospective; single-institution-network; no formal comparator/treatment-effect analysis. |
| Notes on conflict with other studies | No direct conflict with other included studies (none of the others report CNS-specific or TP53 co-mutation OS data for exon 20 insertion NSCLC specifically), though the Passiglia et al. amivantamab study (PMID-42216441) reports intracranial response data in a treated subgroup — these are complementary (natural history vs. treatment-response angles on CNS disease), not directly comparable endpoints. |
| Exclusion reason (if excluded instead) | N/A — included |

### Lu et al., 2026 — Characteristics and outcomes of de novo and acquired compound EGFR mutations (brief report)

| Field | Value |
|---|---|
| Source record | `sources/records/PMID-42320198.md` |
| Study design | Retrospective cohort study (brief report), combining an institutional cohort (UC San Diego Health) and the AACR GENIE database |
| Population / system / sample | Advanced EGFR-mutated NSCLC patients; institutional cohort with L858R (n=159) and exon19del (n=228) baseline populations for de novo compound-mutation analysis, and a separate osimertinib-progression cohort (exon19del n=113, L858R n=89) for acquired C797S analysis; GENIE database used for S768I co-mutation frequency |
| Intervention / exposure / comparator | Osimertinib (for time-to-treatment-failure analysis by compound-mutation subtype); comparator is baseline mutation type (L858R vs. exon19del) for de novo/acquired compound mutation rates |
| Outcomes / endpoints | Frequency of de novo compound mutations by baseline mutation type; frequency of acquired C797S by baseline mutation type; osimertinib time to treatment failure (TTF) by compound-mutation subtype |
| Sample size | Institutional cohort: 159 (L858R) + 228 (exon19del) for de novo analysis; 113 (exon19del) + 89 (L858R) for acquired C797S analysis; GENIE database subset for S768I (denominator not specified in abstract) |
| Key findings | L858R patients more likely to have a de novo compound mutation than exon19del patients (24/159 [15%] vs. 4/228 [2%], P<.01). Acquired C797S more often co-occurred with exon19del than L858R after osimertinib progression (23/113 [20%] vs. 6/89 [7%], P<.01). In GENIE, 88% of S768I-mutated patients had an additional EGFR co-mutation, most commonly G719X. Osimertinib TTF: compound G719X/L861Q median TTF >13 months vs. G719X-alone median TTF <7 months. |
| Quality / limitations | Explicitly a "brief report" — abstract-level findings likely represent a condensed subset of full analyses; combines an institutional cohort with a separate public database (GENIE) using different ascertainment methods, so cross-cohort comparisons (e.g., S768I/G719X frequency vs. institutional TTF figures) should not be treated as a single unified dataset; retrospective; TTF comparison (G719X/L861Q vs. G719X alone) does not report a formal hazard ratio, CI, or p-value in the abstract — presented as a descriptive median comparison only, and should be flagged as such rather than treated as a statistically confirmed difference. |
| Notes on conflict with other studies | Complementary to Shigematsu et al. (PMID-41139406) and Nagano et al. (PMID-42218657) in describing favorable outcomes for specific compound-mutation subgroups (G719X/L861Q here on osimertinib; G719X/compound on afatinib in the other two) — together these suggest compound-mutation subtype matters for TKI choice, but the three studies use different TKIs, comparators, and endpoints, so should not be merged into a single quantitative claim. |
| Exclusion reason (if excluded instead) | N/A — included |

---

## Excluded

| Source record | Reason for exclusion |
|---|---|
| `sources/records/PMID-38382773.md` (Ferro et al., 2024) | Narrative review (non-systematic, no stated search methodology). Excluded per updated `research-question.md` study-type criteria (2026-09-08). Not entered into evidence table or usable as cited support in the report. |
| `sources/records/PMID-41967619.md` (Spitaleri et al., 2026) | Narrative review (non-systematic, no stated search methodology). Excluded per updated `research-question.md` study-type criteria (2026-09-08). Not entered into evidence table or usable as cited support in the report. |
| `sources/records/PMID-42512396.md` (Zullo & Remon, 2026) | Narrative review (non-systematic, no stated search methodology). Excluded per updated `research-question.md` study-type criteria (2026-09-08). Not entered into evidence table or usable as cited support in the report. |

No other candidate records were screened as part of this pass (the 15
remaining records in `sources/records/` beyond these 11 were not part of
the batch handed off for this screening round and are outside this table's
scope).

---

## Ambiguities / judgment calls flagged, not silently resolved

- Lin et al. (PMID-41273219) reports a mixed EGFR/ERBB2 cohort (n=37); the
  research question's population is EGFR-mutated NSCLC specifically. The
  EGFR-vs-ERBB2 comparative PFS finding (HR 0.35) is retained because it is
  directly about EGFR mutation status as a variable, but the abstract does
  not give an EGFR-only sample size or EGFR-subtype-specific PFS broken out
  separately from the EGFR-vs-ERBB2 contrast — this is a genuine
  abstract-level data gap, not an extraction choice, and is flagged in that
  study's "Quality / limitations" row rather than papered over.
- Several subtype-specific claims (Nagano et al.'s L861X/compound subgroup
  results; Lu et al.'s G719X/L861Q vs. G719X-alone TTF comparison) are
  reported in the source abstracts as descriptive/subgroup findings without
  accompanying subgroup sample sizes, hazard ratios, or p-values. These are
  extracted as reported, but explicitly flagged as likely underpowered or
  non-formally-tested, per the anti-fabrication principle of not
  reconstructing precision that isn't in the source.
