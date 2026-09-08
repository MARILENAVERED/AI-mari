# EGFR Mutation Subtypes and Clinical Outcomes in NSCLC: A Synthesis of 2022–2026 Evidence

## Research question and scope

**Question.** What are the most recent peer-reviewed studies (2022–2026)
evaluating EGFR mutation subtypes and their association with treatment
response, acquired resistance, and clinical outcomes in patients with
non-small cell lung cancer (NSCLC)?

**Scope, as defined in `research-question.md`:**

- **Population:** Adult NSCLC patients with EGFR mutations — common
  (exon 19 deletion, L858R) and uncommon (exon 20 insertion, G719X, L861Q,
  S768I, compound mutations).
- **Intervention/exposure:** EGFR mutation subtype, generally in the
  context of EGFR tyrosine kinase inhibitor (TKI) therapy.
- **Comparator:** Other EGFR subtypes, or wild-type EGFR, where reported.
- **Outcomes:** Treatment response (ORR, PFS, OS), acquired resistance
  mechanisms, and subtype-associated clinical outcomes.
- **Study types:** Clinical studies (cohort, trial, retrospective/
  prospective) preferred; mechanistic/basic studies included only if tied
  to clinical outcome data.
- **Date range:** 2022–2026; English language; peer-reviewed only.

**Inclusion criteria:** peer-reviewed published studies; molecularly
confirmed EGFR mutation status in human NSCLC; treatment response,
resistance, or outcome data reported at the subtype level.

**Exclusion criteria:** non-NSCLC or purely preclinical (animal/in vitro)
studies without clinical correlate; single-patient case reports (unless no
other evidence exists for a rare subtype); studies reporting only pooled
"EGFR-mutant" data without subtype breakdown; preprints and conference
abstracts without full text.

**A note on study-type scope.** The written inclusion/exclusion criteria
do not explicitly state whether narrative review articles count as
in-scope "studies." Three of the eleven included records — Ferro et al.
2024 (PMID 38382773), Spitaleri et al. 2026 (PMID 41967619), and Zullo &
Remon 2026 (PMID 42512396) — are narrative reviews, not primary-data
studies. The evidence-reviewer flagged this as a judgment call for the
orchestrator/user to confirm. In this report, these three reviews are used
**only for background and conceptual framing** (epidemiology, treatment
landscape, resistance-mechanism classification) and are explicitly **not**
cited as primary evidence for any quantitative finding. This distinction
is maintained throughout by using them in the Methods/background framing
below and in scene-setting sentences in the synthesis, never as the sole
support for a number.

## Methods summary

Literature was identified by `literature-scout` via five PubMed searches
(`sources/search-log.md`, Runs 1–5, all conducted 2026-09-08), covering:
(1) EGFR subtype and treatment response generally, (2) EGFR exon 20
insertion outcomes, (3) uncommon point mutations (G719X, L861Q, S768I) with
osimertinib, (4) acquired resistance mechanisms by subtype, and (5)
compound EGFR mutations. Publication dates were restricted to
2022/01/01–2026/12/31 at the search stage; language and study-type
screening were applied at intake. Across all runs, 24 unique PMIDs were
verified against PubMed's authoritative metadata (`get_article_metadata`);
12 were passed forward to the evidence-reviewer as on-scope with
`Verified` or `Partial` bibliographic status, and 12 were excluded at
intake (case reports with duplicate coverage elsewhere, pooled/no-subtype
analyses, preclinical-only studies, off-scope focus, or out-of-date-range
publications), each with a documented reason in its source record.

Of the 12 candidates passed to the evidence-reviewer, 11 were included in
the evidence table and 1 was excluded at screening: Jing et al. (PMID
42453333), a review whose primary exposure is concurrent driver-gene
co-mutation status rather than EGFR-subtype-stratified outcomes, and whose
abstract does not report findings broken down by EGFR mutation subtype as
required by the inclusion criteria. No study reached a quality-appraisal
stage and was excluded for methodological reasons alone; all exclusions
were scope-based. All 11 included records carry a source-record
verification status of `Verified` (9 records) or `Partial` (2 records —
Shigematsu et al., PMID 41139406, and Zhou et al./WU-KONG28, PMID
42212913 — both flagged for an incomplete trailing author entry in the
underlying PubMed metadata itself, not a transcription error).

## Evidence synthesis

### Background and treatment landscape (review-derived context only)

EGFR-mutant NSCLC is treated with generations of EGFR-TKIs, with
osimertinib established as first-line standard of care for common
mutations; atypical/uncommon EGFR mutations (S768I, L861Q, G719X, and
others) are reported to account for roughly 12% of all EGFR alterations,
and afatinib is described as the only agent with regulatory approval
specifically for a subset of these atypical variants (S768I, L861Q,
G719X) as of 2018 (Spitaleri et al. 2026, PMID 41967619 — review). Beyond
this approved indication, treatment recommendations for the broader
spectrum of atypical mutations remain undefined in the literature, with
practice often extrapolated from classical-mutation data or defaulting to
chemotherapy (Spitaleri et al. 2026, PMID 41967619 — review). Separately,
resistance to first-line osimertinib is conceptually classified into
EGFR-dependent and EGFR-independent mechanisms, with heterogeneity in
duration of benefit and progression pattern proposed to relate to
mutation-subtype and co-occurring genetic alterations (Ferro et al. 2024,
PMID 38382773 — review). For EGFR exon 20 insertion NSCLC specifically,
the evolving therapeutic landscape — spanning chemotherapy,
immunotherapy, and newer targeted TKIs/antibody-based agents — is
described as addressing open challenges in treatment resistance,
molecular heterogeneity, and optimal sequencing (Zullo & Remon 2026, PMID
42512396 — review). These three reviews are cited here as background
framing only; the quantitative findings below come exclusively from the
eight primary-data studies in the evidence table.

### First-line treatment response in EGFR exon 20 insertion NSCLC

The strongest evidence in this set is a phase 3, international,
randomized controlled trial (WU-KONG28) comparing first-line sunvozertinib
to platinum-based chemotherapy in 324 treatment-naive patients with
EGFR exon 20 insertion NSCLC (Zhou et al. 2026, PMID 42212913). Sunvozertinib
produced longer median PFS (10.3 vs. 7.5 months; HR 0.65, 95% CI 0.50–0.85,
p<0.001), higher 12-month PFS (46.1% vs. 26.7%), higher ORR (58.9% vs.
31.1%), and longer median duration of response (11.2 vs. 7.1 months) than
chemotherapy, at the cost of a higher rate of grade ≥3 adverse events
(75.5% vs. 56.7%); overall survival data were immature (38.9% maturity) at
the time of reporting (PMID 42212913).

### Later-line treatment response in EGFR exon 20 insertion NSCLC

Two studies report outcomes for agents used after progression on prior
therapy, in more heavily pretreated exon 20 insertion populations. In the
Italian ATLAS real-world registry, 64 of 119 registered patients received
single-agent amivantamab in later lines (after prior chemotherapy ±
immunotherapy in most cases), with ORR 37.5%, disease control rate 66.2%,
median PFS 9.6 months, and median OS 16.9 months; among 23 patients with
brain metastases, 13% had partial intracranial response and intracranial
median PFS was 11.6 months (Passiglia et al. 2026, PMID 42216441). In a
single-center prospective cohort of 22 exon 20 insertion patients treated
with mobocertinib (14 with prior amivantamab exposure), ORR was 59%,
disease control rate 82%, and median PFS 5.6 months (95% CI 3.5–9.3); in
the amivantamab-pretreated subgroup, ORR was 57.1% with median PFS 5.8
months, and responses were better in helical-region insertions than other
insertion sites (Kim et al. 2026, PMID 42239888).

**Line-of-therapy caveat (explicit, per evidence-table notes):** the
WU-KONG28 sunvozertinib data (PMID 42212913) are first-line, whereas the
amivantamab (PMID 42216441) and mobocertinib (PMID 42239888) data are
later-line/post-progression in more heavily pretreated populations. The
numerically lower ORR for amivantamab (37.5%) relative to first-line
sunvozertinib (58.9%) reflects this population/line-of-therapy difference,
not a documented head-to-head efficacy comparison, and should not be read
as such. Mobocertinib's ORR (59%) in a later-line, ctDNA-selected cohort
is likewise not comparable to first-line sunvozertinib data without
accounting for this difference.

### Uncommon point mutations (G719X, L861Q, S768I) and TKI generation/choice

Two Japanese multicenter real-world retrospective cohorts address outcomes
in uncommon EGFR point mutations, from overlapping recruitment eras.
Shigematsu et al. (2025, PMID 41139406; n=35) found that later-generation
(2nd/3rd-gen) EGFR-TKI use was associated with significantly longer
overall survival than earlier-generation use (47.7 vs. 15.5 months,
p=0.0177), with non-use of later-generation TKI, liver metastases, and
poor performance status as independent poor prognostic factors on
multivariate analysis; afatinib showed favorable treatment duration
specifically in G719X and compound-mutation subtypes. Nagano et al. (2026,
PMID 42218657; n=162, afatinib 95 vs. osimertinib 67), using inverse
probability of treatment weighting, found no significant difference
between afatinib and osimertinib in time to treatment failure (HR 1.04,
95% CI 0.61–1.77) or overall survival (HR 1.34, 95% CI 0.73–2.44) overall,
though afatinib was associated with higher response rates and more
frequent dose-limiting adverse events; subgroup analysis suggested
osimertinib was favored for L861X mutations and afatinib for compound
mutations.

**Concordance and independence caveat:** both studies concordantly favor
afatinib for compound mutations. However, as noted in the evidence table,
these are both Japanese multicenter real-world cohorts of uncommon EGFR
mutations drawn from overlapping periods, and patient/hospital overlap
between the two cohorts cannot be ruled out from the available
information. They should therefore not be treated as two fully
independent confirmations of the afatinib-compound-mutation finding.
Additionally, Nagano et al.'s subtype-specific subgroup findings (L861X
favoring osimertinib, compound mutations favoring afatinib) are described
in the source abstract as "suggested," consistent with exploratory,
likely underpowered subgroup analysis rather than confirmatory evidence.

### Compound EGFR mutations

Lu et al. (2026, PMID 42320198), using a UC San Diego institutional cohort
plus the AACR GENIE database, found that L858R patients were more likely
than exon 19 deletion patients to have a de novo compound mutation (15%
vs. 2%, p<0.01), and that acquired C797S more often co-occurred with exon
19 deletion than L858R after osimertinib progression (20% vs. 7%, p<0.01).
In the GENIE cohort, 88% of S768I-mutated patients had an additional EGFR
co-mutation, most commonly G719X. Osimertinib time-to-treatment-failure
was markedly longer for the co-mutated G719X/L861Q compound genotype than
for G719X alone (median >13 vs. <7 months).

**Non-comparability caveat:** this osimertinib-based compound-mutation
finding (G719X/L861Q favoring longer TTF on osimertinib) is complementary
to, but not directly comparable with, Nagano et al.'s afatinib-based
finding that afatinib (not osimertinib) was favored for compound
mutations generally (PMID 42218657) — the two studies used different
index drugs, and per the evidence table's own guidance the findings should
be presented side by side rather than merged into a single conclusion
about "the best drug" for compound mutations.

### Acquired resistance mechanisms by subtype

Lin et al. (2025, PMID 41273219), in a retrospective genomic cohort of 37
patients on first-line afatinib (EGFR- and ERBB2-mutated combined),
reported that within the EGFR-mutated subgroup, primary resistance to
afatinib was associated with presence of an EGFR exon 20 insertion
mutation (p=0.011), while baseline exon 19 deletion, higher chromosomal
instability, and age-related mutational signatures were associated with
development of known acquired-resistance mechanisms (T790M, MET
amplification). Kim et al.'s paired ctDNA analysis of mobocertinib-treated
exon 20 insertion patients found diverse acquired resistance mechanisms —
EGFR amplification, RTK/RAS pathway alterations, and rarer events
including gene fusion and small-cell transformation — with baseline ctDNA
absence associated with more favorable outcomes (PMID 42239888). These two
findings are broadly consistent in characterizing exon 20 insertion as a
resistance-prone, mechanistically heterogeneous subtype, though they
examine resistance to different agents (afatinib vs. mobocertinib) and
are not a single unified resistance narrative.

**Disclosed conflict-of-interest note:** Lin et al. (PMID 41273219)
includes two co-authors affiliated with a commercial next-generation
sequencing vendor (Nanjing Geneseeq Technology) in a genomics-based
resistance-mechanism study; this potential conflict of interest is noted
in the evidence table and is disclosed here for transparency when
weighing this study's genomic findings.

### CNS disease and prognostic co-mutations in exon 20 insertion NSCLC

Reyes et al. (2026, PMID 42291370), in a retrospective cohort of 80
patients with EGFR exon 20 insertion NSCLC, found that 36.25% had CNS
progression and 7.5% had leptomeningeal disease. Median overall survival
did not differ significantly by CNS progression status (45.3 vs. 47.8
months; HR 1.21, 95% CI 0.66–2.23, p=0.54) or by TP53 co-mutation status
(31.6 vs. 47.8 months; HR 1.79, 95% CI 0.89–3.60, p=0.11).

**Interpretation caveat:** both hazard ratios are statistically
non-significant with wide confidence intervals spanning 1, indicating the
study is likely underpowered to detect the associations it examines. This
finding should be represented as suggestive/hypothesis-generating —
consistent with a possible OS disadvantage for CNS progression and TP53
co-mutation that the study could not confirm — not as evidence of "no
effect."

## Quality and limitations

**Overall strength of the body of evidence is mixed and uneven across
subtypes.** The strongest single piece of evidence is the WU-KONG28 phase
3 RCT (PMID 42212913), which provides high-internal-validity, randomized
first-line evidence for exon 20 insertion NSCLC, albeit industry-funded
(Dizal Pharmaceuticals) and with immature OS data. All other primary-data
studies are retrospective, real-world, or single-arm cohorts, several with
small sample sizes (n=22 to n=162), limiting statistical power —
especially for subtype-level subgroup analyses (e.g., Shigematsu et al.,
n=35; Kim et al., n=22; Lin et al., n=37 split across two molecular
subgroups).

**Independence concerns.** Two of the uncommon-mutation real-world cohorts
(Shigematsu et al., PMID 41139406, and Nagano et al., PMID 42218657) are
both Japanese multicenter studies from overlapping recruitment periods;
possible patient or hospital overlap cannot be excluded from the available
information, so their concordant finding on afatinib favoring compound
mutations should not be treated as two independent confirmations.

**Conflicting/non-comparable findings.** Nagano et al. (afatinib favored
for compound mutations) and Lu et al. (osimertinib favored for G719X/L861Q
compound mutations by TTF) address a similar question with different
index drugs and are not directly comparable; this report presents both
without resolving them into a single recommendation, since the evidence
table itself flags them as complementary rather than conflicting or
mergeable. Similarly, ORR/PFS figures for sunvozertinib (first-line),
amivantamab, and mobocertinib (both later-line) in exon 20 insertion NSCLC
must not be read as head-to-head comparisons given differing lines of
therapy and patient selection.

**Disclosed conflict of interest.** Lin et al. (PMID 41273219) has two
co-authors affiliated with a commercial NGS vendor in a study whose
central methodology is NGS-based genomic profiling; this is disclosed but
not resolved in the source abstract, and readers should weigh the
genomic-resistance findings from this study with that in mind.

**Underpowered/non-significant findings presented as suggestive.** Reyes
et al.'s CNS-progression and TP53 findings (PMID 42291370) and Nagano et
al.'s L861X/compound-mutation subgroup findings (PMID 42218657) are both
statistically non-significant or explicitly described as exploratory in
their source abstracts; they are presented in this report as
hypothesis-generating, not as established effects.

**Review-vs-primary-data distinction.** Three included records (PMID
38382773, 41967619, 42512396) are narrative reviews without new original
data extraction reported in their abstracts. They are used in this report
only for background/context (epidemiology, treatment-landscape framing,
conceptual resistance classification) and are not counted among the
primary quantitative evidence base described above.

## Gaps and uncertainty

- **No head-to-head randomized comparison exists across exon 20 insertion
  targeted agents** (sunvozertinib vs. amivantamab vs. mobocertinib) in
  this evidence base — cross-agent comparisons in the literature to date
  are confounded by line-of-therapy and population differences, and this
  evidence base cannot resolve which agent is preferable at a given line
  of therapy.
- **Compound-mutation treatment choice (afatinib vs. osimertinib) is not
  resolved by directly comparable data.** The two studies addressing this
  (Nagano et al., Lu et al.) used different index drugs and cannot be
  merged into a single recommendation; a study directly randomizing or
  matching compound-mutation patients across these two TKIs was not found
  in this evidence base.
- **CNS-progression and TP53-co-mutation prognostic effects in exon 20
  insertion NSCLC remain unconfirmed** — Reyes et al.'s findings are
  non-significant and likely underpowered; larger studies would be needed
  to confirm or refute these associations.
- **Possible non-independence of the two Japanese real-world
  uncommon-mutation cohorts** (Shigematsu et al., Nagano et al.) means
  their concordant afatinib-compound-mutation finding carries less
  independent-replication weight than it might appear at face value; this
  evidence base cannot determine the degree of cohort overlap from the
  information available.
- **Full-text-level subtype-specific quantitative detail from the three
  narrative reviews (Ferro et al., Spitaleri et al., Zullo & Remon) was
  not extracted** — only abstract-level synthesis was available to the
  evidence-reviewer for these records, so any more granular figures those
  reviews might contain (e.g., subtype-specific resistance rates cited
  from other primary literature within them) are not represented in this
  report.
- **Whether narrative reviews should count as in-scope "studies" under
  the research question's study-type criteria was not resolved** before
  this report was drafted; this report treats them as background-only,
  per the orchestrator's ruling communicated for this task, but the
  underlying ambiguity in `research-question.md` itself remains
  unresolved and is flagged again here.
- **No evidence in this set addresses treatment response/resistance for
  common EGFR mutations (exon 19 deletion, L858R) as directly as it does
  for uncommon/exon 20 insertion mutations**, aside from the compound-
  mutation and C797S-co-occurrence findings in Lu et al. — the evidence
  base is weighted toward uncommon and exon 20 insertion subtypes relative
  to the classical mutations named in the research question's population
  definition.

## References

1. Ferro A, Marinato GM, Mulargiu C, Marino M, Pasello G, Guarneri V,
   Bonanno L. The study of primary and acquired resistance to first-line
   osimertinib to improve the outcome of EGFR-mutated advanced Non-small
   cell lung cancer patients: the challenge is open for new therapeutic
   strategies. *Critical Reviews in Oncology/Hematology*. 2024;196:104295.
   PMID: 38382773. DOI: 10.1016/j.critrevonc.2024.104295.
   https://doi.org/10.1016/j.critrevonc.2024.104295 [Narrative review —
   used for background/context only, not cited as primary quantitative
   evidence.]

2. Shigematsu L, Tani T, Ikemura S, Ohgino K, Horiuchi K, Shinozaki T,
   Nukaga S, Terai H, Sato T, Naoki K, Sayama K, Oyamada Y, Sakamaki F,
   Soejima K, Yasuda H, Fukunaga K, et al. Clinical Outcomes of
   Later-Generation EGFR-TKIs for Uncommon EGFR Mutations in NSCLC: A
   Multicenter Real-World Study. *Thoracic Cancer*. 2025;16(20):e70179.
   PMID: 41139406. PMCID: PMC12554367. DOI: 10.1111/1759-7714.70179.
   https://doi.org/10.1111/1759-7714.70179

3. Lin F, Zhao M, Wu Q, Wu W, Wu X, Ma Y, Yin JC, Yang M, Gao M. Novel
   Resistance Mechanisms to Second-Generation EGFR Tyrosine Kinase
   Inhibitor Afatinib and Associations With Genomic Features in NSCLC.
   *Genes, Chromosomes & Cancer*. 2025;64(11):e70088. PMID: 41273219.
   PMCID: PMC12639536. DOI: 10.1002/gcc.70088.
   https://doi.org/10.1002/gcc.70088 [Note: two co-authors affiliated with
   a commercial NGS vendor, Nanjing Geneseeq Technology — disclosed
   potential conflict of interest.]

4. Spitaleri G, Trillo Aliaga P, Mariani GA, Attili I, Del Signore E,
   Corvaja C, Napoli VM, Cavallone M, Etessami JD, Zhan Y, Passaro A, de
   Marinis F. Epidermal growth factor receptor (EGFR) atypical mutations
   in non-small-cell lung cancer (NSCLC): 'Where the streets have no
   name'. *Critical Reviews in Oncology/Hematology*. 2026;223:105327.
   PMID: 41967619. DOI: 10.1016/j.critrevonc.2026.105327.
   https://doi.org/10.1016/j.critrevonc.2026.105327 [Narrative review —
   used for background/context only, not cited as primary quantitative
   evidence.]

5. Zhou C, Greillier L, Liu G, John T, Xing L, Kowalski D, Memmott RM,
   Yazici O, Sun M, Shu CA, Pons-Tostivint E, Fan Y, Fernandez-Hinojal G,
   Shum E, Wang M, Bertolini F, Camidge DR, Zhou C, Doucet L, Hong Q,
   Fang J, Huang D, Jin B, Yu Y, Antonuzzo L, Moro-Sibilot D, Bennouna J,
   de Castro G, Zheng L, Heymach JV, et al. First-Line Sunvozertinib in
   NSCLC with EGFR Exon 20 Insertion Mutations (WU-KONG28).
   *New England Journal of Medicine*. 2026;395(8):765-775.
   PMID: 42212913. DOI: 10.1056/NEJMoa2604461.
   https://doi.org/10.1056/NEJMoa2604461

6. Passiglia F, Passaro A, Gariazzo E, Montrone M, Pasello G, Tiseo M,
   Russano M, Citarella F, Muscarella LA, Pozzessere D, Bria E, Roca E,
   Cerea G, Russo A, Grisanti S, Bulotta A, Veccia A, Biello F, Lo Russo
   G, Pilotto S, Genova C, Cortinovis D, Minuti G, Meoni G, Gori S, Reale
   ML, Pavan A, Ramundo M, Grossi F, Parra HS, Scotti V, Vavalà T, Sini
   C, Sergi C, Pelizzari G, Chiari R, Stanzione B, Favaretto A, Leone F,
   Bettini AC, Pagano M, Tondulli L, Toschi L, Lacidogna G, Bennati C,
   Catanese S, Malapelle U, Giannarelli D, Novello S. Amivantamab in
   advanced non-small cell lung cancer with epidermal growth factor
   receptor exon 20 insertion mutations: Real-world data from the Italian
   ATLAS Registry. *Cancer*. 2026;132(11):e70476. PMID: 42216441.
   DOI: 10.1002/cncr.70476. https://doi.org/10.1002/cncr.70476

7. Nagano Y, Yokouchi H, Saito R, Honjo O, Sumi T, Kaburagi T, Ito K,
   Ikezawa Y, Yokoo K, Kikuchi H, Kudo S, Yamazoe M, Shigaki R, Tagami K,
   Tenma T, Ishikawa T, Takahashi M, Sasaki T, Asahina H, Hinotsu S, Chiba
   H, Oizumi S. Afatinib Versus Osimertinib for Non-Small Cell Lung Cancer
   With Uncommon EGFR Mutations: Real-World Outcomes. *Cancer Science*.
   2026;117(8):2236-2246. PMID: 42218657. PMCID: PMC13394325.
   DOI: 10.1111/cas.70400. https://doi.org/10.1111/cas.70400

8. Kim J, Park GH, Park S, Jung HA, Lee SH, Ahn JS, Ahn MJ, Sun JM.
   Paired ctDNA analysis reveals diverse resistance mechanisms to
   mobocertinib in EGFR exon 20 insertion NSCLC. *Frontiers in Oncology*.
   2026;16:1827867. PMID: 42239888. PMCID: PMC13225986.
   DOI: 10.3389/fonc.2026.1827867. https://doi.org/10.3389/fonc.2026.1827867

9. Reyes A, Mambetsariev I, Fricke J, Young JR, Chen BT, Amini A,
   Ladbury C, Arias-Romero J, Nguyen D, Pisick E, Doctor V, Tan B,
   Afkhami M, Kareem W, Li X, Salgia R. Patterns of central nervous
   system disease and molecular landscape in epidermal growth factor
   receptor exon 20 insertion mutated non-small cell carcinoma.
   *Translational Lung Cancer Research*. 2026;15(5):140. PMID: 42291370.
   PMCID: PMC13263828. DOI: 10.21037/tlcr-2026-1-0104.
   https://doi.org/10.21037/tlcr-2026-1-0104

10. Lu K, Patel SP, Azenkot T. Characteristics and Clinical Outcomes of De
    Novo and Acquired Uncommon Compound EGFR Mutations in Patients With
    Advanced Non-Small Cell Lung Cancer: A Brief Report. *Clinical Lung
    Cancer*. 2026;27(6):64-67. PMID: 42320198. DOI: 10.1016/j.cllc.2026.05.005.
    https://doi.org/10.1016/j.cllc.2026.05.005

11. Zullo L, Remon J. New Treatment Strategies for Rare Genomic
    Alterations: EGFR Exon 20 Insertions and HER2-Deregulated Lung Cancer.
    *Cancers (Basel)*. 2026;18(14). PMID: 42512396. PMCID: PMC13406144.
    DOI: 10.3390/cancers18142334. https://doi.org/10.3390/cancers18142334
    [Narrative review — used for background/context only, not cited as
    primary quantitative evidence; HER2-specific content excluded from
    this report as out of EGFR scope.]

### Excluded candidate (for transparency)

Jing R, Miao Y, Daut UN, How SH, Zhang F, Stanslas J. Exploring the
Impact of Multiple Gene Mutations on Epidermal Growth Factor Receptor
Tyrosine Kinase Inhibitor Response in Asian Nonsmall Cell Lung Cancer
Patients. *ACS Pharmacology & Translational Science*. 2026;9(7):1631-1651.
PMID: 42453333. Excluded at evidence-review screening: does not report
outcomes stratified by EGFR mutation subtype, per inclusion criteria.
