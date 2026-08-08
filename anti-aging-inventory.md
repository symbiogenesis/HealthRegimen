# Anti-Aging Therapeutic Inventory

**Target:** healthy male, age 39, US, currently on tirzepatide
**8 August 2026**
**Source:** AgingBiotech.info "Available Therapeutics" survey table (128 rows)
**Detail rows:** [therapeutics-by-mechanism.md](therapeutics-by-mechanism.md)

**How this document is arranged**

1. **Two files.** This one holds the framework, the grouped inventory, the interaction analysis and the two protocol write-ups; the row-level reasoning behind every score lives in [therapeutics-by-mechanism.md](therapeutics-by-mechanism.md).
2. **The inventory is grouped by mechanism, not by verdict.** Every way of hitting a given target sits side by side — all four PCSK9 modalities in one place, both SGLT2 inhibitors in one place, both AMPK activators in one place. A flat score-ordered list sits at the end of Part 2 for anyone who wants the whole thing in one column.
3. **Scoring is two axes multiplied** — evidence × benefit — with safety as a veto flag and effort as a tag outside the score. Part 1 sets out the model.
4. **Pro-growth and anti-growth are treated as a scheduling problem, not a permanent opposition.** Most of the conflict between the two arms is *simultaneity*, and separating them in time dissolves it. Part 3 distinguishes hard pharmacological conflicts from phase conflicts; Part 4 works through the block-cycling hypothesis directly, including what supports it, what it would cost, and how to run and measure it.

---

## Part 0 — The core problem with the source document

The source table is a good **survey**. It is not a **decision tool**, and it can't be turned into one by re-sorting the rows, because none of its scoring columns measure what you said you want to optimize.

### The four score columns don't measure benefit

| Column | What it actually measures | Why sorting by it misleads |
|---|---|---|
| **Gerotherapeutics score (of 12)**, Kulkarni '22 | Which FDA-approved drugs most *deserve a TAME-like trial* — weighted toward safety record, availability, target plausibility | A 12/12 means "we should test this," which is close to the opposite of "this is proven." SGLT2i scores 12; bisphosphonates score 11; rapamycin scores 9. |
| **# age-related pathologies (of 12)**, Khaltourina '20 | *Breadth* of disease categories with any signal | Rewards promiscuity over magnitude. Vitamin D scores 7+2; statins score 1+5. |
| **# fundamental aging pathways (of 11)**, *How Not To Age* | A book author's qualitative pathway assignment | Not a quantitative measure at all. Ornish gets 11/11 partly by aggregation. |
| **Rodent lifespan (+% max)** | Best result from *any* study, including uncontrolled ones | Cherry-picked maxima. MitoQ shows +93%, metformin +92% — neither replicates in ITP. |

### The rodent lifespan column is actively harmful to your ranking

The NIA Interventions Testing Program is the only rigorous arbiter here — three sites, genetically heterogeneous UM-HET3 mice, blinded, adequately powered. Its track record against the compounds on your list:

- **Failed to extend lifespan:** resveratrol, NR, fisetin (−5 to +7%), green tea extract, and eleven further compounds in the April 2026 report.
- **More damning:** that same 2026 report found that **astaxanthin, mitoglitazone, and meclizine — previous ITP *hits* — showed no benefit at different doses or later starting ages.** An ITP positive doesn't even reliably replicate against itself under protocol variation.
- **Nearly every recent hit is male-only:** epicatechin (+5%), halofuginone (+9%), mitoglitazone (+9%), canagliflozin (+14%), 17α-estradiol (+19%), astaxanthin (+12%). This one quirk happens to favor you, and is worth stating explicitly rather than leaving buried.

So: a column showing "+275 days (+93%)" for MitoQ, sitting next to a column showing ITP nulls, with no hierarchy between them, will systematically float weak interventions upward.

### The document is missing its own most important column

Your `best diagnostics/biomarkers` column is `?` or blank for roughly 70 of 128 rows. That is the actual finding. **You cannot rank therapies for one person without knowing that person's risk profile**, and for most of these rows nobody knows what would even indicate need. Any row with `?` in that column is, by its own admission, not rankable for an individual. That's a filter, not a gap.

### And it's missing the thing that will actually kill you

There is no row for blood pressure. No row for ApoB. No row for Lp(a). No row for cancer screening. No row for alcohol. No row for sleep apnea. No row for accidental injury — which, for a US male aged 35–44, is among the leading causes of death *right now*, ahead of cancer.

A 128-row inventory that includes Khavinson peptides and EDTA chelation but not blood pressure control has inverted its own priorities.

---

## Part 1 — The framework

### Rank by competing-risk arithmetic, not by hallmark coverage

For a US male currently 39, lifetime cause-of-death is dominated by atherosclerotic cardiovascular disease (roughly a quarter), then cancer (roughly a fifth), then dementia, metabolic disease, and — in the next decade specifically — unintentional injury. Nothing on the geroscience list moves those numbers as much as the boring interventions do.

The decisive asymmetry at your age is **exposure-time leverage**. Mendelian randomization on lifelong lower LDL-C gives roughly a 54% CHD risk reduction per 1 mmol/L, versus roughly 22% per 1 mmol/L for statins started in mid-life and followed for five years. Same molecule, same target — about **three times the effect** because the clock started earlier. Starting ApoB control at 39 rather than 55 is, on its own, plausibly worth more than every supplement in the source table combined.

The same logic runs the other way for the speculative agents: at 39 you have the *most* time for an unrecognized harm to compound. Risk tolerance should be lower now, not higher.

**Exposure-time leverage also cuts a third way.** If risk is an integral of exposure over time, then *duty cycle* is a lever, not just dose. An intervention run six weeks a year carries roughly a quarter of the cumulative exposure of the same intervention run continuously — for benefit and for harm alike. That observation is what makes Part 4 worth taking seriously rather than dismissing.

### The scoring model

Two questions, multiplied. Everything else is a flag, not a number.

**EVIDENCE (1–5) — how well established is this in humans like you?**

| | |
|---|---|
| **5** | Multiple RCTs, hard clinical outcomes, in populations that include healthy adults |
| **4** | RCTs with hard outcomes but in older or diseased populations; or one strong RCT plus concordant Mendelian randomization; or a surrogate endpoint whose causal link to outcomes is itself established by RCT and MR |
| **3** | RCTs with surrogate endpoints only (ApoB, BP, VO₂max, lean mass); or large consistent cohorts plus MR |
| **2** | Replicated animal lifespan data (ITP); or human observational only; or mechanism plus indirect human trial support |
| **1** | Mechanism, single-arm studies, case reports, unreplicated animal data |

**BENEFIT (1–5) — if the evidence is right, how much does it change *your* outcome at 39?**

| | |
|---|---|
| **5** | Moves a top-two lifetime cause of death; effect measured in years |
| **4** | Moves a top-five cause of death, or a large effect on a moderate one |
| **3** | Meaningful healthspan or function effect |
| **2** | Small or narrow effect |
| **1** | No plausible route to changing your outcomes at 39 |

**SCORE = EVIDENCE × BENEFIT**, integers 1–25.

**SAFETY is a flag, not a score:** `OK` · `MONITOR` (specific lab or symptom check, named in the row) · `AVOID` (serious harm plausible in your situation — overrides the score entirely).

**EFFORT is a tag, not a score:** `trivial` (<$100/yr and <5 min/wk) · `low` · `moderate` · `high` (>$2,000/yr or >4 h/wk).

The E4 tier covers the enlicitide case explicitly: a surrogate endpoint is not automatically E3 when the surrogate itself has been causally validated to the outcome by both RCT and Mendelian randomization. LDL-C lowering via the PCSK9 pathway is the clearest example in medicine of a surrogate that has earned that status.

### Why the model has this shape

**Evidence and benefit are separate factors, multiplied.** *Does this work* and *does it matter* are independent questions, and a single blended number hides which one you disagree about — a well-proven trivial intervention and an unproven important one would otherwise land on the same score for opposite reasons. Keeping them apart makes the disagreement legible: you can argue about the 3 and the 5 separately.

**Safety is a veto, not an averaged term.** Methylene blue carries a serotonin-syndrome interaction, but it's cheap and quick to take — average safety against cost and convenience and a hospitalization-grade risk turns into a respectable middling number. Safety doesn't average.

**Cost and time sit outside the score.** Across the whole inventory they would score 4 or 5 on nearly every row — near-constants, adding width without adding information — and they don't change whether something *works*, only whether it's worth the queue position. Hence a single `effort` tag. The clearest illustration is evolocumab, which scores a full 25 on the merits and is still gated behind a generic statin — not because the drug is worse, but because it's `high` effort and access-restricted, which is a scheduling fact rather than an efficacy one.

**No decimals.** 23.3 versus 20.0 would imply a precision that doesn't exist. Integer products in a 1–25 grid, with the reasoning for both factors written out per row so any item can be challenged on its inputs rather than its arithmetic.

---

## Part 2 — The inventory, grouped by mechanism

Grouped by **what the intervention acts on**, sorted by score within each family. Full reasoning for every score is in [therapeutics-by-mechanism.md](therapeutics-by-mechanism.md).

Why mechanism rather than verdict: grouping by verdict scatters the four PCSK9 inhibitors across three sections, which hides the fact that they share a target and differ only in how far each has been carried through outcomes trials — the exact place a grading error can go unnoticed. Grouping by target makes that class of error visible immediately, and it makes the actual decision — *which* member of a family, at which rung — the thing you are looking at.

`E` = evidence · `B` = benefit · **score = E × B** · safety flag overrides score.

### 2.0 Measurement and diagnostics — these gate everything below

| Score | E×B | Item | Safety | Effort | Note |
|---:|:---:|---|:---:|:---:|---|
| **25** | 5×5 | ApoB | ok | trivial | the input to the single best-evidenced intervention available to you |
| **20** | 5×4 | Home blood pressure series | ok | trivial | a test before it is a therapy; office readings are noise |
| **16** | 4×4 | DEXA body composition | ok | trivial | reference method for lean mass; also the instrument for evaluating Part 4 |
| **16** | 4×4 | Lp(a), once, lifetime | ok | trivial | each Lp(a) particle carries one apoB-100, so it sets a floor under achievable ApoB |
| **16** | 4×4 | Home sleep apnea test | ok | low | diagnostic accuracy solid; CPAP RCTs neutral for MACE, positive for symptoms and BP |
| **12** | 3×4 | VO₂max | ok | low | observational only — nobody randomises people to fitness |
| **6** | 3×2 | Vitamin D (25-OH) | ok | trivial | VITAL largely null; correcting frank deficiency has better support |
| **6** | 3×2 | hsCRP | ok | trivial | gates the residual-inflammation question |
| **6** | 3×2 | Baseline audiogram | ok | trivial | a baseline to detect drift against |
| **6** | 3×2 | Grip dynamometer | ok | trivial | cheapest weekly readout during any restriction phase |
| **6** | 3×2 | APOE genotype / CAD PRS | ok | low | **GINA covers health insurance but NOT life, disability or LTC** — insure first |
| **4** | 2×2 | Homocysteine, B12, folate | ok | trivial | only the correct readout if you pursue methionine work |
| **5** | 5×1 | Coronary artery calcium | ok | low | *defer to 45–50* — most 39-year-olds score zero and zero doesn't exclude soft plaque |

### 2.1 ApoB and the lipoprotein pathway

The highest-yield family on the list. Four molecular targets, one coherent ladder: **HMG-CoA reductase → NPC1L1 → PCSK9 → apo(a)**. ACL is a lateral move for statin intolerance, not a rung.

| Score | E×B | Item | Target | Safety | Effort |
|---:|:---:|---|---|:---:|:---:|
| **25** | 5×5 | ApoB to <60 mg/dL *(the target)* | — | monitor | trivial |
| **25** | 5×5 | Rosuvastatin / atorvastatin, generic | HMG-CoA reductase | monitor | trivial |
| **25** | 5×5 | Evolocumab / alirocumab | PCSK9 (mAb) | ok | high |
| **20** | 4×5 | Inclisiran | PCSK9 (siRNA) | ok | high |
| **20** | 4×5 | Enlicitide (Lipfendra), oral | PCSK9 (macrocyclic peptide) | ok | high |
| **16** | 4×4 | Ezetimibe, generic | NPC1L1 | ok | trivial |
| **16** | 4×4 | Bempedoic acid | ATP citrate lyase | monitor | moderate |
| **16** | 4×4 | ApoB to <30 mg/dL *(the increment)* | — | monitor | high |
| **8** | 2×4 | Lp(a) agents — pelacarsen, olpasiran, lepodisiran, muvalaplin | apo(a) | ok | high |
| **6** | 3×2 | Red yeast rice / monacolins | HMG-CoA reductase | **AVOID** | trivial |

**Within the PCSK9 subfamily**, all four agents block PCSK9-mediated LDL-receptor degradation. Same target, same downstream effect, four delivery routes. They separate on exactly one axis:

| Agent | Modality | Dosing | E×B | Outcomes trial |
|---|---|---|:---:|---|
| Evolocumab / alirocumab | monoclonal antibody | SC q2wk–q4wk | **25** | **Reported** — FOURIER, ODYSSEY |
| Inclisiran | siRNA | SC q6mo after loading | **20** | Pending — ORION-4, VICTORION-2P |
| Enlicitide | oral macrocyclic peptide | 20 mg daily | **20** | Pending — CORALreef Outcomes |

Two grading points are worth stating explicitly, because grouping is what makes them visible.

**Inclisiran sits at E4, not E5.** "FOURIER and ODYSSEY established hard-outcome benefit" is a statement about the monoclonals, not about inclisiran. Inclisiran was approved on LDL-C lowering alone and its outcomes trials have not reported. It belongs in the same evidence position as enlicitide.

**Enlicitide also sits at E4, one point below the monoclonals rather than two.** CORALreef Lipids gave 55.8% placebo-adjusted LDL-C reduction and ~50% ApoB reduction, and CORALreef AddOn beat ezetimibe, bempedoic acid and their combination on background statin. Those are surrogate endpoints — but PCSK9-mediated LDL lowering is a surrogate that has been causally validated to outcomes by both RCT and Mendelian randomization, with benefit tracking absolute LDL-C reduction largely independent of the mechanism used to achieve it. A two-point penalty would overstate the residual uncertainty for a same-target agent with an unusually strong class prior.

**On the effort tag:** the binding constraint for every member of this family is prior authorization and cash price, not administration. All four sit at `high` for that reason. But note the ranking that follows if you strip cost out: inclisiran is **two injections a year**, which is a lighter administration burden than a daily pill. The oral advantage over the monoclonals is real; the oral advantage over inclisiran is not.

**Sequence:** ApoB + Lp(a) → generic statin → add ezetimibe → reassess ApoB at 8 weeks → escalate within the PCSK9 family only if off target or Lp(a) is high. Generic rosuvastatin plus generic ezetimibe costs under $25/month and gets most people to target. Reaching for a $6,000/year drug before trying a $300/year one is the definition of a poor bang-for-buck decision.

**Where Lp(a) changes it:** if Lp(a) comes back >125 nmol/L, and especially >200, the case strengthens considerably, because statins slightly *raise* Lp(a) while PCSK9 inhibitors lower it ~20–25%. Lp(a)HORIZON (pelacarsen, n=8,323) is the first CV outcomes trial for any Lp(a)-lowering therapy and is expected to report before the end of 2026. **Measuring Lp(a) now costs $30 and tells you whether to care.**

### 2.2 Incretin and glucose handling

| Score | E×B | Item | Target | Safety | Effort |
|---:|:---:|---|---|:---:|:---:|
| **16** | 4×4 | Tirzepatide *(continue)* | GLP-1 / GIP receptor | monitor | moderate |
| **9** | 3×3 | Pasteurized *A. muciniphila* (MucT) *(watch)* | Amuc_1100 / gut barrier | ok | moderate |
| **4** | 2×2 | Pendulum Glucose Control (WBF-011) | live multi-strain / SCFA → endogenous GLP-1 | ok | moderate |
| **6** | 3×2 | Empagliflozin / canagliflozin | SGLT2 | monitor | low |

**The SGLT2 subfamily, in one place.** The source table ranked this #1 on a 12/12 gerotherapeutics score with the note "top scoring candidate for TAME-like trial." That note is doing more work than it appears: **the score means "most deserving of a trial," which entails that the human aging evidence does not yet exist.**

What the evidence supports is nonetheless the strongest non-tirzepatide case in this section. ITP canagliflozin gave **+14% median lifespan in males only**, no effect in females — the largest male effect in ITP history, concordant across all three test sites, with 90th-percentile survival up 9%. It happens to be your sex. On the human side the decisive detail is easy to miss: **DAPA-HF, DAPA-CKD and EMPA-KIDNEY enrolled non-diabetics, and the benefit held in that subgroup.** Whatever SGLT2 inhibition is doing, it is not simply lowering glucose in the hyperglycemic. Large cohorts add a consistent ~30% reduction in dementia incidence versus DPP-4 inhibitors, replicated across several meta-analyses — observational, confounded by indication, but pointing the same direction.

What still caps it at E3: every trial is in **type 2 diabetes, heart failure, or chronic kidney disease**, where a substantial part of the benefit is hemodynamic and renal, and none is in metabolically healthy adults.

B2 is the binding constraint, not E. You have no heart failure, no CKD, no diabetes, and ApoB is being handled by a statin. The population where this drug has proven itself is the population you are trying not to join, and the metabolic benefit you'd be reaching for is largely what tirzepatide is already delivering with hard-outcome data behind it.

What it costs: genital mycotic infection in roughly 1 in 10 men, volume depletion and orthostasis, 20–40 g/day glucosuria, Fournier's gangrene (rare but labeled), and euglycemic ketoacidosis.

**Why MONITOR rather than AVOID.** Ketoacidosis risk tracks relative insulin deficiency, not body weight and not the GLP-1 by itself. In DAPA-HF and DAPA-CKD, ketoacidosis events occurred **only** among participants with type 2 diabetes — none among the non-diabetic participants, across several thousand patient-years — and the T2D trial base rate is 0.6–2.2 events per 1,000 patient-years. Euglycemic ketoacidosis in true non-diabetics is real and has its own case literature, but it is rare and nearly always precipitant-driven: fasting, ketogenic diet, surgery, dehydration, acute illness, impaired renal ketone clearance. Being lean is not itself protective — the published SGLT2i-plus-tirzepatide case is a 35-year-old man with a BMI of 20.7, five weeks into the combination, tipped over by nausea and poor intake.

**The real incompatibility is fasting, not the anti-growth block** — see Part 3. An SGLT2 inhibitor is a caloric-restriction mimetic and belongs conceptually in an anti-growth phase; what it cannot share a calendar with is the FMD cycles inside that phase, or any tirzepatide week with vomiting or minimal intake. Those are choices, so this is an either/or rather than a permanent exclusion: run the fasting cycles or run the drug.

**Which agent.** The lifespan data is canagliflozin; the cleaner human safety record is empagliflozin, which carries no CANVAS-style amputation signal. You cannot have both, and the amputation signal is human evidence while the lifespan signal is mouse.

**When the calculus changes:** if you ever develop type 2 diabetes, CKD, or heart failure, SGLT2 inhibitors become first-line and genuinely excellent. Keep the row, change the trigger from "aging" to "diagnosis."

**On the microbiome pair:** these are two separate rows, because the product and its headline ingredient are on different trajectories. Pendulum is a 0.6% HbA1c agent tested in T2D on metformin, whose mechanism — SCFA-driven *endogenous* GLP-1 secretion — is the pathway tirzepatide already saturates pharmacologically, and its trial was authored end to end by seventeen company employees with no independent replication six years on. Pasteurized MucT is a different preparation with three independent RCTs behind it, including Mount et al. (*Nature Medicine*, June 2026, n=90, academic-led), which is the only positive RCT anywhere on this inventory aimed at **post-weight-loss regain** — the one problem GLP-1 users actually face. Buying Pendulum does not get you the trial you just read about. Skip it now; put pasteurized MucT on the taper plan.

### 2.3 AMPK and energy sensing

| Score | E×B | Item | Target | Safety | Effort |
|---:|:---:|---|---|:---:|:---:|
| **20** | 4×5 | Cardiorespiratory fitness training | endogenous AMPK, mitochondrial biogenesis | ok | moderate |
| **4** | 2×2 | Metformin | AMPK, complex I | monitor | trivial |
| **2** | 2×1 | Berberine | AMPK | **AVOID** | trivial |

Putting these three in one family makes the point immediately: **the best-evidenced AMPK activator on this list is exercise, and it is free.** Both pharmacological entries are competing against training and losing on every axis — evidence, effect size, cost, interaction profile.

Metformin's specific problem is that it blunts the VO₂max and mitochondrial adaptation that the intervention scoring 20 exists to produce. That is a *timing* conflict rather than a permanent exclusion (Part 3), and metformin's ~6 h half-life makes it the easiest item in the whole document to phase cleanly. Better schedulability does not improve its evidence, so it still scores 4.

Berberine's AVOID is pharmacokinetic — a potent CYP3A4 and P-gp inhibitor that raises statin, rapamycin and tadalafil exposure unpredictably — and does not relax in any phase.

### 2.4 mTOR and nutrient sensing — the anti-growth arm

| Score | E×B | Item | Target | Safety | Effort |
|---:|:---:|---|---|:---:|:---:|
| **6** | 2×3 | Rapamycin 5–6 mg weekly | mTORC1 | monitor | low |
| **4** | 2×2 | Time-restricted feeding / periodic FMD | AAR, FGF21, autophagy | ok | low |
| **4** | 2×2 | Methionine source shifting *(protein constant)* | amino acid composition — SAM/SAH, FGF21, IGF-1 | ok | low |
| **1** | 1×1 | Methionine restriction <1 g/day, 5 days/week | SAM/SAH, FGF21, IGF-1 | **AVOID as specified** | moderate |
| **1** | 1×1 | Methioninase (oral rMETase) | methionine degradation | **AVOID** | moderate |

Everything here pushes the same direction: down-regulate mTORC1 and IGF-1 signalling, favour autophagy and catabolic housekeeping, reduce the substrate available for anabolic error. This is the arm your hypothesis calls the pruning phase, and the framing is fair.

Three things are worth flagging inside the family. **Rapamycin's ~62 h half-life is an argument for block scheduling rather than weekly dosing** — five half-lives is about 13 days, so weekly dosing never cleanly separates from a 3×/week lifting schedule, while a block structure separates them completely. Bitto 2016 (*eLife*) found transient 3-month rapamycin in middle-aged mice produced persistent lifespan benefit, which is the pharmacological precedent for pulsed use.

And **FMD is already a cycle protocol** — 5 days on, then refeeding, a few times a year. Its score of 4 understates its relevance to Part 4, because it is the only item in this family with human trial infrastructure built around alternation rather than continuous administration.

**The methionine rows are graded on sufficiency, not on depth of cut.** The spread from 4 to 1 across them is not a dose-response where more restriction earns a worse flag for being aggressive — it is the shape of Longo's own curve, where too little methionine causes frailty and too much abolishes the benefit. Source shifting scores 4 because it lands inside that window; the sub-gram protocol and methioninase score 1 because they aim past it. Two practical consequences follow. Methionine work is **not** a substitute for the fasting cycles — the FGF21 and IGF-1 mechanisms overlap, but nothing in the dietary-composition literature touches the hematopoietic and immune reconstitution that fasting/refeeding produces, which is the specific reason FMD earns its place in Part 4. But it **is** compatible with an SGLT2 inhibitor, because composition at constant calories and carbohydrate is not a ketoacidosis precipitant. Methionine work runs in the anti-growth block either way; it is not the variable in the choice below.

### 2.5 GH / IGF-1 and anabolism — the pro-growth arm

| Score | E×B | Item | Target | Safety | Effort |
|---:|:---:|---|---|:---:|:---:|
| **15** | 3×5 | Resistance training 2–3×/wk | mTORC1, myonuclear addition, bone loading | ok | moderate |
| **12** | 3×4 | Protein 1.2–1.6 g/kg/day, distributed | muscle protein synthesis | ok | trivial |
| **9** | 3×3 | Creatine monohydrate 5 g/day | phosphocreatine, cell hydration | ok | trivial |
| **6** | 2×3 | **Block-periodized growth cycling** *(training-led, no rhGH)* | phase separation of mTORC1/IGF-1 | ok | moderate |
| **4** | 4×1 | Testosterone (absent hypogonadism) | androgen receptor | monitor | moderate |
| **2** | 1×2 | rhGH-containing pro-growth block (TRIIM/TRIIM-X style) | thymus regeneration; GH/IGF-1 axis | monitor | high |

This section is the counterweight to 2.4. Muscle and bone maintenance, tissue repair, immune reconstitution and wound healing all require anabolic signalling. A protocol that suppresses it continuously is buying protection from one set of failure modes by accepting exposure to another — sarcopenia, osteopenia, impaired repair, blunted immune reconstitution. That cost is real and it belongs in the ledger.

Note the internal ranking. **The best pro-growth intervention here is resistance training at 15, and the second is protein at 12.** Both are free, both are better evidenced than anything else in the family, and both are already on your do-now list. Any pro-growth phase you construct should be built on those two; the pharmacology is optional garnish on top of a foundation that carries the actual evidence.

Two items are worth reading in full in the detail file: [block-periodized growth cycling](therapeutics-by-mechanism.md#block-periodized-growth-cycling-training-led-no-rhgh) and [the rhGH block](therapeutics-by-mechanism.md#rhgh-containing-pro-growth-block-triim--triim-x-style). Both are argued out in Part 4.

### 2.6 Everything else, by family

**Senescence** — D+Q (1, monitor, skip) · fisetin (1, ok, skip). Senescent-cell burden at 39 is low; there is little to clear. Right idea, wrong decade. Note that senolytics are *already* designed as intermittent hit-and-run agents, and if you ever run growth cycling they belong at the end of an anti-growth block, immediately before the regenerative phase.

**NAD+** — NMN / NR (2, ok, skip). Human trials raise NAD+ without downstream functional benefit. Three source rows for one pathway.

**Redox and hormesis** — omega-3 (6, continue) · sauna (4, optional) · astaxanthin (2, skip — an ITP hit that failed to replicate) · NAC/GlyNAC/glutathione (2, skip). Organizing principle: the ROS burst after training is signal, not damage. Every item here is a timing question rather than a yes/no question — except NAC with methionine work, which is a genuine cancellation rather than a timing issue.

**Hemodynamic and vascular** — blood pressure to <120 systolic (20, monitor) · cardiorespiratory training (20, also listed under 2.3) · aspirin (5, **AVOID** — a high evidence score attached to a finding of no benefit; ASPREE showed net harm in healthy older adults).

**Inflammation** — low-dose colchicine (2, skip — CLEAR SYNERGY/OASIS-9 was neutral at n=7,062) · dental/periodontal care (4, do anyway).

**Immune and infectious** — Shingrix (12, **calendar item at 50**) · H. pylori test-and-treat (8) · hepatitis C one-time screening (8) · influenza vaccination (8) · HPV vaccination (8, **window shuts at 45**).

**Neurological, sensory, mental health** — depression screening and access (16 — suicide is among the leading causes of death for US males 35–44, and its absence from every longevity list is the same blind spot that omits seatbelts) · sleep 7–9 h (15) · hearing protection (9) · social connection (9).

**Diet composition** — alcohol minimal or none (12 — MR has dismantled the J-curve) · fiber 35–40 g/day (9).

**Environmental and external-cause** — nicotine and tobacco: none (25, confirm) · injury prevention (16) · radon test (12) · sun protection (8) · bedroom HEPA (6).

**Early detection** — cancer screening on schedule (20).

**No credible mechanism** — taurine (1, premise retracted by Fernandez 2025) · resveratrol (1) · 17α-estradiol (2, watch, do not take) · blood donation (4, optional) · methylene blue (1, **AVOID** — MAO-A inhibitor) · disease-indication drugs with no aging indication (1, change trigger to diagnosis) · the ~35-row supplement bundle (1) · EDTA/HBOT/stem cells/gene therapy (1, **AVOID**).

### 2.7 Flat ranked list

Score-ordered, all families collapsed.

| Score | Item | Family | Safety | Effort |
|---:|---|---|:---:|:---:|
| 25 | ApoB *(measure)* | diagnostics | ok | trivial |
| 25 | ApoB to <60 mg/dL | lipoprotein | monitor | trivial |
| 25 | Rosuvastatin / atorvastatin | lipoprotein | monitor | trivial |
| 25 | Evolocumab / alirocumab | lipoprotein (PCSK9) | ok | high |
| 25 | Nicotine and tobacco: none | environmental | ok | trivial |
| 20 | Blood pressure to <120 | vascular | monitor | trivial |
| 20 | Home BP series *(measure)* | diagnostics | ok | trivial |
| 20 | Cancer screening on schedule | early detection | ok | low |
| 20 | Cardiorespiratory fitness training | AMPK / vascular | ok | moderate |
| 20 | Inclisiran | lipoprotein (PCSK9) | ok | high |
| 20 | Enlicitide (Lipfendra), oral | lipoprotein (PCSK9) | ok | high |
| 16 | DEXA body composition | diagnostics | ok | trivial |
| 16 | Lp(a), once | diagnostics | ok | trivial |
| 16 | Home sleep apnea test | diagnostics | ok | low |
| 16 | Depression screening and access | mental health | ok | trivial |
| 16 | Injury prevention | environmental | ok | trivial |
| 16 | Ezetimibe | lipoprotein | ok | trivial |
| 16 | Bempedoic acid *(if statin-intolerant)* | lipoprotein | monitor | moderate |
| 16 | ApoB to <30 mg/dL | lipoprotein | monitor | high |
| 16 | Tirzepatide *(continue)* | incretin | monitor | moderate |
| 15 | Sleep 7–9 h | neurological | ok | trivial |
| 15 | Resistance training 2–3×/wk | anabolic | ok | moderate |
| 12 | Alcohol minimal or none | diet | ok | trivial |
| 12 | Protein 1.2–1.6 g/kg/day | anabolic | ok | trivial |
| 12 | Radon test | environmental | ok | trivial |
| 12 | Shingrix *(at 50)* | immune | ok | low |
| 12 | VO₂max *(measure)* | diagnostics | ok | low |
| 9 | Creatine 5 g/day | anabolic | ok | trivial |
| 9 | Fiber 35–40 g/day | diet | ok | trivial |
| 9 | Hearing protection | neurological | ok | trivial |
| 9 | Social connection | neurological | ok | low |
| 9 | Pasteurized *A. muciniphila* *(watch)* | incretin | ok | moderate |
| 8 | H. pylori · hepatitis C · influenza · sun protection · HPV | immune / environmental | ok | trivial–low |
| 8 | Lp(a)-lowering therapy *(watch)* | lipoprotein | ok | high |
| 6 | hsCRP · vitamin D · audiogram · grip · HEPA · APOE/PRS | diagnostics / environmental | ok | trivial–low |
| 6 | Omega-3 *(continue)* | redox | ok | trivial |
| 6 | Rapamycin | mTOR | monitor | low |
| 6 | **Block-periodized growth cycling** | anabolic | ok | moderate |
| 6 | SGLT2 inhibitors | incretin | monitor *(not with fasting cycles)* | low |
| 6 | Red yeast rice | lipoprotein | **AVOID** | trivial |
| 5 | Coronary artery calcium *(defer)* | diagnostics | ok | low |
| 5 | Aspirin | vascular | **AVOID** | trivial |
| 4 | Metformin · TRF/FMD · methionine via food · sauna · blood donation · dental · homocysteine panel | various | ok–monitor | trivial–moderate |
| 4 | Pendulum Glucose Control | incretin | ok | moderate |
| 4 | Testosterone (absent hypogonadism) | anabolic | monitor | moderate |
| 2 | Astaxanthin · NAC/GlyNAC · NMN/NR · 17α-estradiol · colchicine | various | ok–monitor | trivial–moderate |
| 2 | rhGH-containing pro-growth block | anabolic | monitor | high |
| 2 | Berberine | AMPK | **AVOID** | trivial |
| 1 | Fisetin · resveratrol · taurine · D+Q · supplement bundle · disease-indication drugs | various | ok–monitor | trivial–moderate |
| 1 | Methionine restriction <1 g/day · methioninase · methylene blue · EDTA/HBOT/stem cells | various | **AVOID** | moderate–high |

---

## Part 3 — Interactions

Interactions split into two categories, and the distinction matters, because it determines whether an item is *excluded* or merely *scheduled*.

- **Hard conflicts** are pharmacological. They do not resolve with timing, and none of them are affected by Part 4.
- **Phase conflicts** are conflicts of simultaneity. Two interventions pull the same lever in opposite directions *at the same moment*. Separating them in time resolves the conflict, and in several cases the separated version is how the intervention was designed to be used.

### Hard conflicts — these do not resolve with scheduling

**1. SGLT2 inhibitor + fasting or fasting-mimicking cycles → euglycemic ketoacidosis.**
The most dangerous combination available to you, and it is an either/or rather than a sequencing problem. Euglycemic ketoacidosis is documented in **non-diabetic** patients on SGLT2 inhibitors: the drug drives lipolysis and hepatic ketogenesis, and a fasted or carbohydrate-restricted state supplies the relative insulin deficiency that lets ketones run. Because glucose reads normal, it is routinely missed until severe decompensation.

Tirzepatide is an amplifier here, not the second party. It doesn't create the risk on a stable maintenance dose at maintenance calories — the non-diabetic arms of DAPA-HF and DAPA-CKD recorded no ketoacidosis events at all — but it does convert any bad GI week into the same precipitant profile: poor oral intake, vomiting, volume depletion. That is why the mitigation is a hold rule rather than a phase rule.

**Alternating blocks do not fix this one.** An FMD cycle inside an anti-growth block is precisely the state that precipitates it, so the anti-growth block cannot contain both. Run the FMD cycles, or run an SGLT2 inhibitor, and hold the drug for illness and for 3 days before any procedure either way.

**2. Methylene blue + any serotonergic agent** (SSRI, SNRI, triptan, MAOI) → serotonin syndrome. Methylene blue is a potent MAO-A inhibitor. Hospitalization-grade, not a caution.

**3. Berberine + rapamycin / statins / tadalafil** → berberine inhibits CYP3A4 and P-glycoprotein, raising exposure to all three unpredictably.

**4. Quercetin + dasatinib** → quercetin is itself a CYP3A4 inhibitor and raises dasatinib exposure. The senolytic protocol pairs them deliberately; the interaction is real regardless.

**5. Aspirin + fish oil + nattokinase** → additive bleeding risk with no offsetting indication at your age.

**6. GLP-1 agonist + procedures under anesthesia** → retained gastric contents and aspiration risk. Current anesthesia guidance calls for holding GLP-1s before elective procedures. Tell any surgeon, dentist or endoscopist.

**7. NAC or GlyNAC + methionine restriction → mutually cancelling.**
Cysteine supplementation reverses essentially the entire metabolic phenotype of methionine restriction in rodents — adiposity, hepatic SCD1 expression, insulin, leptin, triglycerides, adiponectin all revert to control. Elshorbagy's conclusion was that the anti-obesity effects of MR are driven by **low cysteine**, not low methionine per se.

This one is listed as hard rather than phase-based deliberately. You could in principle alternate them, but there is no reason to: the cancellation is complete, neither has outcome evidence, and running both in alternation would be funding opposite sides of the same experiment on a schedule instead of simultaneously.

### Phase conflicts — real, but scheduling problems rather than exclusions

None of these is a reason not to combine two interventions at all. What each says is *do not run these in the same window*.

**8. Rapamycin + resistance training.**
A single oral dose of rapamycin before resistance exercise **completely blocked** the contraction-induced rise in human muscle protein synthesis (~40% in controls), with S6K1 phosphorylation flat versus a 6-fold rise in controls. Notably, rapamycin did *not* affect post-absorptive protein metabolism — it specifically suppresses the *response to a stimulus*.

The half-life is roughly 62 hours, so five half-lives is about 13 days. **Weekly dosing cannot separate from a 3×/week lifting schedule — but a block structure separates them completely.** The correct conclusion is not "don't use rapamycin," it is "weekly dosing is the wrong administration pattern if you also lift." If you run it, run it inside an anti-growth block with the last dose ≥2 weeks before training volume comes back up.

Note the scores: resistance training 15, rapamycin 6, so on the merits training wins any contest for the same window. Cycling means you don't have to hold that contest.

**9. Metformin + exercise training.**
Same structure, easier fix. Metformin blunts VO₂max and mitochondrial adaptation, and the intervention with the evidence (cardiorespiratory training, 20) loses to accommodate the one without it (metformin, 4). Metformin's half-life is ~6 hours, making it the most cleanly phaseable item in the document. It still scores 4 — good schedulability is not evidence.

**10. High-dose antioxidants + exercise training.**
NAC, high-dose vitamin C/E, MitoQ, astaxanthin. The ROS burst after training is signal, not damage; suppressing it suppresses the adaptation. This is a *window* problem at the scale of hours, not a block problem — keep antioxidants away from the post-training window, or drop them. Given that none of them have outcome evidence, dropping them is simpler.

**11. IGF-1-raising agents + mTOR/IGF-1-lowering agents.**
The general case, and the one your hypothesis is aimed at. rhGH raises IGF-1; rapamycin, methionine restriction and the CR mimetics exist to lower it and to lower mTOR signalling. Run simultaneously, you are paying two premium prices to push one dial in opposite directions, and then measuring the result with an epigenetic clock that cannot tell you which one won.

Run in **alternating blocks**, that objection largely dissolves, and what remains is a real question about whether the alternation itself is beneficial. That question is Part 4.

### Redundancies — you're paying twice for one mechanism

- NAC + glutathione + GlyNAC (NAC is the precursor; pick one)
- NMN + NR + niacin (same pathway)
- Statin + red yeast rice (same molecule)
- MitoQ + astaxanthin + CoQ10 (three lipid-phase scavengers; the chemistry differs — MitoQ is not an ETC carrier and is not a CoQ10 substitute — but they fail together if oxidative damage isn't rate-limiting, and they share the exercise-timing problem above). CoQ10's real case is statin depletion or a cardiac diagnosis, not aging: change the trigger rather than stacking it.
- Glucosamine + chondroitin (weak individually, not additive)
- Multiple simultaneous senolytics
- Pendulum + separately-purchased *Akkermansia* (different preparations, overlapping intent — pick the one with the trial you actually want)

### Synergies worth noting

- **Statin + ezetimibe** — different mechanisms, additive ApoB reduction, both generic. Best value pairing in the document.
- **Resistance training + adequate protein + creatine** — the only combination that reliably protects lean mass during GLP-1 weight loss, and the foundation of any pro-growth phase.
- **PCSK9 inhibitor + statin** — statins slightly *raise* Lp(a); PCSK9 inhibitors lower it ~20–25%. Complementary if Lp(a) is elevated.
- **Senolytic at the end of an anti-growth block, immediately before a regenerative phase** — clear, then rebuild, which is the sequence the underlying biology suggests. Sensible design; does not make either senolytic worth taking at 39.
- **TRT + blood donation** (if TRT ever applies) — donation is the standard management for TRT-induced erythrocytosis.

### Monitoring requirements

| Agent | Watch |
|---|---|
| Rapamycin | Lipids, fasting glucose, CBC, mouth ulcers, wound healing before any surgery |
| Metformin | B12 annually |
| GLP-1/GIP | **Lean mass by DEXA**, gallbladder symptoms, hold before anesthesia |
| SGLT2i (if used) | Home β-hydroxybutyrate meter; genital mycotic infection; volume status. **Hold for any illness with poor oral intake, any fasting or FMD cycle, and 3 days pre-procedure** |
| Statin | ALT at baseline and once; CK only if symptomatic |
| rhGH (if ever) | IGF-1, fasting glucose and insulin, PSA, carpal tunnel symptoms, joint swelling |
| Any growth-cycling protocol | DEXA at every phase boundary; grip weekly; IGF-1 and fasting insulin at phase midpoints |

---

## Part 4 — Growth cycling

**Your hypothesis, as stated:** the anti-growth interventions — rapamycin, fasting, calorie and protein restriction, senolytics — are about pruning senescent cells, avoiding cancer, and getting into an efficient metabolic state that limits byproducts. But growth also matters, for muscle and bone preservation, tissue repair, and thymic regeneration. So rather than running one arm continuously, alternate: a ~6-week pro-growth block (TRIIM-X, heavy strength training, high protein, all anti-growth items suspended), then return to a mostly anti-growth lifestyle with reduced-volume training.

**The structural claim is sound.** Treating pro- and anti-growth as permanently opposed would justify an AVOID flag on TRIIM-X and a rejection of your methionine plan on scheduling grounds — but both of those arguments are about *simultaneity*, and both weaken considerably once the two arms are separated in time. The scoring below prices them that way.

What follows separates the hypothesis into three parts, because they have different evidence and deserve different answers: **the cycling structure**, **the pro-growth phase content**, and **the rhGH question specifically**.

### 4.1 What supports the cycling structure

Nothing here is a trial of block alternation itself — that trial does not exist. What exists is a set of adjacent results that make the structure mechanistically credible rather than merely appealing.

**Pulsed mTOR inhibition already has a precedent.** Bitto et al. (*eLife*, 2016) gave middle-aged mice rapamycin for three months and found lifespan benefit that persisted after withdrawal. Weekly rapamycin dosing in humans is itself a pulse strategy, adopted specifically to get mTORC1 inhibition without continuous immunosuppression. The field's own dosing convention concedes that continuous is not obviously better.

**Fasting protocols are already cycle protocols, and the refeeding phase does work.** Longo's FMD design is 5 days on, then refeeding, a few times a year — the alternation is the intervention, not a compromise. And the refeeding phase is not downtime: Cheng et al. (*Cell Stem Cell*, 2014) found that fasting/refeeding cycles drove hematopoietic stem cell self-renewal and immune reconstitution in mice. That is regeneration triggered by the *transition*, which is precisely the mechanism your hypothesis proposes.

Note what this means for your thymus goal specifically. **The regenerative endpoint you want from TRIIM-X has adjacent support from a protocol that is free, has human trial infrastructure, and does not require rhGH.** If you only take one thing from this section, take that one.

**Exercise periodization is the same idea in a field where it is uncontroversial.** Nobody trains at maximum volume continuously; accumulation and deload blocks alternate because the adaptation happens in the trough. Applying that logic to metabolic signalling is an analogy, not evidence — but it is a reasonable analogy, and the burden of proof that continuous is better has never been discharged either.

**The duty-cycle argument is arithmetically correct.** Two six-week pro-growth blocks a year is a ~23% duty cycle. If the risk of elevated IGF-1 is a function of cumulative exposure — which is the standard framing, and the same framing this document uses in your favour for ApoB — then the lifetime IGF-1 integral under cycling is roughly a quarter of continuous administration, while the anabolic stimulus during the block is undiminished. That materially blunts the IGF-1 exposure objection, and it is your strongest argument.

**It solves your own scheduling problem.** The single sharpest criticism of your original methionine plan was that 5-on/2-off put restriction directly on top of the 48–72 h remodelling window after weekend training — stimulus delivered, then substrate withdrawn. Block cycling fixes that completely: weeks of restriction, then weeks of building, with no interleaving. Whatever else is true, the block version is a strictly better design than the weekly version.

### 4.2 What is not established

**No human trial has tested block alternation against either arm run continuously.** Everything above is mechanism plus adjacent results. Evidence tier 2. That is why the row scores 6 and not 15.

**The optimal block length is guesswork.** Six weeks is a reasonable guess for a hypertrophy accumulation block, which is probably where the number came from, and it is defensible for that reason. But the timescales that matter for the anti-growth arm are different and mostly unmeasured in humans — autophagic flux, senescent-cell clearance, FGF21 kinetics. Nobody knows whether six weeks off rapamycin loses the benefit or preserves it.

**Washout is a real constraint on the transitions, and it is asymmetric.** Rapamycin needs ~2 weeks to clear five half-lives; a pro-growth block that starts 3 days after the last dose is not a clean pro-growth block. Metformin clears in a day. IGF-1 takes 1–2 weeks to normalize after rhGH withdrawal, so the anti-growth block does not truly begin the day the injections stop. Budget roughly two weeks of transition at each boundary, which means a 6-week pro-growth block occupies about 8 weeks of calendar.

**There is a plausible failure mode where you get the costs of both arms and the benefits of neither** — never sustaining restriction long enough to establish the metabolic phenotype, never sustaining training volume long enough to accumulate tissue. This is the same criticism that sank the 5-on/2-off methionine design, applied at a longer timescale. Longer blocks make it less likely, which argues for 6–12 weeks rather than 2–3.

**Cancer risk is the asymmetry that does not average out.** The pruning logic — clear damaged cells during restriction, then rebuild — assumes the clearing happens first and completely. If a pro-growth block instead supplies substrate and signalling to a lesion that the anti-growth block did not clear, the two phases are not symmetric in their consequences. This is speculative in both directions and there is no data to resolve it, but it is the reason to keep the pro-growth blocks anabolic rather than pharmacologically supraphysiologic, and the reason to keep cancer screening (which scores 20) on schedule regardless.

### 4.3 The pro-growth phase content

Here is the part where the analysis is unambiguous.

**Resistance training scores 15. Protein scores 12. Creatine scores 9. rhGH scores 2.** The pro-growth block that carries almost all of the available benefit is *training plus protein plus creatine plus sleep*, and it is free. Adding rhGH to that adds a poorly evidenced drug on top of a well-evidenced foundation, and the marginal contribution is unmeasured.

Two practical findings support running it hard:

**Maintenance is much cheaper than accumulation.** Trained individuals hold strength and lean mass on roughly one-third of accumulation volume for months (Bickel 2011 and the broader minimal-dose literature). Your instinct that weekend-only lifting during the anti-growth phase is sufficient to *hold* what you built is physiologically sound — that is maintenance volume, not detraining. What it will not do is build, which is the point of the structure.

**Protein cannot be banked, but it can be phased.** Muscle protein synthesis has a per-meal ceiling and a refractory period, which is why compressing a week's intake into a weekend fails. Compressing a *year's* anabolic emphasis into two six-week blocks does not have that problem, because you are not trying to make one meal do a week's work — you are running weeks of adequate intake back to back. The per-meal ceiling argument kills the weekend plan and does not touch the block plan.

**One constraint that does not relax:** you are on tirzepatide, and protein at 1.2–1.6 g/kg/day plus resistance training is the mitigation for drug-induced lean-mass loss. That mitigation cannot be suspended during anti-growth blocks. So the anti-growth phase is "reduced volume and reduced anabolic emphasis," not "restriction plus detraining." If the anti-growth block includes genuine protein restriction while you remain on a GLP-1, the lean-mass arithmetic goes the wrong way regardless of how good the cycling structure is.

### 4.4 The rhGH question

Scored separately at **1 × 2 = 2, MONITOR, high effort**.

**Why MONITOR rather than AVOID.** The strongest case for an AVOID would be "raises IGF-1, directly opposes rapamycin, methionine restriction and every CR mimetic on this list." That is a simultaneity argument, and a cycling structure answers it. Setting it aside leaves two objections, both real and both MONITOR-grade rather than AVOID-grade.

**What those two are, honestly.** First, the evidence base: TRIIM was n=9, single-arm, uncontrolled, with ~2.5 years of epigenetic age reversal measured by clocks that are not validated mortality surrogates, and seven years on there are no peer-reviewed TRIIM-X results — only a preliminary presentation at a Foresight talk in May 2026. The trial is participant-funded and sponsor-analyzed, which is a structurally weak evidence generator regardless of the underlying biology. Second, exogenous rhGH raises IGF-1 into a range that training and protein do not; elevated IGF-1 associates with increased prostate, colorectal and breast cancer risk, and reduced IGF-1/insulin signalling is the most conserved life-extension pathway across model organisms. The duty-cycle argument reduces that exposure substantially; it does not eliminate it, and it does not supply the missing efficacy data.

Third, a smaller point that the protocol makes about itself: metformin is in the cocktail specifically to offset GH-induced insulin resistance that the protocol creates. When a therapy needs a second drug to counteract its own primary side effect, that is information about the risk-benefit ratio.

**Eligibility.** NCT04375657 is ages 40–80. You are 39, so it is unavailable this year and available next year. If you want it, the honest reason to enroll at 40 is contributing data to a study that badly needs participants — not receiving a treatment whose effect size is unknown.

**The recommendation that follows.** Run the cycling structure. Build the pro-growth blocks out of training, protein, creatine and sleep, which is where the evidence is. Leave rhGH out of the first several cycles, because adding an unevidenced drug to an unevidenced schedule makes the result uninterpretable — if something improves, you will not know which change did it. If you still want the rhGH arm after two or three clean cycles, you will at least have a personal baseline to compare against, which is more than TRIIM-X itself has.

### 4.5 A concrete calendar, if you run it

Offered as a starting structure, not a protocol — nobody has tested this, and the parameters below are reasoned guesses.

| Weeks | Phase | Training | Diet | Pharmacology |
|---|---|---|---|---|
| 1–6 | **Pro-growth** | Resistance 3–4×/wk, progressive; cardio maintained at 2×/wk | Protein 1.6 g/kg/day distributed; adequate methionine; energy at or slightly above maintenance | Creatine 5 g/day. Nothing anti-growth. No antioxidant supplements near training. |
| 7–8 | Transition down | Taper resistance volume to maintenance | Protein holds at 1.2–1.6 | IGF-1 normalizing; nothing new started |
| 9–20 | **Anti-growth** | Resistance 1–2×/wk at maintenance volume; cardio 3×/wk | Protein holds ≥1.2 g/kg while on tirzepatide; shift methionine *sources* (legumes, soy, dairy) with methionine kept sufficient, rather than cutting protein; 1–2 FMD cycles | Rapamycin only if you decide it's worth 6 points; last dose ≥2 wk before week 21. **An SGLT2 inhibitor and the FMD cycles are mutually exclusive — pick one for this block.** |
| 21–22 | Transition up | Volume ramps | Protein to 1.6 | Rapamycin fully cleared before resistance volume rises |
| 23–28 | **Pro-growth** | repeat | repeat | repeat |

That is roughly two pro-growth blocks per year at a ~23% duty cycle, with 12 weeks of anti-growth emphasis between them and clean two-week transitions at every boundary.

### 4.6 How you would know if it's working

This is the part that separates a hypothesis from a belief, and it is worth more than the protocol design.

**Pre-specify these before starting:**

- **DEXA at every phase boundary** — not the Withings BIA, which will not resolve the 1–2 kg changes at stake. The pro-growth block should show lean mass up; the anti-growth block should show it flat, not falling. Lean mass falling during anti-growth blocks means the structure is failing at its main job.
- **Grip strength weekly** — cheapest early warning, and it moves before DEXA does.
- **IGF-1 and fasting insulin at each phase midpoint** — this is the readout that tells you the phases are actually different. If IGF-1 doesn't separate between blocks, you are not running two phases, you are running one phase with a varying training schedule.
- **ApoB every 8 weeks through the first cycle** — rapamycin raises lipids and a pro-growth block changes intake; the item scoring 25 should not drift while you experiment with items scoring 6.
- **A stopping rule.** If lean mass falls >1 kg across a full anti-growth block despite maintained protein and maintenance-volume training, the anti-growth phase is too aggressive. Shorten it or lighten it.

**And the honest caveat about clocks:** if you evaluate this with an epigenetic age test, you will get a number, and it will not mean what you want it to mean. The clocks are not validated mortality surrogates, they drift with assay batch and cell composition, and the effect sizes you are looking for are inside their noise. DEXA, grip, IGF-1 and ApoB are boring and they will actually tell you something.

**Score for the structure: evidence 2 × benefit 3 = 6, safety OK, effort moderate.** Scored at 6 rather than higher because it is a scheduling structure rather than a therapy — most of its value is already counted in the rows it schedules. Scored at 6 rather than lower because it converts three phase conflicts from exclusions into calendar entries, and because it recovers muscle, bone and repair capacity that a continuously anti-growth protocol gives away for free.

---

## Part 5 — The methionine restriction plan

You proposed: **<1 g methionine/day, five days a week, plus methioninase, with high protein and intense strength training on weekends.**

The underlying instinct is right. The implementation is likely to cost you muscle without delivering the mechanism. Eight problems, roughly in order of severity — and note that **problem 5 is the one your block-cycling hypothesis solves**, which is a real point in its favour.

### 1. The newest data says to keep methionine adequate, not cut it

Fanti, Longo et al., *Cell Metabolism*, June 2026 — the most directly relevant result published on this question. In aged mice, a low-protein "longevity diet" modeling traditional Mediterranean and Okinawan patterns **but supplemented with methionine (LDMM)** reduced fat mass and frailty, improved cardiometabolic markers, raised GH, GLP-1 and FGF21, and lowered IGF-1 — **without lean mass loss and without calorie restriction.** FGF21 was mechanistically required for the fat loss and insulin sensitivity.

Longo's own summary of the dose-response: **too little methionine caused frailty; too much abolished the benefits.** Their conclusion was that overall protein intake may matter less than specific amino acid composition, with a small but *sufficient* methionine intake.

So the lever is **total amino acids down, methionine kept adequate.** Your protocol does close to the inverse: methionine specifically down, total protein potentially high. You'd be aiming at the frailty arm of their dose-response curve.

### 2. Methionine is the initiator amino acid for every protein you make

Translation initiates with Met-tRNAi at every start codon. This isn't a substrate you can trade against leucine or adjust at the margin. Pushing it below requirement doesn't selectively throttle mTOR — it constrains protein synthesis globally, including the repair and remodeling you're training to stimulate.

### 3. The 5-on/2-off structure gets the costs without the benefits

Rodent MR uses roughly 0.17% methionine against 0.86% controls — about an 80% cut, **sustained continuously**, with the phenotype (FGF21 induction, hepatic SCD1 suppression, adiposity change) developing over days to weeks. Five-day cycles with full weekend refeeding are unlikely to establish that steady state.

The costs, meanwhile, accrue immediately: reduced muscle protein synthesis and negative nitrogen balance start on day one of restriction. You'd be collecting the debit reliably and the credit unreliably.

This is a **timescale** objection, not an objection to cycling as such. It says the cycle you chose is too short for the biology, which is an argument for the block structure in Part 4 and against the weekly one.

### 4. You can't bank a week's anabolism into a weekend

Muscle protein synthesis has a per-meal ceiling and a refractory period. The distribution literature consistently shows even protein spread across the day beats bolus loading for net synthesis. Compressing five days of missed intake into two doesn't recover it.

Note that this objection is specific to the weekend design and does not transfer to block cycling, where you are running weeks of adequate intake consecutively rather than asking two days to do a week's work.

### 5. Your training and your restriction are scheduled out of phase — and block cycling fixes this

Hard weekend lifting is fine while methionine-replete. But adaptation, remodeling and repair continue for 48–72 hours afterward — which lands on Monday and Tuesday, your restricted days. You'd deliver the stimulus and then withdraw the substrate precisely during the window when it's being used.

**This is the objection your hypothesis answers directly, and it answers it completely.** Multi-week blocks never interleave stimulus with withdrawal. If you are going to combine training with restriction at all, the block structure is the correct way to do it, and the weekly structure is not. Credit where it's due.

### 6. Drop the methioninase entirely

This is the part I'd remove without hesitation, and it is unaffected by any scheduling change.

- It's a **bacterial enzyme** from *Pseudomonas putida*, developed almost entirely by one laboratory (Hoffman / AntiCancer Inc.) over three decades.
- The injectable form **elicited strong immune reactions in primates**, requiring PEGylation to control antigenicity. Primate safety work also showed reduced food intake, weight loss, and transient declines in red cell values and hemoglobin.
- The oral form is sold as a **dietary supplement** — a regulatory classification, not a safety finding. It means no FDA review of either efficacy or safety.
- The clinical evidence is roughly **eight published studies across thirty years**, nearly all from the originating lab, all in advanced cancer. The oral human data is essentially **two case reports**: a 50% drop in circulating methionine within four hours in one ovarian cancer patient, and a ~70% PSA decline over three months in one prostate cancer patient. That is not a safety database.
- **Mechanistically it produces methanethiol, α-ketobutyrate, and ammonia.** Methanethiol is the principal compound behind severe oral and body malodor. Chronic gut-lumen generation of it is not a trivial cosmetic footnote. The enzyme also requires co-administered pyridoxal-5′-phosphate as cofactor.
- **Functionally it's redundant.** An oral enzyme acting in the gut lumen is a less controllable way of eating less methionine. Food selection achieves the same exposure reduction with a titration dial, a food log, an off switch, and no immunogenic bacterial protein.
- Long-term safety data in healthy people is not weak. It is **absent**.

### 7. The tirzepatide interaction is the practical constraint

GLP-1/GIP agonists produce substantial weight loss, and a meaningful fraction is lean mass unless protein intake and resistance training are aggressive. The evidence-based mitigation is **1.2–1.6 g/kg/day protein distributed across the day, plus 2–3 resistance sessions per week.**

The original protocol moves against both: it restricts protein quality five days a week and concentrates training into two. Stacked on drug-induced loss, the predictable result is accelerated sarcopenia — measured as a number you'd see on a DEXA before you'd feel it in the gym.

Block cycling improves this but does not remove it. As long as you are on tirzepatide, the protein floor holds in **both** phases; an anti-growth block that includes genuine protein restriction while the drug is running has the lean-mass arithmetic going the wrong way regardless of how well the blocks are designed.

### 8. Your own list contains the antidote

Cysteine supplementation reverses essentially all metabolic effects of methionine restriction. Running NAC or GlyNAC alongside cancels the experiment. This is a genuine cancellation rather than a timing problem — see Part 3, hard conflict 7.

### What <1 g/day actually means

Adult requirement for total sulfur amino acids (methionine + cysteine) is roughly 15 mg/kg/day — about 1.3 g/day for an 85 kg man. Methionine can be partially spared by cysteine. So **<1 g of methionine with adequate cysteine sits near, not far below, requirement.** That's the sane version of your plan. Adding methioninase on top is what pushes it into frank deficiency — the frailty arm of Longo's curve.

### The version I'd actually run

1. **Hold total protein at 1.2–1.6 g/kg/day, distributed across meals, in both phases.** Non-negotiable while on tirzepatide.
2. **Shift protein *sources*, don't cut protein *amount*.** Legumes, soy, and dairy carry substantially less methionine per gram of protein than beef, eggs, poultry, and especially fish. That drops methionine 25–40% while total protein stays flat. This is the LDMM pattern — largely plant-based, some fish.
3. **Get the FGF21 signal from time-restricted feeding or periodic fasting-mimicking cycles** — a few 5-day cycles a year — which have human trial data behind them rather than a chronic deficiency state. These slot naturally into the anti-growth blocks in Part 4.
4. **Drop methioninase.**
5. **Drop NAC/GlyNAC if you're pursuing methionine work at all** — pick one.
6. **Use block cycling rather than weekly cycling.** Resistance training 3×/week during pro-growth blocks, 1–2×/week at maintenance volume during anti-growth blocks. This is the change that resolves the phase problem, and it is your idea rather than mine.
7. **Measure properly.** DEXA at baseline and at every phase boundary — not the Withings BIA, which will not resolve the changes at stake. Grip strength weekly. Plasma methionine and homocysteine if you want the biochemical readout.
8. **Pre-specify a stopping rule.** If DEXA shows >1 kg lean mass loss across a full anti-growth block, the block is too aggressive.

### The thing you're actually reaching for

Halofuginone — a prolyl-tRNA synthetase inhibitor that triggers the amino acid response pathway pharmacologically, mimicking amino acid restriction without the nutritional deficit — extended median lifespan **+9% in male mice** in the 2025 ITP report. That is the concept you're after: the signal without the substrate loss. It's not available or advisable now, but it's the right thing to watch, and it's a better bet than a bacterial enzyme sold as a supplement.

---

## Caveats

Rapamycin, statins, ezetimibe, PCSK9 inhibitors, SGLT2 inhibitors, metformin, rhGH, and GLP-1 agonists are all prescription drugs requiring a physician. The interaction analysis above is a prompt for that conversation, not a substitute for it — bring the specific items (especially the SGLT2i ketoacidosis hold rules, and any growth-cycling plan involving rhGH) to whoever manages your tirzepatide.

I'm not a physician and this isn't medical advice. The scoring model is a sorting heuristic, not a measurement — the numbers are there to make the ranking's assumptions legible and arguable, not to imply precision.

Part 4 in particular describes a structure that **no human trial has tested**. It is scored at evidence tier 2 for that reason, and it is written as a hypothesis with a measurement plan attached rather than as a recommendation. The measurement plan is the part worth keeping if you discard everything else.
