# EGFR Mutation Subtypes and Treatment Response, Resistance, and Clinical Outcomes in NSCLC (2022–2026): An Evidence Synthesis

## Research question and scope

**Question:** What are the most recent peer-reviewed studies (2022–2026)
evaluating EGFR mutation subtypes and their association with treatment
response, acquired resistance, and clinical outcomes in patients with
non-small cell lung cancer (NSCLC)?

**Population:** Adult NSCLC patients harboring EGFR mutations, spanning
common subtypes (exon 19 deletion, L858R) and uncommon/rarer subtypes
(exon 20 insertion, G719X, L861Q, S768I, compound mutations).

**Intervention/exposure:** EGFR mutation subtype as a variable, generally
in the context of EGFR tyrosine kinase inhibitor (TKI) therapy
(osimertinib and other generations) or EGFR-directed antibody/ctDNA-guided
therapy.

**Comparator:** Other EGFR mutation subtypes, or wild-type EGFR, where
reported.

**Outcomes:** Treatment response (ORR, PFS, OS), acquired resistance
mechanisms, and clinical outcomes stratified by mutation subtype.

**Study types considered:** Clinical cohort studies, clinical trials
(including trial-embedded biomarker analyses), retrospective/prospective
real-world analyses, and systematic reviews/meta-analyses; mechanistic
studies included only where tied to clinical outcome data.

**Date range / language:** 2022–2026; English.

**Key inclusion criteria:** peer-reviewed (not preprint-only); human NSCLC
with molecularly confirmed EGFR mutation status; outcome data reported
*stratified by EGFR mutation subtype* (not only pooled "EGFR-mutant").

**Key exclusion criteria:** non-NSCLC or purely preclinical studies without
clinical correlate; single-patient case reports (unless no other evidence
exists for a rare subtype); studies reporting only pooled EGFR-mutant data
without subtype breakdown; preprints/conference abstracts without full
text.

## Methods summary

Literature was identified through structured, date-filtered
(2022–2026) `PubMed` searches (via `mcp__PubMed__search_articles`) across
four targeted query passes: (1) general EGFR-subtype/treatment-response,
(2) exon 20 insertion outcomes, (3) acquired-resistance mechanisms after
osimertinib, and (4) compound/PACC mutations. Two earlier candidates
originally surfaced through unstructured web search could not be verified
at that time (network egress to primary bibliographic sources was
blocked) and were re-run and independently confirmed once PubMed MCP
tools became available; a small set of exploratory web-search-only
candidates from that early pass were not re-verified and were not carried
forward. Every candidate ultimately included was verified against
PubMed's own metadata record (`mcp__PubMed__get_article_metadata`) for
title, full author list, journal, year, volume/issue/pages, DOI, and
PMCID — not a search snippet or AI-generated summary.

Fifteen unique candidates were evaluated in total. Four were excluded at
intake: one single-patient case report on a compound mutation (other
multicenter evidence on compound mutations was already available), and
three studies (a MARIPOSA time-to-symptomatic-progression analysis, a
VEGFA/VEGFR2-signaling study, and a LAURA safety analysis) that reported
outcomes only at the pooled EGFR-mutant level without subtype
stratification, failing the study's core inclusion criterion. Nine
candidates passed forward, all verified directly against PubMed, all
peer-reviewed, spanning 2022–2026; these were extracted into
`outputs/evidence-table.md` and form the entire evidentiary basis for
this report.

## Evidence synthesis

### 1. Uncommon and compound EGFR mutations: treatment response and TKI-generation choice

Two studies address this subtopic, using different designs and
overlapping but non-identical populations.

Nagano et al. (2026) conducted a multicenter, retrospective, real-world
cohort (29 Japanese hospitals, IPTW-adjusted, non-randomized) comparing
first-line afatinib (n=95) versus osimertinib (n=67) in advanced/recurrent
non-squamous NSCLC with uncommon EGFR mutations, explicitly excluding
exon 20 insertions and de novo T790M. Overall, there was no statistically
significant difference between afatinib and osimertinib in time to
treatment failure (HR 1.04, 95% CI 0.61–1.77) or overall survival (HR
1.34, 95% CI 0.73–2.44); afatinib was associated with higher response
rates but more dose-reduction-requiring adverse events. A subtype-dependent
signal was observed in post hoc subgroup analysis: osimertinib appeared
favored for L861X mutations, while afatinib appeared favored for compound
mutations (Nagano et al., 2026).

Liu et al. (2026) characterized PACC (uncommon/atypical) and compound
EGFR mutations across a very large cell-free-DNA cohort (15,851
EGFR-mutant NSCLC samples), finding PACC mutations in 9% of samples
(1,421/15,851), predominantly occurring as in-cis compound mutations
(66.2%) — a markedly different co-occurrence pattern than classical
mutations (84.3% single) or exon 20 insertions (88.6% single) (p<0.0001).
In parallel Ba/F3 in vitro drug-sensitivity assays, compound PACC
mutations showed sensitivity similar to single PACC mutations, with
enhanced sensitivity to second-generation versus first- or
third-generation TKIs. This in vitro finding was corroborated in a
separate 1,542-patient real-world clinical cohort, in which
second-generation TKIs were associated with improved outcomes relative to
first- or third-generation TKIs for both single and compound PACC
mutations (Liu et al., 2026).

**Interpretation:** Taken together, these two studies — despite differing
substantially in design (retrospective clinical cohort vs.
genomic/in-vitro/real-world composite) and in exact population definition
(Nagano's "uncommon mutations" excluding exon 20/de novo T790M, versus
Liu's "PACC/compound mutation" framework) — point in a broadly convergent
direction: second-generation (afatinib-class) TKIs may have a
subtype-specific advantage over third-generation osimertinib specifically
in compound-mutation disease, whereas single uncommon mutations (e.g.,
L861X) may respond preferentially to osimertinib. This is a directional
convergence across different evidence types, not a merged effect
estimate, and should not be read as replication of a single finding.

### 2. Exon 20 insertion NSCLC: treatment outcomes across eras and agents

Four studies address exon 20 insertion NSCLC, but at different points in
the treatment-era timeline and with non-overlapping drug/data sources —
they should be read as sequential snapshots, not a single pooled cohort.

Kwon et al. (2022), a systematic review and meta-analysis of 23 real-world
evidence studies and 19 interventional studies (published before
widespread real-world use of amivantamab/mobocertinib), found that in the
pre-targeted-therapy era, non-exon-20-targeting EGFR-TKIs and
immuno-oncology agents underperformed chemotherapy: first-line
chemotherapy pooled ORR was 25.7% (PFS 5.6 months, OS 18.3 months), while
second-line-or-later non-exon-20-targeted EGFR-TKIs and IO agents achieved
only 5.0% and 3.3% ORR respectively, versus 13.9% for chemotherapy in that
line. The review noted limited real-world evidence at that time for
mobocertinib and amivantamab specifically (Kwon et al., 2022).

Ou et al. (2023), using the Flatiron Health US real-world database
(n=237, diagnosed 2011–2020, predating wide targeted-therapy uptake),
similarly found poor outcomes across treatment lines: confirmed ORR 18.6%
(first-line), 9.6% (second-line-or-later), and 14.0% in a
postplatinum-trial-aligned subgroup approximating mobocertinib-trial
eligibility criteria; median OS was 17.0, 13.6, and 11.5 months
respectively (Ou et al., 2023). The authors concluded this underscored an
unmet need for exon-20-targeted therapy.

Against that historical baseline, two more recent studies report outcomes
with exon-20-targeted agents. Passiglia et al. (2026), a multicenter
Italian real-world registry (ATLAS) of 119 exon 20 insertion patients (64
treated with subsequent-line single-agent amivantamab), reported ORR
37.5%, disease control rate 66.2%, median PFS 9.6 months, and median OS
16.9 months under amivantamab, with any-grade treatment-related adverse
events in 68.8% (grade 3–4 in 10.9%); among 23 patients with brain
metastases, intracranial partial response was seen in 13% and intracranial
median PFS was 11.6 months. The authors described this real-world profile
as consistent with the pivotal CHRYSALIS trial (Passiglia et al., 2026).
Kim et al. (2026), a smaller single-center prospective cohort (n=22, 14
with prior amivantamab exposure) using paired ctDNA sequencing around
mobocertinib treatment, reported an overall ORR of 59%, disease control
rate 82%, and median PFS 5.6 months (95% CI 3.5–9.3); in the
amivantamab-pretreated subgroup (n=14), ORR was 57.1% and median PFS 5.8
months. Helical-region insertions were associated with better response
than non-helical insertions, and baseline ctDNA-negative status was
associated with more favorable outcomes; acquired resistance mechanisms
identified via paired ctDNA were diverse, including EGFR amplification,
RTK/RAS pathway alterations, and rarer events such as gene fusion and
small-cell transformation (Kim et al., 2026).

**Interpretation and explicit non-comparison:** The numerically higher
ORR for mobocertinib in Kim et al. (59%, n=22) compared with amivantamab
in Passiglia et al. (37.5%, n=64) and with pooled non-exon-20-targeted
agents in Kwon et al. (5.0% second-line-or-later) should **not** be read
as head-to-head evidence that mobocertinib outperforms amivantamab or
other agents. These studies differ in population (subgroup with/without
prior amivantamab exposure), treatment line, sample size, era, and
setting (single-center prospective vs. multicenter real-world registry vs.
meta-analytic synthesis), and none was designed for direct comparison.
What the body of evidence does support is a temporal contrast: outcomes
with exon-20-targeted agents (amivantamab, mobocertinib) reported in
2026 real-world/prospective cohorts appear more favorable than the
pooled/historical outcomes with non-exon-20-targeted therapies reported
by Kwon (2022) and Ou (2023) in an earlier treatment era — a sequential
comparison across time periods, not a controlled comparative-efficacy
finding.

### 3. Acquired resistance mechanisms after osimertinib

Two studies characterize resistance mechanisms following progression on
osimertinib; they address complementary, non-overlapping aspects of
resistance biology and should not be treated as replicating or
contradicting one another.

Yu et al. (2026), a prespecified exploratory genomic analysis nested in
the phase II ORCHARD trial (NCT03944772; baseline tissue n=400, plasma
n=191) in EGFR-mutant NSCLC progressing on first-line osimertinib, found
TP53 and MDM2/4 alterations to be mutually exclusive and present in 86% of
tumors; combining tissue and plasma NGS, resistance alterations were
detected in 87% of samples, with multiple concurrent resistance
alterations present in 46%. PI3K-pathway, SOX2, and MYC alterations were
frequent specifically in histologically transformed tumors. The analysis
also reported differential co-occurring-mutation patterns between
L858R and exon 19 deletion tumors, satisfying subtype-level reporting for
this arm of the research question, although this comparison is reported
qualitatively in the abstract without accompanying effect sizes (Yu et
al., 2026).

Gariazzo et al. (2026), a multicenter Italian real-world registry
("Rebiopsy on Osi," n=457) restricted to common EGFR mutations only
(exon 19 deletion or L858R) progressing on first-line osimertinib, found
that rebiopsy was performed in 45.1% of patients (mostly tissue, 66.2%),
with a resistance mechanism identified in 38.8% of rebiopsied patients —
detection was higher with tissue (46.6%) than liquid biopsy (13.5%). MET
amplification/overexpression was the most frequent actionable mechanism
identified, and 74.3% (29/39) of adaptively treated patients with this
alteration received a MET-TKI-based regimen. Median PFS/OS was longer
with biomarker-adaptive second-line therapy (7.3/14.1 months) than with
rebiopsy without adaptation (6.5/12.2 months) or no rebiopsy (5.1/8.2
months) (Gariazzo et al., 2026).

**Interpretation:** ORCHARD's genomic landscape (TP53/MDM2/4, PI3K, SOX2,
MYC alterations, tissue-plasma concordance) and Gariazzo's real-world
MET-amplification/adaptive-therapy findings describe different pieces of
a heterogeneous resistance landscape rather than the same finding from
two angles — one is a broad exploratory molecular-profiling analysis
within a trial population with mixed EGFR subtypes, the other is a
real-world clinical-outcomes study restricted to common-mutation disease
focused on one actionable mechanism (MET) and its treatment implications.
Gariazzo's outcome comparisons (adaptive vs. non-adaptive vs. no rebiopsy)
are also non-randomized: patients selected for rebiopsy and treatment
adaptation may simply have had better performance status or lower disease
burden independent of the intervention itself, so the observed PFS/OS
gradient should not be read as a proven causal benefit of the
biomarker-adaptive strategy.

### 4. T790M-mutant disease: PD-L1/immune biomarkers and subtype

Yang et al. (2024), a translational cohort study (n=134: 72 exon 19
deletion, 58 L858R, 4 G719X) of pretreated EGFR T790M-positive NSCLC
treated with osimertinib, found no significant difference in PFS by
PD-L1 status, and PD-L1 expression did not differ by initial EGFR mutation
subgroup or biopsy site. In multivariate Cox analysis, older age and
L858R mutation were independently associated with outcome, although the
abstract does not report the direction or magnitude of this association.
In vitro and xenograft experiments showed PD-L1 overexpression did not
confer osimertinib resistance. The authors concluded PD-L1/immune
profiling is not predictive of osimertinib efficacy in T790M-positive
disease (Yang et al., 2024). The G719X subgroup in this study (n=4) is
too small to support any standalone conclusion about that subtype and is
exploratory only.

## Quality and limitations

**No randomized, subtype-stratified comparative trial exists in this
evidence base.** Every included study is either retrospective/real-world
observational, a single-arm/prospective cohort, a trial-embedded
exploratory biomarker analysis, or a systematic review of such studies.
Nagano et al. (2026) is the closest to a controlled comparison
(IPTW-adjusted afatinib vs. osimertinib) but is non-randomized, and its
overall hazard ratios both cross 1 with wide confidence intervals — a
"no significant difference" here reflects limited power, not
demonstrated equivalence, and its subtype-specific findings (L861X vs.
compound mutations) are post hoc subgroup observations. This is a
body-of-evidence-level limitation that applies across the entire
synthesis: no study in this table can support a causal claim that a
given TKI generation is superior for a given subtype; all subtype-outcome
associations reported here are observational.

**Sample sizes vary by roughly four orders of magnitude across studies**,
and this must be weighed when judging precision and generalizability.
Liu et al. (2026)'s genomic-landscape characterization (n=15,851) offers
strong internal validity for mutation co-occurrence patterns, but its
clinical-outcomes claim rests on a smaller (n=1,542), retrospective,
confounded-by-indication subset. At the other extreme, Yang et al.
(2024)'s G719X subgroup (n=4) and Kim et al. (2026)'s overall cohort
(n=22, subgroup n=14) yield wide confidence intervals and limited
generalizability; Kim et al.'s PFS estimate (95% CI 3.5–9.3 months)
illustrates this directly. Mid-sized studies (Nagano, n=162; Ou, n=237;
Gariazzo, n=457; Passiglia, n=119/64) fall between these extremes and
should be weighted accordingly — none is large enough, on its own, to
resolve subtype-specific efficacy questions with high precision.

**Populations across the exon 20 insertion, uncommon, compound, and
T790M literatures are overlapping but non-identical and should not be
pooled.** Nagano (2026) explicitly excludes exon 20 insertions and de
novo T790M from its "uncommon mutation" population; Liu (2026) uses a
distinct PACC/compound-mutation framework; Ou (2023), Kwon (2022),
Passiglia (2026), and Kim (2026) are exon-20-insertion-specific but drawn
from different eras, agents, and health systems; Yang (2024) addresses
acquired T790M arising in previously common-mutation (or rare G719X)
disease. Numeric outcomes (e.g., ORR figures) from these different strata
are not directly comparable and have not been pooled in this synthesis.

**Confounding by indication is a recurring limitation** across nearly all
included retrospective/real-world studies (Nagano 2026, Liu 2026's
clinical cohort, Passiglia 2026, Ou 2023, Gariazzo 2026): treatment
selection reflected routine clinical practice rather than randomization,
so observed outcome differences may partly reflect why a given therapy
was chosen rather than the therapy's effect itself.

**Kwon et al. (2022) is a synthesis, not an independent patient cohort**
— its pooled estimates should not be treated as additional confirmatory
sample size alongside the primary studies it may itself include, and its
conclusions about non-exon-20-targeted agents underperforming chemotherapy
are the most dated in this table (predating widespread real-world use of
amivantamab and mobocertinib).

**Overall strength of evidence:** Moderate for descriptive
outcome/response rates within a given subtype and study; low for any
comparative or causal claim about relative TKI efficacy by subtype, given
the complete absence of randomized subtype-stratified trials in the
included literature.

## Gaps and uncertainty

- **No randomized controlled trial in this evidence base directly compares
  EGFR-TKIs (or other agents) by mutation subtype.** All subtype-outcome
  associations described above are drawn from observational or
  trial-embedded exploratory analyses; the research question as scoped
  cannot be answered with trial-level causal evidence from the current
  evidence table.
- **L858R vs. exon 19 deletion resistance-mechanism differences (Yu et
  al., 2026) are reported qualitatively without effect sizes** in the
  available abstract-level extraction; the magnitude and statistical
  robustness of this subtype difference cannot be characterized further
  from the evidence table as it stands.
- **The direction/magnitude of the L858R multivariate association with
  outcome in Yang et al. (2024)** is noted as significant in that study's
  multivariate model but is not reported in enough detail (abstract-level
  only) to state whether L858R was associated with better or worse
  outcome.
- **G719X-specific conclusions cannot be drawn:** the only G719X-specific
  data point in this evidence base is a subgroup of 4 patients within
  Yang et al. (2024), explicitly too small for standalone interpretation.
- **Rare uncommon subtypes (S768I as an isolated mutation, isolated
  L861Q) are not separately reported** in the included evidence beyond
  their inclusion within Nagano (2026)'s and Liu (2026)'s broader
  uncommon/PACC categories; subtype-specific outcome data for these
  individual rare alterations is a gap.
- **No included study reports long-term (beyond the endpoints stated)
  overall survival data specific to compound-mutation disease** beyond
  what is captured in Liu et al. (2026)'s real-world cohort description.
- **Pre-osimertinib-era vs. current-era comparisons for exon 20 insertion
  disease (Kwon 2022/Ou 2023 vs. Passiglia 2026/Kim 2026) are
  time-sequential, not controlled**, so the apparent improvement in
  outcomes with exon-20-targeted agents cannot be attributed with
  certainty to the agents themselves versus other changes in
  supportive care, staging, or patient selection over the intervening
  years.

## References

1. Nagano Y, Yokouchi H, Saito R, Honjo O, Sumi T, Kaburagi T, Ito K,
   Ikezawa Y, Yokoo K, Kikuchi H, Kudo S, Yamazoe M, Shigaki R, Tagami K,
   Tenma T, Ishikawa T, Takahashi M, Sasaki T, Asahina H, Hinotsu S,
   Chiba H, Oizumi S. Afatinib Versus Osimertinib for Non-Small Cell Lung
   Cancer With Uncommon EGFR Mutations: Real-World Outcomes. *Cancer
   Science*. 2026;117(8):2236-2246. DOI: 10.1111/cas.70400. PMID:
   42218657. https://pubmed.ncbi.nlm.nih.gov/42218657/

2. Liu X, Stamboulian M, Borgeaud M, Zhu E, Weipert C, Zhang N, Nilsson
   MB, Wang K, Hong L, Wang J, Morris BB, Heeke S, Robichaux JP, Lewis C,
   Drusbosky L, Chen H, Yang Y, He J, Cai L, Wu J, Zhang J, Alfredo A,
   Heymach JV, Le X. Compound EGFR Mutations Are Predominantly P-Loop and
   Alpha-C Helix Compressing Mutations With Increased Responsiveness to
   Second- Versus Third-Generation Tyrosine Kinase Inhibitors. *Journal of
   Thoracic Oncology*. 2026. DOI: 10.1016/j.jtho.2026.103948. PMID:
   42191070. https://pubmed.ncbi.nlm.nih.gov/42191070/

3. Passiglia F, Passaro A, Gariazzo E, Montrone M, Pasello G, Tiseo M,
   Russano M, Citarella F, Muscarella LA, Pozzessere D, Bria E, Roca E,
   Cerea G, Russo A, Grisanti S, Bulotta A, Veccia A, Biello F, Lo Russo
   G, Pilotto S, Genova C, Cortinovis D, Minuti G, Meoni G, Gori S, Reale
   ML, Pavan A, Ramundo M, Grossi F, Parra HS, Scotti V, Vavalà T, Sini C,
   Sergi C, Pelizzari G, Chiari R, Stanzione B, Favaretto A, Leone F,
   Bettini AC, Pagano M, Tondulli L, Toschi L, Lacidogna G, Bennati C,
   Catanese S, Malapelle U, Giannarelli D, Novello S. Amivantamab in
   advanced non-small cell lung cancer with epidermal growth factor
   receptor exon 20 insertion mutations: Real-world data from the Italian
   ATLAS Registry. *Cancer*. 2026;132(11):e70476. DOI: 10.1002/cncr.70476.
   PMID: 42216441. https://pubmed.ncbi.nlm.nih.gov/42216441/

4. Ou SI, Lin HM, Hong JL, Yin Y, Jin S, Lin J, Mehta M, Nguyen D, Neal
   JW. Real-World Response and Outcomes in Patients With NSCLC With EGFR
   Exon 20 Insertion Mutations. *JTO Clinical and Research Reports*.
   2023;4(10):100558. DOI: 10.1016/j.jtocrr.2023.100558. PMID: 37744306.
   https://pubmed.ncbi.nlm.nih.gov/37744306/

5. Kwon CS, Lin HM, Crossland V, Churchill EN, Curran E, Forsythe A,
   Tomaras D, Ou SI. Non-small cell lung cancer with EGFR exon 20
   insertion mutation: a systematic literature review and meta-analysis
   of patient outcomes. *Current Medical Research and Opinion*.
   2022;38(8):1341-1350. DOI: 10.1080/03007995.2022.2083326. PMID:
   35621011. https://pubmed.ncbi.nlm.nih.gov/35621011/

6. Yu HA, Tang KH, Markovets A, Hartmaier R, Smith PE, Cho BC, de Langen
   AJ, Goldberg SB, Goldman JW, Le X, Iwama E, Cosaert J, Riess JW,
   Piotrowska Z. Genomic Profiling of Epidermal Growth Factor Receptor
   Mutation-Positive Non-Small Cell Lung Cancer after Progression on
   First-line Osimertinib: Phase II ORCHARD Study. *Clinical Cancer
   Research*. 2026;32(17):3746-3756. DOI: 10.1158/1078-0432.CCR-25-4540.
   PMID: 41790029. https://pubmed.ncbi.nlm.nih.gov/41790029/

7. Gariazzo E, Colamartini F, Cantale O, Mogavero A, Vitale A, Romano L,
   Peroni M, Rijavec E, Banini M, Mazzoni S, Montrone M, Pasello G,
   Veccia A, Ogliari FR, Leo S, Cortinovis D, Delmonte A, Belluomini L,
   La Cava G, Meoni G, Sini C, Delcuratolo MD, Bettini A, Pagano M,
   Genova C, Russo A, Pelizzari G, Tondulli L, Sergi C, Roca E, Bennati
   C, Grisanti S, Stanzione B, Mariotti S, Vavalà T, Soto Parra H, Ortega
   C, Pignataro D, Lacidogna G, Pino MS, Chiari R, Calabrò L, Pozzessere
   D, Masini S, Gelibter A, Scotti V, Grossi F, Tiseo M, Bria E, Metro G.
   EGFR-mutant NSCLC progressing on first-line osimertinib: rebiopsy in
   real-world and impact of second-line therapies (the "Rebiopsy on Osi"
   study). *The Oncologist*. 2026;31(9). DOI: 10.1093/oncolo/oyag285.
   PMID: 42502985. https://pubmed.ncbi.nlm.nih.gov/42502985/

8. Yang CY, Liao WY, Ho CC, Chen KY, Tsai TH, Hsu CL, Su KY, Chang YL, Wu
   CT, Hsu CC, Liu YN, Peng GR, Kangartaputra AA, Yu SH, Liao BC, Hsu WH,
   Lee JH, Lin CC, Shih JY, Yang JCH, Yu CJ. PD-L1 expression and immune
   profiling cannot predict osimertinib efficacy in lung cancer with EGFR
   T790M mutation: A translational study. *Journal of the Formosan
   Medical Association*. 2024;125(2):155-163. DOI:
   10.1016/j.jfma.2024.12.020. PMID: 39694766.
   https://pubmed.ncbi.nlm.nih.gov/39694766/

9. Kim J, Park GH, Park S, Jung HA, Lee SH, Ahn JS, Ahn MJ, Sun JM.
   Paired ctDNA analysis reveals diverse resistance mechanisms to
   mobocertinib in EGFR exon 20 insertion NSCLC. *Frontiers in Oncology*.
   2026;16:1827867. DOI: 10.3389/fonc.2026.1827867. PMID: 42239888.
   https://pubmed.ncbi.nlm.nih.gov/42239888/
