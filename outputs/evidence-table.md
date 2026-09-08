# Evidence Table

Screened against `research-question.md` inclusion/exclusion criteria. All
rows below map to a `sources/records/*.md` entry with verification status
Verified or Partial, per QC Gate 2. Quantitative findings are taken
directly from the PubMed-confirmed title/abstract metadata for each PMID
(via `get_article_metadata`), not inferred or reconstructed.

According to PubMed, article details below are sourced from PubMed and
each row cites the article DOI.

---

### Ferro A, et al., 2024 — Resistance to first-line osimertinib in EGFR-mutated NSCLC

| Field | Value |
|---|---|
| Source record | `sources/records/PMID-38382773.md` |
| Study design | Narrative review (non-systematic; no stated systematic search methodology in the abstract). [DOI](https://doi.org/10.1016/j.critrevonc.2024.104295) |
| Population / system / sample | EGFR-mutated advanced NSCLC patients on first-line osimertinib (literature synthesis, not a defined patient cohort). |
| Intervention / exposure / comparator | First-line osimertinib (3rd-generation EGFR-TKI); no direct comparator arm (review). |
| Outcomes / endpoints | Pattern of clinical benefit/progression and categorization of resistance mechanisms (EGFR-dependent vs. EGFR-independent) as related to EGFR mutation subtype heterogeneity and concomitant genetic alterations. |
| Sample size | Not applicable (review article, no original cohort). |
| Key findings | Abstract states that heterogeneity in duration of benefit and pattern of progression on first-line osimertinib "might be related to molecular factors including subtypes of EGFR mutations and concomitant genetic alterations," and that acquired resistance separates into EGFR-dependent and EGFR-independent mechanistic classes. The abstract itself does not report subtype-specific quantitative figures (e.g., no percentages/HRs by subtype) — that level of detail, if present, would be in the full text, which was not retrieved. |
| Quality / limitations | Narrative review, not a primary study — presents synthesis/framework rather than new stratified data. Abstract-level access only for this record; if subtype-level quantitative detail is required, full text would need to be pulled and is not confirmed here. |
| Notes on conflict with other studies | Provides the conceptual resistance-mechanism framework (EGFR-dependent/independent) that Lin et al. 2025 (PMID 41273219) and Kim et al. 2026 (PMID 42239888) instantiate with primary genomic/ctDNA data — complementary, not conflicting. |
| Exclusion reason (if excluded instead) | N/A — included, but see quality note on review-level vs. primary-data scope; flagged to orchestrator as a scope ambiguity for narrative reviews generally (see handoff). |

---

### Shigematsu L, et al., 2025 — Later-generation EGFR-TKIs for uncommon EGFR mutations (multicenter real-world)

| Field | Value |
|---|---|
| Source record | `sources/records/PMID-41139406.md` |
| Study design | Retrospective multicenter (Keio University + affiliated hospitals) real-world cohort study. [DOI](https://doi.org/10.1111/1759-7714.70179) |
| Population / system / sample | Advanced/recurrent NSCLC with uncommon EGFR mutations (G719X, L861Q, S768I, and compound mutations), diagnosed 2014–2019, Japan; common mutations and exon 20 insertions excluded unless part of a compound mutation. |
| Intervention / exposure / comparator | Later-generation (2nd/3rd-gen) EGFR-TKI vs. first-generation EGFR-TKI (as initial or subsequent therapy); subtype (G719X vs. L861Q vs. S768I vs. compound) as stratifying variable. |
| Outcomes / endpoints | Overall survival (OS), by TKI generation and by mutation subtype; independent prognostic factors via multivariate Cox model. |
| Sample size | n = 35 patients. |
| Key findings | G719X was the most frequent uncommon mutation, followed by L861Q and S768I. 71% of patients eventually received a later-generation EGFR-TKI. Later-generation EGFR-TKI use was associated with significantly longer OS (47.7 vs. 15.5 months; p = 0.0177). Multivariate analysis identified non-use of later-generation EGFR-TKI, liver metastases, and poor performance status as independent poor prognostic factors. Afatinib showed favorable treatment duration specifically in G719X and compound mutation subtypes. |
| Sample size | n = 35. |
| Quality / limitations | Small sample (n=35) limits statistical power, especially for subtype-specific subgroup comparisons; single-country (Japan), retrospective (confounding by indication in TKI choice not fully controllable); PubMed metadata record itself has an incomplete trailing author entry (source record marked Partial for this reason, not a data-quality issue with the results). |
| Notes on conflict with other studies | Overlaps in population/geography/era with Nagano et al. 2026 (PMID 42218657) — both are Japanese multicenter retrospective real-world cohorts of uncommon EGFR mutations from overlapping recruitment periods. Patient/hospital overlap between the two cohorts cannot be ruled out from the abstracts; writer should not treat their sample sizes as fully independent evidence. Both studies concordantly favor afatinib for compound mutations, but Nagano additionally finds osimertinib favored specifically for L861X — a subtype-level nuance not present in this study. |
| Exclusion reason (if excluded instead) | N/A — included. |

---

### Lin F, et al., 2025 — Resistance mechanisms to afatinib in EGFR/ERBB2-mutated NSCLC

| Field | Value |
|---|---|
| Source record | `sources/records/PMID-41273219.md` |
| Study design | Retrospective genomic cohort study (targeted NGS, paired baseline/post-progression samples). [DOI](https://doi.org/10.1002/gcc.70088) |
| Population / system / sample | 37 NSCLC patients on first-line afatinib, harboring either EGFR (uncommon activating mutations) or ERBB2 activating mutations. Per source record, the ERBB2-mutated subgroup is outside strict EGFR scope and is excluded from EGFR-specific extraction below. |
| Intervention / exposure / comparator | First-line afatinib; EGFR-mutated vs. ERBB2-mutated as comparator groups; exon 20 insertion vs. exon 19 deletion as EGFR subtype comparator for resistance analysis. |
| Outcomes / endpoints | Progression-free survival (PFS); genomic features of primary and acquired resistance. |
| Sample size | n = 37 total (EGFR- and ERBB2-mutated combined; EGFR-only subgroup size not given in abstract). |
| Key findings | PFS on first-line afatinib was longer in EGFR-mutated than ERBB2-mutated patients (HR = 0.35, 95% CI 0.15–0.79, p = 0.008). Within the EGFR-relevant findings: primary resistance was associated with presence of EGFR exon 20 insertion mutation (p = 0.011); baseline EGFR exon 19 deletion, higher chromosomal instability, and age-related mutational signatures were associated with development of known acquired-resistance mechanisms (EGFR T790M, MET amplification). (ERBB2-specific novel resistance findings — loss of CDKN2A/NF1/ERBB2 mutation — are out of EGFR scope and not extracted here.) |
| Quality / limitations | Small sample (n=37, split across two molecular subgroups plus further EGFR-subtype comparisons), reducing power; single-arm retrospective design without an independent validation cohort; two co-authors affiliated with a commercial NGS vendor (Nanjing Geneseeq Technology) — potential conflict of interest in a genomics-vendor-linked resistance study, not disclosed as resolved in the abstract. |
| Notes on conflict with other studies | Exon 20 insertion associated with primary resistance to afatinib here is consistent with the broader literature (Zullo/Remon 2026, PMID 42512396; Spitaleri et al. 2026, PMID 41967619) that treats exon 20 insertion as a distinct, TKI-first-generation/second-generation-resistant entity requiring specific agents (sunvozertinib, amivantamab, mobocertinib). |
| Exclusion reason (if excluded instead) | N/A — included (EGFR-relevant findings only; ERBB2-specific findings excluded from extraction as out of scope). |

---

### Spitaleri G, et al., 2026 — Atypical EGFR mutations in NSCLC (review)

| Field | Value |
|---|---|
| Source record | `sources/records/PMID-41967619.md` |
| Study design | Narrative review (non-systematic per abstract). [DOI](https://doi.org/10.1016/j.critrevonc.2026.105327) |
| Population / system / sample | NSCLC patients with atypical/uncommon EGFR mutations (S768I, L861Q, G719X, and others), across published clinical studies (literature synthesis). |
| Intervention / exposure / comparator | First-, second-, and third-generation EGFR-TKIs across atypical-mutation subgroups; no single defined comparator (review). |
| Outcomes / endpoints | Therapeutic efficacy by TKI generation and by atypical mutation subtype; resistance mechanisms; structure-function-based classification of EGFR mutations. |
| Sample size | Not applicable (review). |
| Key findings | Atypical EGFR mutations account for approximately 12% of all EGFR alterations (per abstract). Afatinib remains the only agent with regulatory approval (FDA/EMA, 2018) specifically for selected atypical variants (S768I, L861Q, G719X); treatment recommendations for the wider spectrum of atypical mutations remain undefined, with practice often extrapolated from classical-mutation data or defaulting to chemotherapy. |
| Quality / limitations | Narrative review — synthesis-level evidence, not new primary data; abstract does not itemize subtype-specific efficacy statistics beyond the regulatory-approval framing described above. |
| Notes on conflict with other studies | Provides synthesis context for the atypical-mutation TKI-response findings in Shigematsu et al. 2025 (PMID 41139406) and Nagano et al. 2026 (PMID 42218657); no conflicting claims identified. |
| Exclusion reason (if excluded instead) | N/A — included; same review-scope caveat as PMID 38382773 above (flagged to orchestrator). |

---

### Zhou C, et al., 2026 — WU-KONG28: First-line sunvozertinib vs. chemotherapy in EGFR exon 20 insertion NSCLC (Phase 3 RCT)

| Field | Value |
|---|---|
| Source record | `sources/records/PMID-42212913.md` |
| Study design | Phase 3, international, randomized controlled trial (1:1 randomization), crossover permitted after confirmed progression. [DOI](https://doi.org/10.1056/NEJMoa2604461) |
| Population / system / sample | Advanced nonsquamous NSCLC with EGFR exon 20 insertion mutations, treatment-naive (first-line). |
| Intervention / exposure / comparator | Sunvozertinib vs. chemotherapy (carboplatin–pemetrexed). |
| Outcomes / endpoints | Primary: PFS (blinded independent central review). Secondary: OS, investigator-assessed PFS, objective response rate (ORR), change in tumor size, duration of response, safety. |
| Sample size | n = 324 (163 sunvozertinib, 161 chemotherapy). |
| Key findings | Median PFS 10.3 vs. 7.5 months (HR 0.65, 95% CI 0.50–0.85, p<0.001). 12-month PFS 46.1% vs. 26.7%. ORR 58.9% vs. 31.1%. Median best tumor-size change −42.1% vs. −24.7%. Median duration of response 11.2 vs. 7.1 months. OS data immature (38.9% maturity) at reporting. Grade ≥3 adverse events: 75.5% (sunvozertinib) vs. 56.7% (chemotherapy); no deaths attributed to sunvozertinib-related AEs. |
| Quality / limitations | Strongest design in this evidence set (randomized, phase 3, blinded central PFS review) — highest internal validity for the exon 20 insertion population. Industry-funded (Dizal Pharmaceuticals). OS immature, so long-term survival benefit not yet established. Higher rate of grade ≥3 AEs with sunvozertinib is a real tolerability trade-off against the efficacy gain. |
| Notes on conflict with other studies | Represents first-line data; contrasts with Passiglia et al. 2026 (PMID 42216441, amivantamab, largely post-chemotherapy/later-line real-world use) and Kim et al. 2026 (PMID 42239888, mobocertinib, post-amivantamab). Line-of-therapy differences mean ORR/PFS figures across these three exon 20 insertion studies are not directly comparable head-to-head; writer should represent them as evidence at different treatment lines, not pool them. |
| Exclusion reason (if excluded instead) | N/A — included. |

---

### Passiglia F, et al., 2026 — Amivantamab in EGFR exon 20 insertion NSCLC: Italian ATLAS real-world registry

| Field | Value |
|---|---|
| Source record | `sources/records/PMID-42216441.md` |
| Study design | Multicenter, retrospective, observational real-world registry study. [DOI](https://doi.org/10.1002/cncr.70476) |
| Population / system / sample | Advanced NSCLC with EGFR exon 20 insertion mutations, enrolled in the Italian ATLAS registry, Jan–Dec 2024. |
| Intervention / exposure / comparator | Single-agent amivantamab (in later lines, after first-line platinum-based chemotherapy ± immunotherapy in most patients); no randomized comparator (single-arm real-world). |
| Outcomes / endpoints | ORR, disease control rate (DCR), PFS, OS, intracranial response, treatment-related adverse events (TRAEs). |
| Sample size | n = 119 total registry patients; 64 of 119 received single-agent amivantamab in subsequent lines; 23 patients with brain metastases assessed for intracranial outcomes. |
| Key findings | ORR 37.5%, DCR 66.2%, median PFS 9.6 months, median OS 16.9 months under amivantamab. Among 23 patients with brain metastases: 13% partial intracranial response, 43.5% stable disease, intracranial median PFS 11.6 months. TRAEs of any grade in 68.8% (grade 3–4 in 10.9%), most commonly skin rash (56%, grade 3 in 9.4%), asthenia (9%), peripheral edema (8%), infusion-related reactions (9.4%, grade 3 in 1.5%). Dose interruptions/reductions/discontinuations due to TRAEs in 20.3%/12.5%/3.1%. |
| Quality / limitations | Real-world, retrospective, single-arm — no internal comparator group; heavily pretreated population (most had prior chemotherapy ± immunotherapy) limits generalizability to treatment-naive patients; results are described in the abstract as concordant with the pivotal CHRYSALIS trial, supporting external validity of the efficacy/safety signal in real-world use. |
| Notes on conflict with other studies | Efficacy magnitude (ORR ~38%) is lower than sunvozertinib's first-line ORR (58.9%, PMID 42212913), consistent with amivantamab being used in a later-line, more heavily pretreated population rather than a true head-to-head discrepancy — writer should attribute this to line-of-therapy/population differences, not agent superiority. |
| Exclusion reason (if excluded instead) | N/A — included. |

---

### Nagano Y, et al., 2026 — Afatinib vs. osimertinib for uncommon EGFR mutations: real-world outcomes (multicenter Japan)

| Field | Value |
|---|---|
| Source record | `sources/records/PMID-42218657.md` |
| Study design | Multicenter (29 hospitals, Japan) retrospective cohort study; inverse probability of treatment weighting (IPTW) used to adjust for baseline imbalances. [DOI](https://doi.org/10.1111/cas.70400) |
| Population / system / sample | Advanced/recurrent non-squamous NSCLC with uncommon EGFR mutations (excluding exon 20 insertions and de novo T790M), first-line afatinib or osimertinib, Jan 2015–Jan 2024. |
| Intervention / exposure / comparator | First-line afatinib (n=95) vs. first-line osimertinib (n=67); mutation subtype (L861X vs. compound mutations, etc.) as an effect-modifying stratifier. |
| Outcomes / endpoints | Time to treatment failure (TTF), overall survival (OS), response rate, subsequent-line outcomes (ICI + platinum doublet vs. platinum doublet alone in 56 patients who received further systemic therapy). |
| Sample size | n = 162 (afatinib 95, osimertinib 67); subsequent-therapy subgroup n = 56. |
| Key findings | Weighted analyses showed no significant difference between afatinib and osimertinib in TTF (HR 1.04, 95% CI 0.61–1.77) or OS (HR 1.34, 95% CI 0.73–2.44). Afatinib was associated with higher response rates but more frequent adverse events requiring dose reduction. Subgroup analysis suggested osimertinib favored for L861X mutations and afatinib favored for compound mutations. Among patients receiving subsequent therapy, ICI+platinum doublet and platinum doublet alone produced comparable outcomes. |
| Quality / limitations | Real-world retrospective design; IPTW mitigates but does not eliminate confounding by indication (vs. a true RCT). Subtype-specific subgroup findings (L861X, compound) are described as "suggested" in the abstract — likely exploratory/hypothesis-generating given probable small subgroup sizes, not confirmatory. |
| Notes on conflict with other studies | See note under Shigematsu et al. 2025 (PMID 41139406) regarding possible cohort/hospital overlap (both are Japanese multicenter real-world uncommon-EGFR-mutation cohorts from overlapping periods) — treat as potentially non-independent evidence. Both studies agree afatinib favors compound mutations; this study adds an L861X-specific osimertinib advantage not reported in Shigematsu et al. |
| Exclusion reason (if excluded instead) | N/A — included. |

---

### Kim J, et al., 2026 — Paired ctDNA analysis of resistance to mobocertinib in EGFR exon 20 insertion NSCLC

| Field | Value |
|---|---|
| Source record | `sources/records/PMID-42239888.md` |
| Study design | Single-center, prospective, observational study with paired pre-/post-treatment ctDNA sequencing. [DOI](https://doi.org/10.3389/fonc.2026.1827867) |
| Population / system / sample | 22 patients with EGFR exon 20 insertion-positive NSCLC treated with mobocertinib; 14 of the 22 had prior amivantamab exposure. |
| Intervention / exposure / comparator | Mobocertinib (targeted EGFR exon 20 inhibitor); insertion-site location (helical region vs. other) as a subtype-level stratifier; prior amivantamab exposure vs. none as a comparator. |
| Outcomes / endpoints | ORR, DCR, PFS (RECIST v1.1); acquired resistance mechanisms via paired ctDNA. |
| Sample size | n = 22 (14 with prior amivantamab exposure). |
| Key findings | ORR 59%, DCR 82%, median PFS 5.6 months (95% CI 3.5–9.3). In the amivantamab-pretreated subgroup (n=14): ORR 57.1%, median duration of response and PFS 5.1 and 5.8 months respectively. Better responses observed in helical-region insertions than other insertion sites. Baseline ctDNA absence was associated with favorable outcomes. Acquired resistance mechanisms were diverse: EGFR amplification, RTK/RAS pathway alterations, and rare events including gene fusion and small-cell lung cancer transformation. |
| Quality / limitations | Small single-center sample (n=22, with a 14-patient pretreated subgroup) limits statistical power and generalizability; no randomized comparator arm; prospective design and paired ctDNA methodology are methodological strengths for resistance-mechanism characterization specifically. |
| Notes on conflict with other studies | Confirms exon 20 insertion as resistance-prone/heterogeneous, consistent with Lin et al. 2025 (PMID 41273219, exon 20 insertion associated with primary afatinib resistance) and Reyes et al. 2026 (PMID 42291370, exon 20 insertion as a "distinct population"). Efficacy (ORR 59%) regardless of prior amivantamab is a later-line result and should not be compared directly to first-line sunvozertinib efficacy (PMID 42212913) without noting the line-of-therapy difference. |
| Exclusion reason (if excluded instead) | N/A — included. |

---

### Reyes A, et al., 2026 — CNS disease patterns and molecular landscape in EGFR exon 20 insertion NSCLC

| Field | Value |
|---|---|
| Source record | `sources/records/PMID-42291370.md` |
| Study design | Retrospective single-institution (plus network sites) cohort study. [DOI](https://doi.org/10.21037/tlcr-2026-1-0104) |
| Population / system / sample | 80 patients with NSCLC and EGFR exon 20 insertion mutations, seen 2014–2024 at a large cancer center and network sites. |
| Intervention / exposure / comparator | CNS progression status and TP53 co-mutation status as exposure variables (no treatment-arm comparison reported in abstract). |
| Outcomes / endpoints | Overall survival (OS); CNS metastasis/leptomeningeal disease patterns. |
| Sample size | n = 80. |
| Key findings | 36.25% of patients had CNS progression; 7.5% had leptomeningeal disease. Median OS was similar with vs. without CNS progression (45.3 vs. 47.8 months; HR 1.21, 95% CI 0.66–2.23, p=0.54 — not statistically significant). TP53 co-mutation was associated with numerically lower median OS (31.6 vs. 47.8 months; HR 1.79, 95% CI 0.89–3.60, p=0.11 — not statistically significant). |
| Quality / limitations | Retrospective, single-institution-anchored cohort; both key HRs are statistically non-significant with wide confidence intervals, indicating the study is likely underpowered to detect the associations it reports — findings should be described as suggestive/hypothesis-generating, not confirmed effects. |
| Notes on conflict with other studies | Reinforces the exon 20 insertion population as biologically/clinically distinct (echoed in Zullo & Remon 2026, PMID 42512396, and Spitaleri et al. 2026, PMID 41967619 for the broader uncommon-mutation category). No direct conflict with other included studies, but its non-significant findings should not be overstated as "no effect" given the small sample and wide CIs. |
| Exclusion reason (if excluded instead) | N/A — included. |

---

### Lu K, et al., 2026 — Compound EGFR mutations in advanced NSCLC: characteristics and clinical outcomes (brief report)

| Field | Value |
|---|---|
| Source record | `sources/records/PMID-42320198.md` |
| Study design | Retrospective, dual-cohort study: institutional cohort (UC San Diego Health) plus AACR GENIE database analysis; published as a "Brief Report." [DOI](https://doi.org/10.1016/j.cllc.2026.05.005) |
| Population / system / sample | Advanced EGFR-mutated NSCLC patients at UC San Diego Health, plus an independent GENIE-database cohort with EGFR mutations (including compound mutations). |
| Intervention / exposure / comparator | EGFR mutation subtype as exposure: L858R vs. exon 19 deletion (for de novo compound mutation rate); exon 19 deletion vs. L858R (for acquired C797S co-occurrence after osimertinib progression); S768I with vs. without co-mutation (GENIE); G719X alone vs. G719X/L861Q compound (osimertinib TTF). |
| Outcomes / endpoints | Rate of de novo compound mutation by baseline subtype; rate of acquired C797S co-occurrence by baseline subtype after osimertinib progression; osimertinib time to treatment failure (TTF) by compound-mutation subtype. |
| Sample size | Institutional cohort: 159 L858R and 228 exon19del patients (de novo compound analysis); 113 exon19del and 89 L858R patients (acquired C797S analysis, osimertinib-progressed). GENIE cohort size for S768I analysis not given in abstract. |
| Key findings | L858R patients were more likely than exon19del patients to have a de novo compound mutation (24/159 [15%] vs. 4/228 [2%], p<0.01). Acquired C797S more often co-occurred with exon19del than L858R after osimertinib progression (23/113 [20%] vs. 6/89 [7%], p<0.01). In GENIE, 88% of S768I-mutated patients had an additional EGFR co-mutation, most commonly G719X. Osimertinib TTF: median >13 months for co-mutated G719X/L861Q vs. <7 months for G719X alone. |
| Quality / limitations | "Brief Report" format constrains detail (abstract-level figures only retrieved here; full methodological detail on GENIE cohort size, follow-up, and multivariate adjustment not available from the abstract). Combines a single-institution clinical cohort with a multi-institutional genomic database (GENIE) that has heterogeneous data completeness/clinical annotation — the two data sources should not be treated as a single homogeneous cohort. |
| Notes on conflict with other studies | The G719X/L861Q compound-mutation TTF advantage on osimertinib is complementary to, but not directly comparable with, Nagano et al. 2026 (PMID 42218657), which found afatinib (not osimertinib) favored for compound mutations generally — different index drugs, so the two findings should be presented side-by-side rather than merged. |
| Exclusion reason (if excluded instead) | N/A — included. |

---

### Zullo L & Remon J, 2026 — New treatment strategies for EGFR exon 20 insertions (and HER2-deregulated) lung cancer (review)

| Field | Value |
|---|---|
| Source record | `sources/records/PMID-42512396.md` |
| Study design | Narrative review (non-systematic per abstract). [DOI](https://doi.org/10.3390/cancers18142334) |
| Population / system / sample | NSCLC with EGFR exon 20 insertion mutations (EGFR-specific portion only; the HER2-deregulated NSCLC portion of this review is out of strict EGFR scope and is excluded from extraction here, per the source record's own scope note). |
| Intervention / exposure / comparator | Review of diagnostic approaches (NGS, biomarker testing) and therapeutic landscape (chemotherapy, immunotherapy, targeted agents including TKIs and antibody-based therapies) specific to EGFR exon 20 insertion NSCLC; no single defined comparator (review). |
| Outcomes / endpoints | Epidemiology, molecular biology, diagnostic approach, and evolving treatment/resistance landscape for EGFR exon 20 insertion NSCLC. |
| Sample size | Not applicable (review). |
| Key findings | Synthesizes epidemiology and evolving targeted-therapy landscape for EGFR exon 20 insertion NSCLC, addressing treatment resistance, molecular heterogeneity, and optimal therapeutic sequencing as major open challenges; abstract does not itemize original quantitative efficacy data (those are covered by the primary studies above, e.g., PMID 42212913, 42216441, 42239888). |
| Quality / limitations | Narrative review — synthesis-level evidence, not new primary data; provides context/sequencing framework rather than independently verifiable numbers. |
| Notes on conflict with other studies | Synthesizes and is consistent with the exon 20 insertion primary-data studies above (sunvozertinib, amivantamab, mobocertinib); no conflicting claims identified. |
| Exclusion reason (if excluded instead) | N/A — included; same review-scope caveat as PMID 38382773 and PMID 41967619 above (flagged to orchestrator); HER2-specific content excluded from extraction as out of EGFR scope. |

---

## Excluded at this stage

| Source record | Title (short) | Exclusion reason |
|---|---|---|
| `sources/records/PMID-42453333.md` | Jing R, et al. — Impact of multiple gene mutations on EGFR-TKI response in Asian NSCLC patients | Excluded — this review's primary exposure variable is concurrent/co-occurring driver-gene mutations (KRAS, ALK, MET, PIK3CA, BRAF, ROS1, HER2) in EGFR-mutant NSCLC generally, not EGFR-mutation-subtype-stratified treatment response/resistance/outcome data as required by the inclusion criteria. The abstract does not report outcomes stratified by EGFR mutation subtype (exon19del/L858R/exon20ins/G719X/etc.); it discusses the EGFR-mutant population pooled against co-mutation status, which the exclusion criteria flags as insufficient ("studies not reporting subtype-level ... data"). |

---

## Flagged ambiguity for orchestrator (not a screening exclusion)

`research-question.md` "Study types" scope lists clinical studies (preferred) and mechanistic/basic studies tied to clinical outcome data, but does not explicitly state whether narrative review articles are in-scope "studies." Three of the 11 included records (PMID-38382773, PMID-41967619, PMID-42512396) are narrative reviews rather than primary-data studies. I have included them under a literal reading of the inclusion criteria (they do report treatment-response/resistance/outcome information stratified by EGFR mutation subtype, drawn from the literature, and nothing in the written exclusion criteria bars review articles), but I have appraised them explicitly as synthesis-level evidence, not primary data, in the Quality/limitations field of each row. This is a judgment call on an unwritten criterion — flagging it so the orchestrator/user can confirm whether narrative reviews should count toward the "clinical studies preferred" study-type framework, or should be treated as background-only and excluded from the evidence table in a future pass.
