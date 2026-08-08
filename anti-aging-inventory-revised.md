# Anti-Aging Therapeutic Inventory — Revised

**Target:** healthy male, age 39, US, currently on tirzepatide
**Revision date:** 8 August 2026
**Source:** AgingBiotech.info "Available Therapeutics" survey table (128 rows)

---

## Part 0 — The core problem with the current document

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

## Part 1 — The corrected framework

### Rank by competing-risk arithmetic, not by hallmark coverage

For a US male currently 39, lifetime cause-of-death is dominated by atherosclerotic cardiovascular disease (roughly a quarter), then cancer (roughly a fifth), then dementia, metabolic disease, and — in the next decade specifically — unintentional injury. Nothing on the geroscience list moves those numbers as much as the boring interventions do.

The decisive asymmetry at your age is **exposure-time leverage**. Mendelian randomization on lifelong lower LDL-C gives roughly a 54% CHD risk reduction per 1 mmol/L, versus roughly 22% per 1 mmol/L for statins started in mid-life and followed for five years. Same molecule, same target — about **three times the effect** because the clock started earlier. Starting ApoB control at 39 rather than 55 is, on its own, plausibly worth more than every supplement in the source table combined.

The same logic runs the other way for the speculative agents: at 39 you have the *most* time for an unrecognized harm to compound. Risk tolerance should be lower now, not higher.

### The scoring model

Two questions, multiplied. Everything else is a flag, not a number.

**EVIDENCE (1–5) — how well established is this in humans like you?**

| | |
|---|---|
| **5** | Multiple RCTs, hard clinical outcomes, in populations that include healthy adults |
| **4** | RCTs with hard outcomes but in older or diseased populations; or one strong RCT plus concordant Mendelian randomization |
| **3** | RCTs with surrogate endpoints only (ApoB, BP, VO₂max, lean mass); or large consistent cohorts plus MR |
| **2** | Replicated animal lifespan data (ITP); or human observational only |
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

### Why this replaced the four-axis version

The previous model scored EV, safety, cost and time and averaged the last three. Three things were wrong with it.

**Evidence was double-counted.** "EV" was defined as benefit *already discounted for evidence quality*, and then evidence appeared again as a separate letter grade. That conflated two independent questions — *does this work* and *does it matter* — into one number, so a well-proven trivial intervention and an unproven important one landed on the same score for opposite reasons. Splitting them and multiplying makes the disagreement legible: you can now argue about the 3 and the 5 separately.

**Averaging safety was a design failure.** Methylene blue carries a serotonin-syndrome interaction, but it's cheap and quick to take — so averaging safety (1) with cost (4) and time (5) produced a respectable 3.3 and diluted a hospitalization-grade risk into a middling number. Safety doesn't average. It's now a veto.

**Cost and time weren't discriminating.** Across the whole inventory they scored 4 or 5 on nearly every row — two columns of near-constants, adding width without adding information. They now sit outside the score as a single `effort` tag, which is where they actually belong: they don't change whether something *works*, they change whether it's worth the queue position. The clearest illustration is evolocumab, which scores a full 25 on the merits and is still gated behind a generic statin — not because the drug is worse, but because it's `high` effort and access-restricted, which is a scheduling fact rather than an efficacy one.

**And no more decimals.** 23.3 versus 20.0 implied a precision that doesn't exist. Integer products in a 1–25 grid, with the reasoning for both factors written out in the `why this score` column so any row can be challenged on its inputs rather than its arithmetic.

## Part 2 — The ranked inventory

Grouped by what to do, sorted by score within each group. Full reasoning for every score sits in the `why this score` column of the accompanying spreadsheet.

`E` = evidence · `B` = benefit · **score = E × B** · safety flag overrides score.

### Measure first — these gate the decisions below

| Score | E×B | Intervention | Safety | Effort | Note |
|---:|:---:|---|:---:|:---:|---|
| **25** | 5×5 | ApoB | ok | trivial | the input to the single best-evidenced intervention available to you |
| **20** | 5×4 | Home blood pressure series | ok | trivial | SPRINT and dozens of RCTs, hard outcomes |
| **16** | 4×4 | DEXA body composition | ok | trivial | the reference method for lean mass |
| **16** | 4×4 | Lp(a), once, lifetime | ok | trivial | each Lp(a) particle carries one apoB-100, so a high Lp(a) sets a floor under achievable ApoB |
| **16** | 4×4 | Home sleep apnea test | ok | low | diagnostic accuracy is solid; CPAP RCTs (SAVE, RICCADSA) were neutral for MACE though clearly positive for symptoms and BP |
| **12** | 4×3 | Radon test (home) | ok | trivial | consistent dose-response across miner cohorts and pooled residential analyses; no RCT is possible |
| **12** | 3×4 | VO2max | ok | low | observational only - nobody randomises people to fitness |
| **6** | 3×2 | Vitamin D (25-OH) | ok | trivial | VITAL was largely null for supplementation; correcting frank deficiency has better support |

### Do now

| Score | E×B | Intervention | Safety | Effort | Note |
|---:|:---:|---|:---:|:---:|---|
| **25** | 5×5 | ApoB to <60 mg/dL - statin (rosuvastatin or atorvastatin, generic) | monitor | trivial | do not stack with red yeast rice (same molecule); berberine raises exposure via CYP3A4 |
| **25** | 5×5 | Nicotine and tobacco: none | ok | trivial | *CONFIRM* — the single highest-value item in all of preventive medicine, conditional on being a user. Listed for completeness - a competing-risk inventory that om |
| **20** | 5×4 | Blood pressure to <120 systolic | monitor | trivial | SPRINT plus dozens of RCTs with hard outcomes |
| **20** | 5×4 | Cancer screening on schedule | ok | low | sigmoidoscopy and FIT RCTs show mortality reduction; NordICC was intention-to-treat disappointing but per-protocol positive |
| **20** | 4×5 | Cardiorespiratory fitness training | ok | moderate | rapamycin and metformin both blunt training adaptation; high-dose antioxidants blunt the hormetic signal |
| **16** | 4×4 | Depression screening and treatment access | ok | trivial | screening plus access to treatment reduces morbidity, and treatment RCTs are solid |
| **16** | 4×4 | Injury prevention | ok | trivial | natural-experiment and case-control evidence for seatbelts, helmets and safe storage is overwhelming even without RCTs |
| **15** | 3×5 | Sleep 7-9h | ok | trivial | strong and consistent observational plus Mendelian randomisation, but sleep-extension RCTs with hard outcomes do not exist |
| **15** | 3×5 | Resistance training 2-3x/wk | ok | moderate | rapamycin blocks contraction-induced muscle protein synthesis; methionine restriction removes the substrate |
| **12** | 4×3 | Alcohol minimal or none | ok | trivial | Mendelian randomisation has essentially dismantled the J-curve; the apparent benefit of moderate drinking was confounding |
| **12** | 3×4 | Protein 1.2-1.6 g/kg/day, distributed | ok | trivial | DIRECT CONFLICT with the proposed methionine restriction protocol |
| **9** | 3×3 | Creatine monohydrate 5 g/day | ok | trivial | hundreds of RCTs, but on strength and lean mass rather than hard outcomes |
| **9** | 3×3 | Fiber 35-40 g/day | ok | trivial | large consistent cohorts plus RCTs on surrogates |
| **9** | 3×3 | Hearing protection | ok | trivial | rests on the hearing-loss-to-dementia cohort literature |
| **9** | 3×3 | Social connection | ok | low | observational only, but the meta-analytic effect sizes for social isolation are in the same range as major behavioural risk factors |
| **8** | 4×2 | H. pylori stool antigen | ok | trivial | test-and-treat RCTs reduce gastric cancer incidence, though mostly in high-incidence populations |
| **8** | 4×2 | Hepatitis C: one-time screening | ok | trivial | USPSTF recommends one-time screening for all adults 18-79; direct-acting antivirals are curative in >95% |
| **8** | 4×2 | Influenza vaccination, annual | ok | trivial | efficacy RCTs are solid, and post-MI trials (IAMI) showed reduced all-cause death, hinting at a cardiovascular benefit beyond infection itself |
| **8** | 4×2 | Sun protection / UV avoidance | ok | trivial | RCTs show reduced melanoma and squamous cell carcinoma incidence with regular sunscreen use |
| **8** | 4×2 | HPV vaccination | ok | low | RCTs on cancer-precursor endpoints plus registry data on cancer incidence |
| **6** | 3×2 | Baseline audiogram | ok | trivial | hearing loss is the largest single modifiable dementia risk factor in the Lancet Commission model, but the causal chain rests on cohort data |
| **6** | 3×2 | Bedroom HEPA / PM2.5 awareness | ok | trivial | air pollution epidemiology is strong; the specific benefit of consumer HEPA is inferred |
| **6** | 3×2 | Grip dynamometer | ok | trivial | observational |
| **4** | 2×2 | Dental / periodontal care | ok | low | the CVD and dementia links are observational; intervention trials show surrogate improvement only |

### Continue — already in your stack

| Score | E×B | Intervention | Safety | Effort | Note |
|---:|:---:|---|:---:|:---:|---|
| **16** | 4×4 | GLP-1 / GIP agonist (tirzepatide) | monitor | moderate | ** euglycemic ketoacidosis if combined with an SGLT2i **; hold before anesthesia; conflicts with low-protein protocols |
| **6** | 3×2 | Omega-3 (EPA/DHA) | ok | trivial | additive bleeding with aspirin or nattokinase; AF signal at high dose |

### Conditional, calendar, and watch items

| Score | E×B | Intervention | Safety | Effort | Note |
|---:|:---:|---|:---:|:---:|---|
| **25** | 5×5 | PCSK9i - evolocumab / alirocumab / inclisiran | ok | high | *DO IF off target* — none known; additive with statin by design |
| **16** | 4×4 | Ezetimibe (generic) | ok | trivial | *DO IF off target* — IMPROVE-IT showed a real but modest hard-outcome benefit on top of statin |
| **16** | 4×4 | Bempedoic acid | monitor | moderate | *DO IF statin-intolerant* — raises uric acid; tendon rupture signal |
| **16** | 4×4 | ApoB to <30 mg/dL (the increment beyond <60) | monitor | high | *DO IF affordable* — requires a PCSK9i, which insurance will not cover without ASCVD or FH; Lp(a) sets a hard ApoB floor |
| **15** | 3×5 | PCSK9i - enlicitide (Lipfendra), oral | ok | high | *DO IF off target* — none known |
| **12** | 3×4 | Shingrix (recombinant zoster vaccine) | ok | low | *DO AT 50* — the zoster efficacy RCTs are excellent, but the dementia finding rests on natural experiments (Wales, Australia, Canada) and cohort data, not an RCT |
| **9** | 3×3 | Pasteurized A. muciniphila (MucT) - weight-regain prevention | ok | moderate | *WATCH (act if you come off tirzepatide)* — different preparation from Pendulum's - pasteurized single strain, not a live multi-strain blend |
| **8** | 2×4 | Lp(a)-lowering therapy (pelacarsen, olpasiran, lepodisiran, muvalap… | ok | high | *WATCH* — no outcomes data yet for any agent in the class |
| **6** | 3×2 | APOE genotype / CAD polygenic risk score | ok | low | *THINK FIRST* — ** GINA covers health insurance but NOT life, disability or long-term-care insurance ** |
| **5** | 5×1 | Coronary artery calcium | ok | low | *DEFER TO 45-50* — E5 for risk stratification |

### Optional — defensible, low stakes either way

| Score | E×B | Intervention | Safety | Effort | Note |
|---:|:---:|---|:---:|:---:|---|
| **6** | 3×2 | hsCRP | ok | trivial | consistently predictive, but interventions targeting it have a mixed record |
| **4** | 2×2 | Homocysteine, B12, folate | ok | trivial | homocysteine-lowering RCTs have not reduced cardiovascular events |
| **4** | 2×2 | Blood donation 2-3x/yr | ok | low | observational only |
| **4** | 2×2 | Methionine reduction via food choice (protein held constant) | ok | low | cancelled by NAC/GlyNAC; do not combine with total protein restriction on a GLP-1 |
| **4** | 2×2 | Time-restricted feeding / periodic FMD | ok | low | ** ketoacidosis risk if combined with an SGLT2i ** |
| **4** | 2×2 | Sauna 3-4x/wk | ok | moderate | the Finnish cohort data is suggestive and heavily confounded by who uses saunas; no RCT |

### Skip

| Score | E×B | Intervention | Safety | Effort | Note |
|---:|:---:|---|:---:|:---:|---|
| **6** | 3×2 | Red yeast rice / monacolins | **AVOID** | trivial | ** unstandardised lovastatin at an unknown dose - do not stack with a statin ** |
| **6** | 2×3 | Rapamycin 5-6 mg weekly | monitor | low | ** blocks contraction-induced muscle protein synthesis; t-half ~62h so weekly dosing does not clear a 3x/wk lifting schedule **; berberine and quercetin raise exposure |
| **4** | 2×2 | Metformin | monitor | trivial | ** blunts exercise VO2max and mitochondrial adaptation ** |
| **4** | 2×2 | Pendulum Glucose Control (WBF-011: A. muciniphila, C. butyricum, C.… | ok | moderate | *SKIP (for its stated indication)* — the chicory-root inulin is a fermentable prebiotic - stacked on tirzepatide's delayed gastric emptying it will likely worsen bloating and gas |
| **4** | 4×1 | Testosterone (absent hypogonadism) | monitor | moderate | raises hematocrit; suppresses fertility |
| **2** | 2×1 | Astaxanthin | ok | trivial | blunts exercise adaptation |
| **2** | 2×1 | Berberine | **AVOID** | trivial | ** potent CYP3A4 / P-gp inhibitor - raises statin, rapamycin and tadalafil exposure unpredictably ** |
| **2** | 2×1 | 17-alpha estradiol | monitor | low | a male-specific ITP hit (+19%) - genuinely one of the more interesting results in the field |
| **2** | 2×1 | Low-dose colchicine (Lodoco 0.5 mg) | monitor | low | interacts with CYP3A4 and P-gp inhibitors, including berberine and grapefruit |
| **2** | 2×1 | NAC / GlyNAC / glutathione | ok | low | ** cysteine reverses essentially all metabolic effects of methionine restriction (Elshorbagy) **; blunts exercise adaptation |
| **2** | 2×1 | NMN / NR | ok | moderate | redundant with niacin |
| **1** | 1×1 | Fisetin | ok | trivial | ITP result was null (-5 to +7%) |
| **1** | 1×1 | Resveratrol | ok | trivial | failed ITP, poor bioavailability, and the sirtuin mechanism itself is disputed |
| **1** | 1×1 | Taurine | ok | trivial | PREMISE RETRACTED. Fernandez et al., Science 2025 - longitudinal data across three human cohorts, rhesus monkeys and mice show taurine RISES or holds  |
| **1** | 1×1 | Bisphosphonates, acipimox, pentoxifylline, azithromycin, piperlongu… | monitor | low | *SKIP (change trigger to diagnosis)* — various |
| **1** | 1×1 | Dasatinib + quercetin (D+Q) | monitor | moderate | quercetin inhibits CYP3A4 and raises dasatinib exposure |
| **1** | 1×1 | Supplement bundle: AKG, spermidine, urolithin A, ergothioneine, api… | ok | moderate | several blunt exercise adaptation; several are CYP inhibitors; nattokinase adds bleeding risk |

### Avoid

| Score | E×B | Intervention | Safety | Effort | Note |
|---:|:---:|---|:---:|:---:|---|
| **5** | 5×1 | Aspirin | **AVOID** | trivial | additive bleeding with fish oil or nattokinase |
| **4** | 2×2 | SGLT2 inhibitors (canagliflozin, empagliflozin) | **AVOID** | low | *AVOID (revisit if T2D/CKD/HF)* — ** SEVERE: with a GLP-1 plus any carb restriction or fasting -> EUGLYCEMIC KETOACIDOSIS, documented in non-diabetics; glucose reads normal so it is routinely missed ** |
| **1** | 1×1 | Methylene blue | **AVOID** | trivial | ** potent MAO-A inhibitor: SEROTONIN SYNDROME with any SSRI, SNRI or triptan ** |
| **1** | 1×1 | Methioninase (oral rMETase) | **AVOID** | moderate | cancels with NAC/GlyNAC; compounds GLP-1 lean-mass loss |
| **1** | 1×1 | Methionine restriction <1g/day, 5 days/week | **AVOID** | moderate | ** compounds GLP-1 lean-mass loss; cancelled by NAC/GlyNAC; training and restriction are scheduled out of phase ** |
| **1** | 1×1 | EDTA chelation, HBOT, mitochondrial transfusion, stem cells / exoso… | **AVOID** | high | various |
| **1** | 1×1 | TRIIM / TRIIM-X protocol (rhGH + DHEA + metformin) | **AVOID** | high | ** raises IGF-1 - directly opposes rapamycin, methionine restriction and every CR mimetic on this list ** |

## Part 3 — Incompatibilities

### Hard conflicts — do not combine

**1. SGLT2 inhibitor + GLP-1 agonist + any carbohydrate restriction or fasting → euglycemic ketoacidosis.**
This is the most dangerous combination available to you, and you're already holding one of the three pieces.

Euglycemic ketoacidosis is documented in **non-diabetic** patients on SGLT2 inhibitors. The precipitant profile is reduced carbohydrate intake, volume depletion, relative insulin deficiency, and acute illness — which is a fair description of what a GLP-1 agonist does on a bad week. Because glucose reads normal, it is routinely missed until severe decompensation. Adding fasting, low-carb, or a GI-upset week to that stack is the documented recipe.

**2. NAC or GlyNAC + methionine restriction → mutually cancelling.**
Cysteine supplementation reverses essentially the entire metabolic phenotype of methionine restriction in rodents — adiposity, hepatic SCD1 expression, insulin, leptin, triglycerides, adiponectin all revert to control. Elshorbagy's conclusion was that the anti-obesity effects of MR are driven by **low cysteine**, not low methionine per se. Running both is funding opposite sides of the same experiment.

**3. Rapamycin + resistance training → blocks the adaptation you're training for.**
A single oral dose of rapamycin before resistance exercise **completely blocked** the contraction-induced rise in human muscle protein synthesis (~40% in controls), with S6K1 phosphorylation flat versus a 6-fold rise in controls. Notably, rapamycin did *not* affect post-absorptive protein metabolism — it specifically kills the *response to a stimulus*.

Rapamycin's half-life is roughly 62 hours. Weekly dosing does not cleanly separate from a 3×/week lifting schedule. If you use it: dose immediately after your last hard session of the week, take the longest possible gap before the next one, and accept that you're trading some hypertrophy for a speculative benefit. Given that resistance training scores 15 and rapamycin scores 6, that trade is backwards.

**4. Metformin + exercise training → blunts VO₂max and mitochondrial adaptation.**
Same structure as #3, same conclusion. The intervention with an EV of 5 loses to accommodate the one with an EV of 2.

**5. High-dose antioxidants + exercise training → blunt hormetic adaptation.**
NAC, high-dose vitamin C/E, MitoQ, astaxanthin. The ROS burst after training is signal, not damage. Suppressing it suppresses the adaptation. Keep antioxidants away from the post-training window, or drop them.

**6. Methylene blue + any serotonergic agent** (SSRI, SNRI, triptan, MAOI) → serotonin syndrome. Methylene blue is a potent MAO-A inhibitor. This is a hospitalization-grade interaction, not a caution.

**7. Berberine + rapamycin / statins / tadalafil** → berberine inhibits CYP3A4 and P-glycoprotein, raising exposure to all three unpredictably.

**8. Quercetin + dasatinib** → quercetin is itself a CYP3A4 inhibitor and raises dasatinib exposure. The senolytic protocol pairs them deliberately; the interaction is real regardless.

**9. Aspirin + fish oil + nattokinase** → additive bleeding risk with no offsetting indication at your age.

**10. GLP-1 agonist + procedures under anesthesia** → retained gastric contents and aspiration risk. Current anesthesia guidance calls for holding GLP-1s before elective procedures. Tell any surgeon, dentist, or endoscopist.

### Redundancies — you're paying twice for one mechanism

- NAC + glutathione + GlyNAC (NAC is the precursor; pick one)
- NMN + NR + niacin (same pathway)
- Statin + red yeast rice (same molecule)
- MitoQ + astaxanthin + CoQ10 + ergothioneine + green tea extract (one antioxidant thesis, five invoices)
- Glucosamine + chondroitin (weak individually, not additive)
- Multiple simultaneous senolytics

### Synergies worth noting

- **Statin + ezetimibe** — different mechanisms, additive ApoB reduction, both generic. Best value pairing in the document.
- **Resistance training + adequate protein + creatine** — the only combination that reliably protects lean mass during GLP-1 weight loss.
- **PCSK9 inhibitor + statin** — statins slightly *raise* Lp(a); PCSK9 inhibitors lower it ~20–25%. Complementary if Lp(a) is elevated.
- **TRT + blood donation** (if TRT ever applies) — donation is the standard management for TRT-induced erythrocytosis.

### Monitoring requirements

| Agent | Watch |
|---|---|
| Rapamycin | Lipids, fasting glucose, CBC, mouth ulcers, wound healing before any surgery |
| Metformin | B12 annually |
| GLP-1/GIP | **Lean mass by DEXA**, gallbladder symptoms, hold before anesthesia |
| SGLT2i (if ever) | Ketones, genital mycotic infection, volume status, hold 3 days pre-procedure |
| Statin | ALT at baseline and once; CK only if symptomatic |
| Boron / T-boosting stack | Free and total testosterone, SHBG, hematocrit, PSA baseline |

---

## Part 4 — The items you asked about

### TRIIM-X — skip, and not just because you're ineligible

**Status as of August 2026:** NCT04375657 remains open, ages **40–80**. You are 39, so it is not available to you regardless. Seven years after the original TRIIM publication, **no peer-reviewed TRIIM-X results exist.** The only public data is a "sneak peek" of preliminary findings presented in a Foresight Institute talk in May 2026.

**Four structural problems, in ascending order of importance:**

1. **The original trial was n=9, single-arm, uncontrolled.** Epigenetic age reversal of ~2.5 years, measured by clocks that are not validated surrogates for mortality benefit. No control group means no way to separate treatment from regression to the mean, measurement drift, or the behavioral changes that accompany enrolling in a longevity study.

2. **TRIIM-X is participant-funded and sponsor-run.** Intervene Immune markets it alongside a diagnostics program: "Access cutting-edge thymus regeneration treatment through our TRIIM-X clinical trial." A paid, single-arm, sponsor-analyzed study is a structurally weak evidence generator no matter how good the underlying biology is.

3. **The protocol contains its own tell.** Growth hormone causes insulin resistance. Metformin is in the cocktail specifically to mitigate a harm the protocol creates. When a therapy needs a second drug to offset its own primary side effect, that's a signal about the risk-benefit ratio, not a sign of sophistication.

4. **The biology doesn't apply to you.** Thymic involution at 39 is modest; the immunosenescence rationale is built on 65-year-olds. And recombinant GH in a man with an intact GH axis raises IGF-1 — where the evidence points the *other* way. Elevated IGF-1 associates with increased prostate, colorectal, and breast cancer risk, and reduced IGF-1/insulin signaling is the most conserved life-extension pathway across every model organism tested.

**The sharpest objection:** TRIIM raises IGF-1. Methionine restriction, rapamycin, and every CR-mimetic on your list exist to *lower* IGF-1 and mTOR signaling. If you ran both, you would be paying two premium prices to push the same dial in opposite directions, and then measuring the result with an epigenetic clock that can't tell you which one won.

**Score: evidence 1 × benefit 1 = 1, safety AVOID, effort high.** Revisit at 60, if by then there is a controlled trial with clinical endpoints.

---

### PCSK9 inhibitors — the real upgrade, but fourth in line

This is the item on your list with the largest genuine upside, **conditional on your ApoB and Lp(a) numbers**, which you haven't measured.

**What changed since your document was last updated:** On 15–16 July 2026 the FDA approved **enlicitide decanoate (Lipfendra)** — the first **oral** PCSK9 inhibitor, a macrocyclic peptide, 20 mg once daily. Placebo-adjusted LDL-C reduction was **55.8%** in CORALreef Lipids (n=2,904) and **59.4%** in CORALreef HeFH, with roughly **50% ApoB reduction** and adverse events comparable to placebo. In CORALreef AddOn it beat ezetimibe, bempedoic acid, and their combination on top of background statins.

That removes the injection barrier that kept this class from wider use — the field has long attributed poor real-world uptake of injectable PCSK9 inhibitors to prior-authorization burden and injection logistics rather than to the drug's efficacy.

**Three things that should temper the enthusiasm:**

1. **No cardiovascular outcomes data for enlicitide yet.** Approval rests on LDL-C alone. CORALreef Outcomes (>14,500 enrolled) is still running. The class prior is good — FOURIER and ODYSSEY established outcome benefit for the monoclonals — but "this specific agent reduces events" remains unproven.

2. **Coverage will be the binding constraint.** Prior authorization for PCSK9 inhibitors generally requires established ASCVD or heterozygous FH *plus* maximally tolerated statin therapy. A healthy 39-year-old with no event history meets none of that. Cash price for the injectable class runs ~$500–600/month; enlicitide's pricing and coverage pathway are not yet established.

3. **You have not exhausted the cheap options.** Generic rosuvastatin plus generic ezetimibe costs under $25/month and gets most people to an ApoB target. Reaching for a $6,000/year drug before trying a $300/year one is the definition of a poor bang-for-buck decision.

**Where Lp(a) changes the calculus:** if your Lp(a) comes back elevated (>125 nmol/L, and especially >200), the case strengthens considerably, because statins slightly *raise* Lp(a) while PCSK9 inhibitors lower it ~20–25%. The dedicated Lp(a) agents are close but not here: **Lp(a)HORIZON** (pelacarsen, n=8,323) is the first cardiovascular outcomes trial for any Lp(a)-lowering therapy and is expected to report before the end of 2026, with olpasiran, lepodisiran, and oral muvalaplin behind it. That readout will define the field. **Measuring Lp(a) now costs $30 and tells you whether to care.**

**Recommended sequence:** ApoB + Lp(a) → generic statin → add ezetimibe → reassess ApoB at 8 weeks → escalate to PCSK9 inhibitor only if off target or Lp(a) is high.

**Scores — generic statin: evidence 5 × benefit 5 = 25, effort trivial. Ezetimibe: 4 × 4 = 16, effort trivial. Evolocumab/alirocumab/inclisiran: 5 × 5 = 25, effort high. Enlicitide: 3 × 5 = 15, effort high.**

Note what the model is telling you here. The injectable PCSK9 inhibitors score a full 25 — identical to the generic statin — because on the merits they are that good. Enlicitide scores lower *only* because its outcomes trial hasn't reported, not because it's expensive. What actually keeps all of them behind the statin is the `effort` tag and the coverage gate, which are scheduling facts rather than efficacy ones. That separation is the point of the revised scoring.

---

### How low should ApoB go? — the case for and against a sub-30 target

Worth splitting into two line items, because the two moves have different evidence, different economics, and different answers.

| | ApoB 100 → 60 | ApoB 60 → 30 |
|---|---|---|
| **How** | Generic statin, ± generic ezetimibe | Statin + ezetimibe + PCSK9 inhibitor |
| **Evidence** | 5 | 4 |
| **Benefit** | 5 | 4 |
| **Score** | **25** | **16** |
| **Cost** | ~$60/yr | ~$6,000/yr |
| **Insurance** | Covered | Not without ASCVD or FH |

**What supports going very low.** FOURIER-OLE followed patients for a median of five years beyond the parent trial and found a *monotonic* relationship: lower achieved LDL-C, down to under 20 mg/dL, tracked with lower cardiovascular risk, with no significant safety concerns. Roughly a quarter of that cohort was living below 20 mg/dL. The earlier prespecified FOURIER analysis found the same monotonic pattern with no signal for new-onset diabetes, cataracts, neurocognitive events, malignancy, or hemorrhagic stroke across achieved-LDL strata. No threshold of diminishing return has been found.

The genetic evidence is the closest thing we have to a fifty-year experiment. People carrying loss-of-function variants in *PCSK9* or *ANGPTL3* live their entire lives with LDL-C in the teens and are healthy, fertile, and markedly protected from coronary disease. That is reassuring in a way no trial can be, because it covers the duration a trial never will.

And the cumulative-exposure argument cuts in favor of you specifically. If risk is a function of the integral of ApoB over time, then a 39-year-old has fifty years over which a deeper reduction compounds. **The sub-30 target is more defensible at your age than at 65**, which is the opposite of how these decisions usually get made.

**What argues against it.** Four things, none fatal, cumulatively enough to score it 16 rather than 25.

1. **Nobody has ever been randomized to this target.** Every supporting analysis is post-hoc, comparing people who *happened* to achieve very low levels. Those people differ systematically from those who didn't — better adherence, different baseline, different metabolism. The multivariable adjustment helps; it doesn't make it a randomized comparison. This is the single reason evidence is 4 rather than 5.

2. **The second increment is a smaller slice of a shrinking pie.** Proportional risk reduction per unit of ApoB lowered is roughly constant, but *absolute* benefit scales with the baseline risk you're operating on — and you've already cut that with the first move. So you pay roughly 100× more per year for a smaller absolute return. That's not an argument that it doesn't work. It's an argument that it's an ordinary purchase where the first increment was an extraordinary one.

3. **Duration mismatch.** The longest data at LDL under 20 is about seven years, in older secondary-prevention patients. Pharmacologic suppression starting at 39 is not identical to germline-low levels from conception — different tissue exposure history, different developmental window. The genetic evidence is reassuring by analogy, not by demonstration.

4. **Lp(a) may put a floor under it.** Every Lp(a) particle carries one apoB-100, so measured ApoB includes an Lp(a)-derived component you cannot remove with LDL-directed therapy. If your Lp(a) is high, a sub-30 ApoB may be arithmetically unreachable — another reason the $30 test comes first.

**On your hormone stack specifically**, since cholesterol is the steroidogenesis substrate and this is the obvious worry: the 2024 systematic review (21 studies, 9,879 patients) found statins lower *total* testosterone by about 13 ng/dL in randomized trials — real, but not enough to drop anyone below the normal range — with **no difference in free testosterone, LH, estradiol, or SHBG.** Free testosterone is the fraction that matters for symptoms. This is not a reason to hold back.

**Practical answer.** Get to ApoB 60 with the $60/year generic — that decision is close to unambiguous. Then measure Lp(a). If it's elevated, the sub-30 target becomes both more valuable and possibly unreachable, and the PCSK9 inhibitor earns its price on the Lp(a) reduction alone. If Lp(a) is low and you hit 60 easily, going to 30 is a defensible six-thousand-dollar-a-year bet on an extrapolation — reasonable, not obligatory, and the kind of thing to revisit when CORALreef Outcomes reads out and puts a hard number on the oral option.


---

### SGLT2 inhibitors — I'd reverse your ranking entirely

Your sheet gives this a gerotherapeutics score of 12/12, the highest in the table, with the note "top scoring candidate for TAME-like trial." That note is doing more work than you may realize: **the score means "most deserving of a trial," which entails that the human aging evidence does not yet exist.**

**What the evidence actually supports:**
- ITP canagliflozin: **+14% median lifespan in males only**, no effect in females. Real, replicated within ITP, and it happens to be your sex.
- Human outcome trials — EMPA-REG, CANVAS, DECLARE, DAPA-HF, EMPEROR, DAPA-CKD, EMPA-KIDNEY — are uniformly excellent, and uniformly in **type 2 diabetes, heart failure, or chronic kidney disease.** Much of the benefit is hemodynamic and renal. There is **no trial in metabolically healthy non-diabetics**, and no strong reason to assume the mechanism transfers to someone with normal kidneys and no heart failure.

**What it costs you:**
- Genital mycotic infection in roughly 1 in 10 men
- Volume depletion and orthostasis
- 20–40 g/day glucosuria — a persistent urinary glucose substrate
- Fournier's gangrene (rare, but a labeled concern)
- **Euglycemic ketoacidosis**

**And the specific reason it's wrong for you right now:** you are on tirzepatide. GLP-1/GIP agonists substantially reduce caloric intake, can cause vomiting and dehydration, and shift substrate use toward fat oxidation. That is precisely the precipitant profile for euglycemic ketoacidosis. Layer in any carb restriction, fasting protocol, or gastroenteritis week and you have assembled every documented risk factor at once. The presentation is subtle because glucose reads normal — which is exactly why it gets missed.

There is also a redundancy argument: the metabolic benefits you'd be reaching for, tirzepatide already delivers, with human hard-outcome data behind it.

**Score: evidence 2 × benefit 2 = 4, safety AVOID, effort low.** The AVOID flag here is driven by the tirzepatide interaction, not by the drug in isolation — which is exactly the distinction a flag can make and an averaged safety score cannot.

**When this flips:** if you ever develop type 2 diabetes, CKD, or heart failure, SGLT2 inhibitors become first-line and genuinely excellent. Keep the row, change the trigger condition from "aging" to "diagnosis."

---

### Pendulum Glucose Control — right to separate it out, wrong indication for you

You're correct that this shouldn't sit inside a generic "probiotics" row. Evidence in this field attaches to **named strains at named doses**, not to the category, and collapsing a clinically-tested five-strain formulation into the same bucket as store-brand acidophilus was too coarse. Fixed. But separating it out produces two rows, not one, because the product and its headline ingredient are now on different evidence trajectories.

**The Pendulum trial is real and it is thin.** Perraudeau et al., *BMJ Open Diabetes Research & Care*, 2020 (NCT03893422): randomized, double-blind, placebo-controlled, 12 weeks, T2D subjects on metformin ± sulfonylurea. WBF-011 produced HbA1c −0.6% and a 33% reduction in postprandial glucose AUC against placebo. That is a genuine, properly-designed trial and better than what backs almost anything else in your source table's supplement section.

The problems are structural rather than methodological:

- **The active arm was n=23** against n=26 placebo, out of 76 randomized across three arms.
- **All seventeen authors were Pendulum employees.** Not "industry-funded" — industry-authored, end to end.
- The paper describes itself as a **proof-of-concept study**.
- **Six years on, there is still no independent replication.** The one planned academic study (USC, NCT04228003) was withdrawn before enrolling anyone: *"the funding and project never started."*
- The 2022 *BMC Microbiology* follow-up showing circulating butyrate and ursodeoxycholate rose is mechanistically supportive but comes from the same group.

**The indication mismatch is the bigger problem.** The studied population was type 2 diabetics on metformin. You are on tirzepatide, which lowers HbA1c by roughly 2.0–2.4%. This is a 0.6% agent, and its proposed mechanism — short-chain fatty acids driving *endogenous* GLP-1 secretion — is precisely the pathway your drug already saturates pharmacologically. Nobody has tested it on top of a GLP-1. Adding it is paying roughly $2,000/year to nudge a lever that is already pinned.

**One concrete caution:** the formulation includes chicory-root inulin, a fermentable prebiotic. Stacked on tirzepatide-delayed gastric emptying, expect more bloating and gas, not less.

**Score: evidence 2 × benefit 2 = 4.** Same band as metformin and time-restricted feeding — not absurd, not justified.

### But the ingredient is having a much better year than the product

Here is the part worth your attention, and it points somewhere other than glucose control.

**Mount et al., *Nature Medicine*, June 2026** (n=90, Maastricht and Copenhagen, academic-led): participants completed an 8-week low-energy diet for ≥8% weight loss, then spent 24 weeks eating *ad libitum* with daily pasteurized *A. muciniphila* MucT or placebo. Weight regain was **1.2 ± 0.7 kg on MucT versus 3.2 ± 0.4 kg on placebo** (P = 0.012). Net weight loss from baseline was 3.1 kg greater (P = 0.009). Roughly **40% of the MucT group kept losing weight** during maintenance, against about 5% on placebo. No serious treatment-related adverse events. Depommier 2019 (*Nature Medicine*, n=32) and Zhang 2025 (*Cell Metabolism*) point the same direction.

That is a positive randomized trial aimed squarely at **the one problem GLP-1 users actually face** — regain after stopping. It is the only supplement anywhere on this inventory with an RCT targeting that question.

Three things keep it at 9 rather than higher:

1. **It's a different preparation.** Mount used *pasteurized* single-strain MucT. Pendulum sells *live* multi-strain. This is not a pedantic distinction — the activity is attributed to the heat-stable surface protein Amuc_1100, and there is an open argument that pasteurized preparations outperform live ones partly because live *Akkermansia* may not survive gastric transit in standard capsules. Buying Pendulum does not get you the trial you just read about.
2. **The weight loss was diet-induced, not GLP-1-induced.** Post-tirzepatide regain is a different physiological setting, and applying the result there is an extrapolation.
3. **Both Zhang and Mount found the benefit concentrates in people with low baseline *Akkermansia*.** So it is responder-dependent, and there is no validated consumer test to tell you whether you're a responder. An effect of ~2 kg over 24 weeks, averaged across responders and non-responders, is what you'd be buying blind.

**Practical read:** skip it now — it does nothing your tirzepatide isn't already doing harder. Put pasteurized MucT on the watch list and revisit it as part of the taper plan, which is when regain becomes the live question. That is also the moment to have resistance training, protein at 1.2–1.6 g/kg, and creatine already established, since those carry better evidence for the same goal and cost a fraction as much.


---

## Part 5 — The methionine restriction plan

You proposed: **<1 g methionine/day, five days a week, plus methioninase, with high protein and intense strength training on weekends.**

I think the underlying instinct is right and the implementation is likely to cost you muscle without delivering the mechanism. Eight problems, roughly in order of severity.

### 1. The newest data says to keep methionine adequate, not cut it

Fanti, Longo et al., *Cell Metabolism*, June 2026 — the most directly relevant result published on this question. In aged mice, a low-protein "longevity diet" modeling traditional Mediterranean and Okinawan patterns **but supplemented with methionine (LDMM)** reduced fat mass and frailty, improved cardiometabolic markers, raised GH, GLP-1 and FGF21, and lowered IGF-1 — **without lean mass loss and without calorie restriction.** FGF21 was mechanistically required for the fat loss and insulin sensitivity.

Longo's own summary of the dose-response: **too little methionine caused frailty; too much abolished the benefits.** Their conclusion was that overall protein intake may matter less than specific amino acid composition, with a small but *sufficient* methionine intake.

So the lever is **total amino acids down, methionine kept adequate.** Your protocol does close to the inverse: methionine specifically down, total protein potentially high. You'd be aiming at the frailty arm of their dose-response curve.

### 2. Methionine is the initiator amino acid for every protein you make

Translation initiates with Met-tRNAi at every start codon. This isn't a substrate you can trade against leucine or adjust at the margin. Pushing it below requirement doesn't selectively throttle mTOR — it constrains protein synthesis globally, including the repair and remodeling you're training to stimulate.

### 3. The 5-on/2-off structure gets the costs without the benefits

Rodent MR uses roughly 0.17% methionine against 0.86% controls — about an 80% cut, **sustained continuously**, with the phenotype (FGF21 induction, hepatic SCD1 suppression, adiposity change) developing over days to weeks. Five-day cycles with full weekend refeeding are unlikely to establish that steady state.

The costs, meanwhile, accrue immediately: reduced muscle protein synthesis and negative nitrogen balance start on day one of restriction. You'd be collecting the debit reliably and the credit unreliably.

### 4. You can't bank a week's anabolism into a weekend

Muscle protein synthesis has a per-meal ceiling and a refractory period. The distribution literature consistently shows even protein spread across the day beats bolus loading for net synthesis. Compressing five days of missed intake into two doesn't recover it.

### 5. Your training and your restriction are scheduled exactly out of phase

Hard weekend lifting is fine while methionine-replete. But adaptation, remodeling and repair continue for 48–72 hours afterward — which lands on Monday and Tuesday, your restricted days. You'd deliver the stimulus and then withdraw the substrate precisely during the window when it's being used.

### 6. Drop the methioninase entirely

This is the part I'd remove without hesitation.

- It's a **bacterial enzyme** from *Pseudomonas putida*, developed almost entirely by one laboratory (Hoffman / AntiCancer Inc.) over three decades.
- The injectable form **elicited strong immune reactions in primates**, requiring PEGylation to control antigenicity. Primate safety work also showed reduced food intake, weight loss, and transient declines in red cell values and hemoglobin.
- The oral form is sold as a **dietary supplement** — that is a regulatory classification, not a safety finding. It means no FDA review of either efficacy or safety.
- The clinical evidence is roughly **eight published studies across thirty years**, nearly all from the originating lab, all in advanced cancer. The oral human data is essentially **two case reports**: a 50% drop in circulating methionine within four hours in one ovarian cancer patient, and a ~70% PSA decline over three months in one prostate cancer patient. That is not a safety database.
- **Mechanistically it produces methanethiol, α-ketobutyrate, and ammonia.** Methanethiol is the principal compound behind severe oral and body malodor. Chronic gut-lumen generation of it is not a trivial cosmetic footnote. The enzyme also requires co-administered pyridoxal-5′-phosphate as cofactor.
- **Functionally it's redundant.** An oral enzyme acting in the gut lumen is a less controllable way of eating less methionine. Food selection achieves the same exposure reduction with a titration dial, a food log, an off switch, and no immunogenic bacterial protein.
- Long-term safety data in healthy people is not weak. It is **absent**.

### 7. The tirzepatide interaction is the practical dealbreaker

GLP-1/GIP agonists produce substantial weight loss, and a meaningful fraction is lean mass unless protein intake and resistance training are aggressive. The evidence-based mitigation is **1.2–1.6 g/kg/day protein distributed across the day, plus 2–3 resistance sessions per week.**

Your protocol moves against both: it restricts protein quality five days a week and concentrates training into two. Stacked on drug-induced loss, the predictable result is accelerated sarcopenia — measured as a number you'd see on a DEXA before you'd feel it in the gym.

### 8. Your own list contains the antidote

GlyNAC is row 18. Cysteine supplementation reverses essentially all metabolic effects of methionine restriction. Running both cancels the experiment.

### What <1 g/day actually means

Adult requirement for total sulfur amino acids (methionine + cysteine) is roughly 15 mg/kg/day — about 1.3 g/day for an 85 kg man. Methionine can be partially spared by cysteine. So **<1 g of methionine with adequate cysteine sits near, not far below, requirement.** That's the sane version of your plan. Adding methioninase on top is what pushes it into frank deficiency — the frailty arm of Longo's curve.

### The version I'd actually run

1. **Hold total protein at 1.2–1.6 g/kg/day, distributed across meals.** Non-negotiable while on tirzepatide.
2. **Shift protein *sources*, don't cut protein *amount*.** Legumes, soy, and dairy carry substantially less methionine per gram of protein than beef, eggs, poultry, and especially fish. That drops methionine 25–40% while total protein stays flat. This is the LDMM pattern — largely plant-based, some fish.
3. **Get the FGF21 signal from time-restricted feeding or periodic fasting-mimicking cycles** — a few 5-day cycles a year — which have human trial data behind them rather than a chronic deficiency state.
4. **Drop methioninase.**
5. **Drop NAC/GlyNAC if you're pursuing methionine restriction at all** — pick one.
6. **Move resistance training to 3×/week spread across the week**, not compressed into two weekend days. This matters more than the methionine question.
7. **Measure properly.** DEXA at baseline and 12 weeks — not the Withings BIA, which will not resolve the changes at stake. Grip strength weekly. Plasma methionine and homocysteine if you want the biochemical readout.
8. **Pre-specify a stopping rule.** If DEXA shows >1 kg lean mass loss at 12 weeks, stop.

### The thing you're actually reaching for

Halofuginone — a prolyl-tRNA synthetase inhibitor that triggers the amino acid response pathway pharmacologically, mimicking amino acid restriction without the nutritional deficit — extended median lifespan **+9% in male mice** in the 2025 ITP report. That is the concept you're after: the signal without the substrate loss. It's not available or advisable now, but it's the right thing to watch, and it's a better bet than a bacterial enzyme sold as a supplement.

---

## Part 6 — Summary of changes from your original

**Scoring model:** four averaged axes → two multiplied axes (evidence × benefit), with safety as a veto flag and effort as a tag outside the score.

**Promoted:** ApoB and the statin ladder (unranked → 25, top of list) · blood pressure (absent → 20) · cancer screening (absent → 20) · resistance training (undifferentiated "exercise" → 15) · GLP-1 (unranked → 16)

**Demoted:** SGLT2 inhibitors (top-ranked → 4, AVOID while on a GLP-1) · rapamycin (top-ranked → 6, SKIP) · metformin (→ 4, SKIP) · aspirin (listed → 5, AVOID) · taurine (listed → 1, premise retracted) · TRIIM (listed → 1, AVOID)

**Added:** Lp(a) · ApoB (both targets, split) · blood pressure · VO₂max · sleep apnea screening · radon · creatine · fiber · ezetimibe · bempedoic acid · enlicitide · Shingrix · HPV vaccination · hearing protection · injury prevention · alcohol · H. pylori · periodontal care · air quality · nicotine · depression screening · sun protection · hepatitis C · influenza vaccination · social connection · Lp(a)-lowering watch list · hsCRP · APOE/PRS · homocysteine · colchicine (as a documented skip) · Pendulum Glucose Control and pasteurized A. muciniphila (split into separate rows)

**Cut:** ~35 supplement rows with no human outcome data, all offshore gene therapy, EDTA chelation, methylene blue, HBOT, Khavinson peptides, TA-65, methioninase

---

## Caveats

Rapamycin, statins, ezetimibe, PCSK9 inhibitors, SGLT2 inhibitors, metformin, and GLP-1 agonists are all prescription drugs requiring a physician. The interaction analysis above is a prompt for that conversation, not a substitute for it — bring the specific items (especially the SGLT2i + GLP-1 ketoacidosis risk and the rapamycin/training timing conflict) to whoever manages your tirzepatide.

I'm not a physician and this isn't medical advice. The scoring model is a sorting heuristic, not a measurement — the numbers are there to make the ranking's assumptions legible and arguable, not to imply precision.
