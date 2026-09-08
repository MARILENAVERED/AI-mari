# Evidence Table

Canonical working evidence table for the research question in
`research-question.md`. Populated by `evidence-reviewer` from
`sources/records/*.md` (all status `Verified`), with extraction drawn
from each study's PubMed-indexed abstract (confirmed via
`mcp__PubMed__get_article_metadata` against the PMID already verified in
the source record — reading detail on an already-verified candidate, not
new discovery). Row structure follows `templates/evidence-table-row.md`.

**Note on extraction depth:** figures below are as reported in the
PubMed abstract. Full-text-only detail (e.g. complete subgroup breakdowns,
supplementary tables) was not retrieved in this pass; where the abstract
doesn't state a figure, the row says so explicitly rather than guessing.

---

## Included studies

### Nagano et al., 2026 — Afatinib vs. osimertinib in uncommon EGFR-mutant NSCLC (real-world)

| Field | Value |
|---|---|
| Source record | `sources/records/2026-nagano-afatinib-vs-osimertinib-uncommon-egfr.md` |
| Study design | Multicenter (29 hospitals, Japan), retrospective cohort; inverse probability of treatment weighting (IPTW) to adjust for baseline imbalance (not randomized) |
| Population / system / sample | Advanced/recurrent non-squamous NSCLC with uncommon EGFR mutations (UMs), excluding exon 20 insertions and de novo T790M; treated Jan 2015–Jan 2024 |
| Intervention / exposure / comparator | First-line afatinib (n=95) vs. osimertinib (n=67) |
| Outcomes / endpoints | Time to treatment failure (TTF), overall survival (OS), response rate, adverse events; post-TKI treatment patterns (including subsequent ICI-based regimens) |
| Sample size | 162 (afatinib 95, osimertinib 67) |
| Key findings | No significant difference in TTF (HR 1.04, 95% CI 0.61–1.77) or OS (HR 1.34, 95% CI 0.73–2.44) between afatinib and osimertinib overall. Afatinib associated with higher response rates but more dose-reduction-requiring AEs. **Subtype-dependent effect**: osimertinib favored for L861X mutations, afatinib favored for compound mutations. Subsequent ICI+platinum vs. platinum alone showed comparable outcomes (n=56). |
| Quality / limitations | Retrospective, non-randomized (confounding by indication for drug choice, only partly mitigated by IPTW); multicenter design supports generalizability within Japan; wide confidence intervals (crossing 1) on both HRs reflect limited power to detect a moderate difference — a "no significant difference" is not strong evidence of true equivalence, especially within subtype subgroups analyzed post hoc |
| Notes on conflict with other studies | Subtype-dependent TKI preference partially echoes Liu et al. 2026 (2nd-gen preference in PACC/compound mutations) — Nagano's afatinib-favors-compound-mutations finding is directionally consistent with Liu's 2nd-gen-favors-PACC/compound finding, though the two studies use different designs and populations; treat as corroborating, not identical, evidence |
| Exclusion reason (if excluded instead) | N/A — included |

### Liu et al., 2026 — Compound EGFR mutations (PACC): TKI-generation responsiveness

| Field | Value |
|---|---|
| Source record | `sources/records/2026-liu-compound-egfr-mutations-pacc-tki-response.md` |
| Study design | Mixed: genomic/molecular landscape characterization (cfDNA) + in vitro drug-sensitivity assays (Ba/F3 models) + retrospective real-world clinical outcomes cohort |
| Population / system / sample | 15,851 EGFR-mutant NSCLC cfDNA samples for landscape characterization; 1,542-patient real-world cohort (MD Anderson + Guardant Health + literature review) for clinical outcomes |
| Intervention / exposure / comparator | Second- vs. first- or third-generation EGFR TKIs, in single vs. compound PACC mutations |
| Outcomes / endpoints | Mutation co-occurrence patterns; in vitro drug sensitivity; real-world clinical outcomes by TKI generation |
| Sample size | 15,851 (genomic landscape); 1,542 (clinical outcomes cohort) |
| Key findings | PACC mutations found in 9% of samples (1,421/15,851), predominantly as in-cis compound mutations (66.2%, 941/1,421) — contrasts with classical mutations (84.3% single) and exon 20 insertions (88.6% single) (p<0.0001). In vitro: compound PACC mutations show sensitivity similar to single PACC mutations, with enhanced sensitivity to 2nd- vs. 1st-/3rd-generation TKIs. Retrospective clinical data corroborated improved outcomes with 2nd-generation TKIs for single or compound PACC mutations vs. 1st-/3rd-generation. |
| Quality / limitations | Very large sample for the genomic characterization (strong internal validity for mutation co-occurrence claim); retrospective clinical cohort subject to confounding by indication; in vitro sensitivity data supports but does not itself establish clinical efficacy — the paired real-world corroboration strengthens the claim but is not randomized evidence |
| Notes on conflict with other studies | Corroborates Nagano et al. 2026's subtype-dependent signal (afatinib/2nd-gen favored for compound mutations); the two should be read together as convergent evidence from different designs, not merged into a single effect estimate |
| Exclusion reason (if excluded instead) | N/A — included |

### Passiglia et al., 2026 — Amivantamab in EGFR exon 20 insertion NSCLC (ATLAS Italian registry)

| Field | Value |
|---|---|
| Source record | `sources/records/2026-passiglia-amivantamab-exon20-atlas-registry.md` |
| Study design | Multicenter, retrospective, observational registry study (ATLAS Italian registry, Jan–Dec 2024 enrollment window) |
| Population / system / sample | Advanced NSCLC, EGFR exon 20 insertion (ex20ins); 76/119 (63.9%) received 1L platinum-based chemo ± IO; 64/119 later received single-agent amivantamab |
| Intervention / exposure / comparator | Amivantamab (subsequent-line, real-world use); no randomized comparator |
| Outcomes / endpoints | Objective response rate (ORR), disease control rate (DCR), progression-free survival (PFS), overall survival (OS), treatment-related adverse events (TRAEs), intracranial response (23 patients with brain mets) |
| Sample size | 119 (64 treated with amivantamab) |
| Key findings | Under amivantamab: ORR 37.5%, DCR 66.2%, median PFS 9.6 months, median OS 16.9 months. TRAEs any-grade 68.8%, grade 3–4 10.9% (skin rash 56%/G3 9.4%, asthenia 9%, peripheral edema 8%, infusion reactions 9.4%/G3 1.5%). Among 23 patients with brain metastases: 13% intracranial partial response, 43.5% intracranial stable disease, intracranial mPFS 11.6 months. Authors describe this as consistent with the CHRYSALIS trial's efficacy/safety profile in a heavily pretreated real-world population. |
| Quality / limitations | Retrospective registry, no control arm — real-world confirmatory data rather than comparative-efficacy evidence; heavily pretreated population may differ from trial populations; single-country (Italy) registry limits generalizability to other health systems; moderate sample size (n=64 on amivantamab) for precise PFS/OS estimates |
| Notes on conflict with other studies | Complements Ou 2023, Kwon 2022, and Kim 2026 (all exon 20 insertion) but different drugs/settings/outcome domains — do not pool numerically across these studies as if one cohort; Passiglia's real-world ORR (37.5%) for amivantamab is markedly higher than the pooled real-world ORR for non-exon-20-targeting agents reported in Kwon 2022's meta-analysis, consistent with amivantamab's exon-20-specific mechanism of action |
| Exclusion reason (if excluded instead) | N/A — included |

### Ou et al., 2023 — Real-world response and outcomes in EGFR exon 20 insertion NSCLC by treatment line

| Field | Value |
|---|---|
| Source record | `sources/records/2023-ou-real-world-exon20-outcomes.md` |
| Study design | Retrospective real-world cohort using the Flatiron Health electronic health record database (US), three cohorts by treatment line |
| Population / system / sample | 237 NSCLC patients with EGFR exon 20 insertions, diagnosed Jan 2011–Feb 2020; 129 in first-line (1L) cohort, 114 in ≥2L cohort |
| Intervention / exposure / comparator | Real-world treatment patterns by line: 1L platinum+non-platinum chemo (31.0%) and EGFR-TKIs (28.7%) most common; ≥2L immuno-oncology monotherapy (28.1%) and EGFR-TKIs (17.5%) most common. A ≥2L "postplatinum trial-aligned" subgroup approximates mobocertinib-trial (NCT02716116) eligibility. |
| Outcomes / endpoints | Confirmed ORR, median OS, median PFS, by treatment-line cohort |
| Sample size | 237 total (1L n=129, ≥2L n=114) |
| Key findings | Confirmed ORR: 18.6% (1L), 9.6% (≥2L), 14.0% (≥2L postplatinum trial-aligned). Median OS: 17.0, 13.6, 11.5 months respectively. Median PFS: 5.2, 3.7, 3.3 months respectively. Authors conclude outcomes are poor across lines, underscoring unmet need for exon-20-targeted therapy. |
| Quality / limitations | Retrospective EHR-based real-world design, no randomization, treatment assignment reflects routine practice (confounding by indication); large real-world sample for a rare subtype is a strength; conducted before amivantamab/mobocertinib were widely used, so may understate outcomes achievable with current exon-20-targeted agents (contrast with the more recent Passiglia 2026 and Kim 2026 data below) |
| Notes on conflict with other studies | Predates targeted-therapy-era data (Passiglia 2026, Kim 2026); its poor pre-targeted-therapy outcomes provide useful historical baseline/contrast rather than conflicting evidence — research-writer should frame these as sequential rather than contradictory |
| Exclusion reason (if excluded instead) | N/A — included |

### Kwon et al., 2022 — Systematic review and meta-analysis of EGFR exon 20 insertion NSCLC outcomes

| Field | Value |
|---|---|
| Source record | `sources/records/2022-kwon-exon20-meta-analysis.md` |
| Study design | Systematic literature review (23 real-world evidence [RWE] studies + 19 interventional studies) with meta-analysis of pooled RWE outcomes by line of therapy |
| Population / system / sample | NSCLC, EGFR exon 20 insertion mutation-positive, across pooled RWE and interventional studies |
| Intervention / exposure / comparator | 1L chemotherapy, EGFR-TKIs, and IO agents; ≥2L chemotherapy, EGFR-TKIs, and IO agents; interventional agents: mobocertinib, poziotinib, osimertinib, afatinib, CLN-081, DZD9008 (TKIs), amivantamab (mAb), luminespib (HSP90i) |
| Outcomes / endpoints | Pooled ORR, PFS, OS by line and treatment class |
| Sample size | Aggregate across 23 RWE + 19 interventional studies (patient-level N not stated in abstract) |
| Key findings | 1L chemotherapy: pooled ORR 25.7%, PFS 5.6 mo, OS 18.3 mo. ≥2L: ORR 5.0% (EGFR-TKI), 3.3% (IO), 13.9% (chemo); PFS 2.1, 2.3, 4.4 mo respectively; OS 14.1, 8.8, 17.1 mo (chemo OS not itself pooled). Conclusion: non-exon-20-targeting EGFR-TKIs and IO agents underperform chemotherapy in this population; limited RWE existed (at time of review) for mobocertinib/amivantamab specifically, though interventional evidence supported their potential. |
| Quality / limitations | As a meta-analysis/synthesis, this is not an independent new patient cohort — should not be double-counted as additional confirmatory N alongside the primary studies it may include; predates (2022) most other included primary studies (2023–2026) and predates wide real-world uptake of amivantamab/mobocertinib, so its targeted-therapy conclusions are the most dated in this table |
| Notes on conflict with other studies | Its finding that chemotherapy outperforms non-exon-20-targeting TKIs/IO is consistent with — and helps explain — Ou 2023's poor outcomes in an era before exon-20-targeted agents were standard; its caution about limited RWE for amivantamab/mobocertinib is directly updated by the newer Passiglia 2026 and Kim 2026 data in this table |
| Exclusion reason (if excluded instead) | N/A — included |

### Yu et al., 2026 — Genomic profiling after progression on first-line osimertinib (ORCHARD, phase II)

| Field | Value |
|---|---|
| Source record | `sources/records/2026-yu-orchard-resistance-mechanisms.md` |
| Study design | Phase II, biomarker-directed clinical trial (NCT03944772); prespecified exploratory baseline tissue (n=400) and plasma (n=191) NGS analysis |
| Population / system / sample | EGFR-mutation-positive NSCLC progressing on first-line osimertinib |
| Intervention / exposure / comparator | Molecular-profile-directed second-line allocation into 3 groups (trial design); this analysis focuses on baseline resistance-mechanism genomics rather than treatment comparison |
| Outcomes / endpoints | Resistance-alteration frequency/type (tissue+plasma NGS); tissue-plasma concordance; co-occurring-mutation patterns by baseline EGFR subtype |
| Sample size | Tissue n=400, plasma n=191 |
| Key findings | TP53 and MDM2/4 alterations mutually exclusive, present in 86% of tumors. Combined tissue+plasma: resistance alterations detected in 87% of samples, with multiple concurrent resistance alterations in 46%. PI3K-pathway, SOX2, and MYC alterations frequent in histologically transformed tumors. **Differential co-occurring-mutation patterns observed between L858R and exon 19 deletion tumors** — i.e., resistance-mechanism patterns are reported by baseline EGFR subtype, satisfying this project's subtype-level inclusion requirement. |
| Quality / limitations | Large, well-characterized trial cohort (n=400 tissue) is a strength; this is an exploratory, hypothesis-generating genomic analysis nested in a clinical trial, not a comparative-efficacy result; L858R-vs-exon19del comparison is a secondary/qualitative observation in the abstract, not accompanied by effect sizes here |
| Notes on conflict with other studies | Complements Gariazzo 2026 (also post-osimertinib resistance, but restricted to a real-world Italian common-mutation cohort with MET-amplification focus) — ORCHARD's broader resistance-landscape data (TP53/MDM2/4, PI3K, SOX2, MYC) and Gariazzo's MET-amplification finding both describe pieces of the same heterogeneous-resistance picture; present as complementary, not overlapping/redundant, findings |
| Exclusion reason (if excluded instead) | N/A — included. **Reversed from evidence-reviewer's initial exclusion**: full abstract confirms subtype-stratified (L858R vs. exon 19del) reporting, resolving the ambiguity flagged in that pass. |

### Gariazzo et al., 2026 — "Rebiopsy on Osi": EGFR-mutant NSCLC progressing on first-line osimertinib

| Field | Value |
|---|---|
| Source record | `sources/records/2026-gariazzo-rebiopsy-on-osi.md` |
| Study design | Multicenter, retrospective, real-world observational cohort (Italian ATLAS registry) |
| Population / system / sample | Advanced NSCLC, common EGFR mutation only (exon 19 deletion or L858R), progressed on 1L osimertinib |
| Intervention / exposure / comparator | Rebiopsy (tissue and/or liquid biopsy) vs. no rebiopsy; biomarker-driven adaptive 2L therapy vs. non-adaptive 2L therapy vs. no rebiopsy |
| Outcomes / endpoints | Rebiopsy rate, resistance-mechanism detection rate, 2L PFS and OS by rebiopsy/treatment-adaptation status |
| Sample size | 457 patients (206 rebiopsied; 239 received 2L therapy, 39 of those adaptive) |
| Key findings | Rebiopsy performed in 45.1% (206/457), mostly tissue (66.2%). Resistance mechanism identified in 38.8% (80/206) overall — higher detection with tissue (46.6%) than liquid biopsy (13.5%). MET amplification/overexpression was the most frequent actionable mechanism; 29/39 (74.3%) of adaptively treated patients with MET amplification/overexpression received a MET-TKI-based regimen. Median PFS/OS: 7.3/14.1 months (adaptive therapy) vs. 6.5/12.2 months (rebiopsy, no adaptation) vs. 5.1/8.2 months (no rebiopsy). |
| Quality / limitations | Retrospective, non-randomized allocation to rebiopsy/adaptive therapy (likely confounded by performance status/disease burden — patients well enough for rebiopsy and adaptive therapy may simply have better prognosis independent of the intervention); large sample (n=457) supports reasonable precision within the common-mutation population; restricted to common mutations only — does not address uncommon/compound subtypes |
| Notes on conflict with other studies | Complements Yu et al. 2026 (ORCHARD) — see that row; MET-amplification finding here is consistent with MET pathway alterations being a recognized osimertinib-resistance mechanism generally, though ORCHARD's abstract emphasizes TP53/MDM2/4/PI3K/SOX2/MYC rather than MET specifically, so the two studies highlight different (not necessarily conflicting) parts of a heterogeneous resistance landscape |
| Exclusion reason (if excluded instead) | N/A — included |

### Yang et al., 2024 — PD-L1/immune profiling and osimertinib efficacy in EGFR T790M-mutant NSCLC

| Field | Value |
|---|---|
| Source record | `sources/records/2024-yang-pdl1-t790m-osimertinib.md` |
| Study design | Translational cohort study with in vitro/in vivo (xenograft) correlative experiments |
| Population / system / sample | Pre-treated EGFR T790M+ NSCLC, by initial EGFR mutation subtype: 72 exon 19 deletion, 58 L858R, 4 G719X |
| Intervention / exposure / comparator | Osimertinib treatment; comparator is PD-L1-positive (TC≥1%) vs. PD-L1-negative status |
| Outcomes / endpoints | PFS by PD-L1 status; immune-cell infiltration; in vitro/xenograft osimertinib sensitivity with PD-L1 overexpression |
| Sample size | 134 (72 del19, 58 L858R, 4 G719X); 21/134 (15.7%) PD-L1-positive |
| Key findings | No significant PFS difference by PD-L1 status (Kaplan-Meier). PD-L1 expression did not differ by initial EGFR mutation subgroup or biopsy site. Multivariate Cox: older age and L858R mutation independently associated with outcome (direction/magnitude not stated in abstract). PD-L1 overexpression did not confer osimertinib resistance in vitro or in xenografts. Conclusion: PD-L1/immune profiling is not predictive of osimertinib efficacy in T790M+ disease. |
| Quality / limitations | G719X subgroup (n=4) is too small for any standalone subtype conclusion — exploratory only; single-cohort translational design with correlative lab experiments is a strength for mechanistic plausibility but the clinical PFS analysis is retrospective/observational; L858R identified as an independent predictive factor in multivariate analysis but the abstract does not report the effect direction/size, limiting how this can be reported |
| Notes on conflict with other studies | Distinct outcome domain (biomarker prediction) from most other included studies; no direct conflict identified |
| Exclusion reason (if excluded instead) | N/A — included |

### Kim et al., 2026 — Paired ctDNA analysis of resistance mechanisms to mobocertinib in EGFR exon 20 insertion NSCLC

| Field | Value |
|---|---|
| Source record | `sources/records/2026-kim-mobocertinib-ctdna-resistance-exon20.md` |
| Study design | Single-center, prospective observational cohort |
| Population / system / sample | EGFR exon 20 insertion-positive NSCLC treated with mobocertinib; 14/22 previously received amivantamab |
| Intervention / exposure / comparator | Mobocertinib; paired pre-/post-treatment ctDNA sequencing; sub-analysis by prior amivantamab exposure and by insertion site (helical vs. non-helical region) |
| Outcomes / endpoints | ORR, DCR, PFS (RECIST v1.1); acquired resistance mechanisms via ctDNA |
| Sample size | 22 (14 with prior amivantamab exposure) |
| Key findings | ORR 59%, DCR 82%, median PFS 5.6 months (95% CI 3.5–9.3) overall. Amivantamab-pretreated subgroup (n=14): ORR 57.1%, median duration of response 5.1 months, median PFS 5.8 months. Helical-region insertions associated with better response than non-helical. Baseline ctDNA-negative status associated with favorable outcomes. Resistance mechanisms were diverse: EGFR amplification, RTK/RAS pathway alterations, and rarer events (gene fusion, small-cell transformation). |
| Quality / limitations | Small sample (n=22, subgroup n=14) substantially limits precision of all point estimates (note the wide 95% CI on PFS) and generalizability; single-center design; prospective design and paired ctDNA sampling are genuine strengths specifically for characterizing resistance-mechanism diversity |
| Notes on conflict with other studies | Mobocertinib's 59% ORR here is markedly higher than the pooled non-exon-20-targeted-TKI ORR in Kwon 2022's meta-analysis (5.0% ≥2L) and higher than amivantamab's real-world 37.5% ORR in Passiglia 2026 — but Kim's n=22 single-center result and Passiglia's n=64 real-world result are not designed for head-to-head comparison (different populations, lines of therapy, and settings); research-writer should not present this as mobocertinib "beating" amivantamab |
| Exclusion reason (if excluded instead) | N/A — included |

---

## Excluded candidates (at intake, by literature-scout / evidence-reviewer)

| Study | PMID | Exclusion reason |
|---|---|---|
| Compound-mutation case report (V774M/S768I) | — | Case report; other multicenter/large-cohort evidence on compound mutations already included (Liu 2026) — exclusion criterion for case reports applies |
| Assessing time to symptomatic progression, MARIPOSA study | 42492306 | Phase III RCT but endpoint analysis reported at the pooled EGFR-mutant level in the record reviewed, not broken out by mutation subtype — exclusion criterion: "not reporting subtype-level (only pooled 'EGFR-mutant') data" |
| VEGFA/VEGFR2 signaling and EGFR-TKI outcomes | 42231027 | Stratifies by VEGFA/VEGFR2 expression, not by EGFR mutation subtype — outcome variable of interest (subtype) not the study's stratification axis |
| LAURA study safety analysis (osimertinib after CRT, stage III) | 42296617 | Safety data reported at the pooled EGFR-mutated level, not stratified by mutation subtype |

---

## Summary

- **9 studies included**, all `Verified` source records, all peer-reviewed, 2022–2026.
- **4 candidates excluded at intake** (1 case report, 3 pooled/non-subtype-stratified).
- Evidence spans three research-question subtopics: (1) uncommon/compound-mutation treatment response and TKI-generation choice — Nagano 2026, Liu 2026; (2) exon 20 insertion treatment outcomes — Ou 2023, Kwon 2022, Passiglia 2026, Kim 2026; (3) acquired resistance mechanisms — Yu 2026 (ORCHARD), Gariazzo 2026, plus the T790M/biomarker angle in Yang 2024.
- No included study is a randomized head-to-head trial directly comparing EGFR-TKIs by mutation subtype as its primary design (Nagano 2026 is the closest, and is retrospective/IPTW-adjusted, not randomized) — this is a body-of-evidence limitation to carry into the report.
