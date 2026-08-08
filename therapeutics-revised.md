# Therapeutic Detail Rows — grouped by mechanism

Companion to [anti-aging-inventory-revised.md](anti-aging-inventory-revised.md). This file holds the row-level reasoning for every scored item.

**Format:** `E × B = score` · safety flag · effort tag · access
`E` = evidence (1–5) · `B` = benefit to a healthy 39-year-old US male (1–5) · safety is a veto flag, not a score · effort sits outside the score.

Items are grouped by **mechanism**, not by verdict, so that every way of hitting a given target sits side by side and can be compared on its merits. A few items act on more than one pathway and are cross-referenced rather than duplicated.

**Contents**

1. [Measurement and diagnostics](#1-measurement-and-diagnostics)
2. [ApoB and the lipoprotein pathway](#2-apob-and-the-lipoprotein-pathway)
3. [Incretin and glucose handling](#3-incretin-and-glucose-handling)
4. [AMPK and energy sensing](#4-ampk-and-energy-sensing)
5. [mTOR and nutrient sensing — the anti-growth arm](#5-mtor-and-nutrient-sensing--the-anti-growth-arm)
6. [GH / IGF-1 and anabolism — the pro-growth arm](#6-gh--igf-1-and-anabolism--the-pro-growth-arm)
7. [Cellular senescence](#7-cellular-senescence)
8. [NAD+ metabolism](#8-nad-metabolism)
9. [Redox and hormesis](#9-redox-and-hormesis)
10. [Hemodynamic, vascular and antithrombotic](#10-hemodynamic-vascular-and-antithrombotic)
11. [Inflammation](#11-inflammation)
12. [Immune and infectious](#12-immune-and-infectious)
13. [Neurological, sensory and mental health](#13-neurological-sensory-and-mental-health)
14. [Diet composition](#14-diet-composition)
15. [Environmental and external-cause exposure](#15-environmental-and-external-cause-exposure)
16. [Early detection](#16-early-detection)
17. [No credible mechanism, or unregulated administration](#17-no-credible-mechanism-or-unregulated-administration)

---

## 1. Measurement and diagnostics

These are not therapies. They gate which therapies are even rankable for you, which is why they sit first.

### ApoB
**5 × 5 = 25** · OK · trivial · lab test
**Target:** atherogenic particle count · **Cadence:** annual; q8wk during titration · **Cautions:** none
**Why:** E5 — the input to the single best-evidenced intervention available to you. B5 — ASCVD is the #1 lifetime cause of death for a US male. Treat this number, not LDL-C.

### Home blood pressure series
**5 × 4 = 20** · OK · trivial · device ~$50
**Target:** vascular load · **Cadence:** weekly 7-day averages, AM/PM · **Cautions:** none
**Why:** E5 — SPRINT and dozens of RCTs, hard outcomes. B4 — enormous if elevated, zero if not, so this is a test before it is a therapy. Office readings are noise.

### DEXA body composition
**4 × 4 = 16** · OK · trivial · ~$75
**Target:** lean mass · **Cadence:** 2×/yr while on a GLP-1 · **Cautions:** none
**Why:** E4 — the reference method for lean mass. B4 — the only way to catch GLP-1-driven lean-mass loss early. Segmental BIA (Withings Body Comp) drifts with hydration and will not resolve the 1–2 kg changes that matter. This is also the primary instrument for evaluating a growth-cycling protocol (§6).

### Lp(a), once, lifetime
**4 × 4 = 16** · OK · trivial · lab test ~$30
**Target:** genetic ASCVD + aortic stenosis risk · **Cadence:** once, never repeat
**Cautions:** each Lp(a) particle carries one apoB-100, so a high Lp(a) sets a floor under achievable ApoB
**Why:** E4 — Mendelian randomisation causality is settled; the therapy it would trigger is not yet proven (Lp(a)HORIZON pending). B4 — determines how aggressive the whole ApoB plan should be. Highest information-per-dollar test here.

### Home sleep apnea test
**4 × 4 = 16** · OK · low · Rx, ~$200
**Target:** OSA · **Cadence:** once; repeat if weight shifts · **Cautions:** none
**Why:** E4 — diagnostic accuracy is solid; CPAP RCTs (SAVE, RICCADSA) were neutral for MACE though clearly positive for symptoms and BP. B4 — undiagnosed OSA silently drives hypertension, AF and cognitive decline. Weight trajectory on tirzepatide makes this timely.

### VO₂max
**3 × 4 = 12** · OK · low · ~$150 or estimated
**Target:** cardiorespiratory fitness · **Cadence:** annual · **Cautions:** none
**Why:** E3 — observational only; nobody randomises people to fitness. B4 — the fitness-mortality gradient is among the largest effect sizes in the epidemiological literature. Track this, not minutes trained.

### Vitamin D (25-OH)
**3 × 2 = 6** · OK · trivial · lab test
**Target:** pleiotropic · **Cadence:** once, then as needed · **Cautions:** none
**Why:** E3 — VITAL was largely null for supplementation; correcting frank deficiency has better support. B2 — only matters if you are actually deficient. Test rather than assume.

### hsCRP
**3 × 2 = 6** · OK · trivial · lab ~$15
**Target:** residual inflammatory risk · **Cadence:** annual with ApoB · **Cautions:** none
**Why:** E3 — consistently predictive, but interventions targeting it have a mixed record. B2 — mainly gates the inflammation question (§11): whether residual risk after ApoB control is inflammatory. Cheap enough to add to a draw you are already doing.

### Baseline audiogram
**3 × 2 = 6** · OK · trivial · insurance
**Target:** hearing loss / dementia risk · **Cadence:** once, then q5y · **Cautions:** none
**Why:** E3 — hearing loss is the largest single modifiable dementia risk factor in the Lancet Commission model, but the causal chain rests on cohort data. B2 — at 39 the value is a baseline to detect drift against.

### Grip dynamometer
**3 × 2 = 6** · OK · trivial · ~$30 once
**Target:** whole-body strength proxy · **Cadence:** monthly · **Cautions:** none
**Why:** E3 — observational. B2 — it will not change your outcome by itself, but it is the cheapest early-warning signal for the lean-mass problem GLP-1s create, and the cheapest weekly readout during an anti-growth block.

### APOE genotype / CAD polygenic risk score
**3 × 2 = 6** · OK · low · DTC or clinical
**Target:** genetic risk stratification · **Cadence:** once
**Cautions:** **GINA covers health insurance but NOT life, disability or long-term-care insurance**
**Why:** E3 — APOE4 is robustly predictive; polygenic scores are improving but not yet decision-changing for most people. B2 — at 39 there is little you would do differently that is not already on this list. The real consideration is not medical: secure term life and own-occupation disability coverage **before** testing, because those underwriters can legally use the result, and two young children make that coverage worth more than the information.

### Homocysteine, B12, folate
**2 × 2 = 4** · OK · trivial · lab ~$40
**Target:** one-carbon metabolism · **Cadence:** if pursuing any methionine work, or on metformin · **Cautions:** none
**Why:** E2 — homocysteine-lowering RCTs have not reduced cardiovascular events. B2 — near-zero as a therapy target. Included only because it is the correct biochemical readout if you pursue methionine work (§5), and because metformin depletes B12.

### Coronary artery calcium
**5 × 1 = 5** · OK · low · ~$100 · **DEFER TO 45–50**
**Target:** subclinical atherosclerosis · **Cadence:** revisit at 45–50 · **Cautions:** none
**Why:** E5 for risk stratification. B1 at your age — most 39-year-olds score zero, and zero does not exclude soft plaque, so the result will not change what you do. Earlier only if ApoB or Lp(a) come back high.

---

## 2. ApoB and the lipoprotein pathway

The single highest-yield mechanism family on the list, and the one where you have four distinct molecular targets and a coherent escalation ladder.

**The ladder:** HMG-CoA reductase (statin) → NPC1L1 (ezetimibe) → PCSK9 (four modalities) → apo(a) (not yet available). ACL (bempedoic acid) is a lateral move for statin intolerance, not a rung.

### 2a. Targets

#### ApoB to <60 mg/dL
**5 × 5 = 25** · MONITOR · trivial · statin ± ezetimibe, ~$60/yr
**Why:** E5 — three decades of RCTs with hard outcomes. B5 — ASCVD is the #1 lifetime cause of death and cumulative ApoB exposure is the driver. Mendelian randomisation gives roughly 3× the risk reduction per mmol/L for lifelong versus mid-life lowering. Starting at 39 rather than 55 is the whole argument.

#### ApoB to <30 mg/dL (the increment beyond <60)
**4 × 4 = 16** · MONITOR · high · Rx; needs triple therapy
**Measure:** ApoB q8wk during titration; hsCRP; HbA1c
**Cautions:** requires a PCSK9 inhibitor, which insurance will not cover without ASCVD or FH; Lp(a) sets a hard ApoB floor
**Why:** E4 — no RCT has ever *randomised* anyone to an ultra-low target. Support is post-hoc achieved-level analysis (FOURIER-OLE: monotonic benefit down to LDL-C <20 mg/dL over ~7 years, no excess safety signal) plus genetic evidence from PCSK9 and ANGPTL3 loss-of-function carriers who are healthy at lifelong LDL in the teens. Strong, but a different evidence class than the <60 target. B4 — the increment is real, and cumulative-exposure logic makes it *more* attractive at 39 than at 65, but it is the second slice of a shrinking pie taken from an already-reduced baseline. `high` effort because reaching it costs roughly 100× more per year.

### 2b. HMG-CoA reductase

#### Rosuvastatin or atorvastatin (generic)
**5 × 5 = 25** · MONITOR · trivial · Rx, $4–15/mo
**Measure:** ApoB at 8 weeks; ALT once at baseline
**Cautions:** do not stack with red yeast rice (same molecule); berberine raises exposure via CYP3A4
**Why:** E5 — three decades of RCTs with hard outcomes. B5 — moves a typical 39-year-old from roughly ApoB 100 to roughly 60 for about $60/year, the largest and cheapest increment available anywhere in this document. Hormone-stack reassurance: the 2024 meta-analysis (21 studies, 9,879 patients) found statins lower *total* testosterone by ~13 ng/dL in RCTs, not below the normal range, with no change in *free* testosterone, LH, estradiol or SHBG.

#### Red yeast rice / monacolins
**3 × 2 = 6** · **AVOID** · trivial · OTC
**Cautions:** **unstandardised lovastatin at an unknown dose — do not stack with a statin**
**Why:** E3 — it works, because it is a statin. B2 — same benefit as a prescription statin. AVOID only because the dose is unknown and unregulated. Take the actual statin.

### 2c. NPC1L1 (cholesterol absorption)

#### Ezetimibe (generic)
**4 × 4 = 16** · OK · trivial · Rx, ~$10/mo
**Measure:** ApoB at 8 weeks · **Cautions:** none
**Why:** E4 — IMPROVE-IT showed a real but modest hard-outcome benefit on top of statin. B4 — adds roughly 20% ApoB reduction for pocket change. Best value-per-dollar pairing in the document and absent from the source table entirely.

### 2d. ATP citrate lyase

#### Bempedoic acid
**4 × 4 = 16** · MONITOR · moderate · Rx, ~$400/mo · **only if statin-intolerant**
**Measure:** ApoB; uric acid · **Cautions:** raises uric acid; tendon rupture signal
**Why:** E4 — CLEAR Outcomes showed MACE reduction, but in a statin-intolerant population. B4 — meaningful ApoB reduction. A lateral move, not a rung on the ladder.

### 2e. PCSK9 — four modalities, one target

All four block PCSK9-mediated degradation of the LDL receptor, so LDL receptors recycle instead of being destroyed. Same target, same downstream effect, four delivery routes. They are separated here **only** by how far each has been carried through outcomes trials.

| Agent | Modality | Dosing | E × B | Outcomes trial |
|---|---|---|:---:|---|
| Evolocumab / alirocumab | monoclonal antibody | SC q2wk or q4wk | **5 × 5 = 25** | **Reported** — FOURIER, ODYSSEY |
| Inclisiran | siRNA | SC q6mo after loading | **4 × 5 = 20** | Pending — ORION-4, VICTORION-2P |
| Enlicitide (Lipfendra) | oral macrocyclic peptide | 20 mg daily, oral | **4 × 5 = 20** | Pending — CORALreef Outcomes |

#### Evolocumab / alirocumab
**5 × 5 = 25** · OK · high · Rx, ~$500–600/mo cash
**Measure:** ApoB; Lp(a) · **Cautions:** none known; additive with statin by design
**Why:** E5 — FOURIER and ODYSSEY established hard-outcome benefit. B5 — same target as the statin, deeper. Scores identically to the generic statin because on the merits it is that good; the entire difference is the effort tag and the coverage gate. Prior authorisation generally requires established ASCVD or HeFH, which you do not have.

#### Inclisiran
**4 × 5 = 20** · OK · high · Rx, ~$500–600/mo equivalent
**Measure:** ApoB; Lp(a) · **Cautions:** none known; additive with statin by design
**Why:** E4 — the monoclonals' justification ("FOURIER and ODYSSEY established hard-outcome benefit") does not apply here. Inclisiran was approved on LDL-C lowering alone; ORION-4 and VICTORION-2P have not reported. It sits in the same evidence position as enlicitide, not the same position as the monoclonals. B5 — same target, same depth of LDL receptor recycling. Note that two injections a year is arguably the *lowest* administration burden in this family, oral included; what keeps it at `high` effort is cost and prior authorisation, not logistics.

#### Enlicitide decanoate (Lipfendra), oral
**4 × 5 = 20** · OK · high · Rx, approved 15–16 Jul 2026
**Measure:** ApoB; Lp(a) · **Cautions:** none known
**Why:** E4 — CORALreef Lipids gave 55.8% placebo-adjusted LDL-C reduction (n=2,904) and ~50% ApoB reduction; CORALreef HeFH gave 59.4%; CORALreef AddOn beat ezetimibe, bempedoic acid and their combination on background statin. These are surrogate endpoints and CORALreef Outcomes (>14,500 enrolled) has not reported — but the class prior here is unusually strong. PCSK9-mediated LDL lowering is one of the best-validated surrogates in medicine, and CTT plus Mendelian randomisation show benefit tracking absolute LDL-C reduction largely independent of the mechanism used to achieve it. A two-point penalty against the monoclonals would overstate the uncertainty; one point is right. B5 — removes the injection barrier for the best non-statin target in the family.

### 2f. apo(a) / Lp(a)

#### Lp(a)-lowering therapy (pelacarsen, olpasiran, lepodisiran, muvalaplin)
**2 × 4 = 8** · OK · high · not yet approved · **WATCH**
**Measure:** Lp(a) once · **Cautions:** none
**Why:** E2 — no outcomes data yet for any agent in the class. B4 — if Lp(a) is elevated it is your single largest unaddressed genetic risk, and nothing currently available lowers it much. Lp(a)HORIZON (pelacarsen, n=8,323) is the first CV outcomes trial for the class and is expected to report before the end of 2026. This row exists so the readout finds you already knowing your number.

---

## 3. Incretin and glucose handling

### 3a. GLP-1 / GIP receptor agonism

#### Tirzepatide
**4 × 4 = 16** · MONITOR · moderate · Rx · **CONTINUE**
**Measure:** DEXA lean mass; HbA1c; ApoB
**Cautions:** **euglycemic ketoacidosis if combined with an SGLT2 inhibitor**; hold before anesthesia; interacts with low-protein protocols
**Why:** E4 — SELECT showed ~20% MACE reduction with semaglutide in non-diabetic overweight adults; for tirzepatide specifically the hard-outcome trial (SURMOUNT-MMO) has not reported. B4 — the best-evidenced pharmacological item in your stack. Pair with protein and lifting or the lean-mass cost is real. This is the item that most constrains everything else on the list.

### 3b. SGLT2 inhibition

#### Canagliflozin / empagliflozin
**2 × 2 = 4** · **AVOID** while on a GLP-1 · low · Rx · **revisit if T2D / CKD / HF**
**Measure:** ketones; volume status; genital exam
**Cautions:** **SEVERE — with a GLP-1 plus any carbohydrate restriction or fasting → euglycemic ketoacidosis, documented in non-diabetics; glucose reads normal so it is routinely missed**
**Why:** E2 — ITP gave +14% median lifespan in **males only** for canagliflozin, and every human outcome trial (EMPA-REG, CANVAS, DECLARE, DAPA-HF, EMPEROR, DAPA-CKD, EMPA-KIDNEY) is in T2D, HF or CKD where much of the benefit is hemodynamic and renal. B2 — no trial exists in metabolically healthy non-diabetics. The source table ranked this #1 on a 12/12 gerotherapeutics score, but that score means "most deserves a trial," which entails that the human aging evidence does not exist.

**The AVOID flag is driven by the tirzepatide interaction, not by the drug.** That distinction is exactly what a flag can express and an averaged safety score cannot. Costs in isolation: genital mycotic infection in roughly 1 in 10 men, volume depletion and orthostasis, 20–40 g/day glucosuria, Fournier's gangrene (rare, labeled), and euglycemic ketoacidosis. There is also a redundancy argument — the metabolic benefit you would be reaching for, tirzepatide already delivers with human hard-outcome data behind it.

**This flag does not relax during an anti-growth block.** A fasting or carbohydrate-restricted phase is the *worst* time to add an SGLT2 inhibitor, not a neutral one. If growth cycling is adopted, this row stays AVOID throughout.

### 3c. Microbiome → SCFA → endogenous GLP-1

#### Pasteurized *A. muciniphila* (MucT)
**3 × 3 = 9** · OK · moderate · OTC, sold separately from Pendulum · **WATCH — act if you come off tirzepatide**
**Target:** Amuc_1100 surface protein; gut barrier; insulin sensitivity
**Measure:** weight and DEXA during and after GLP-1 taper; baseline *Akkermansia* abundance if testing
**Cautions:** different preparation from Pendulum's — pasteurized single strain, not a live multi-strain blend
**Why:** E3 — three independent RCTs now, with academic rather than in-house leadership. Mount et al., *Nature Medicine*, June 2026 (n=90, Maastricht/Copenhagen): after an 8-week low-energy diet, 24 weeks of pasteurized MucT gave 1.2 ± 0.7 kg regain versus 3.2 ± 0.4 kg on placebo (P=0.012); net weight loss from baseline 3.1 kg greater (P=0.009); ~40% of the MucT group kept losing weight versus ~5% on placebo; no serious treatment-related adverse events. Depommier 2019 (*Nature Medicine*, n=32) and Zhang 2025 (*Cell Metabolism*) point the same direction. B3 — weight regain after weight loss is the single unsolved problem for anyone on a GLP-1, and this is the only supplement on the entire inventory with a positive RCT aimed at it.

Held at 3×3 rather than higher for three reasons: the effect is ~2 kg over 24 weeks; the weight loss was diet-induced rather than GLP-1-induced, so applying it is an extrapolation; and both Zhang and Mount found the benefit concentrates in people with **low baseline *Akkermansia***, making it responder-dependent with no validated consumer test for responder status.

#### Pendulum Glucose Control (WBF-011)
**2 × 2 = 4** · OK · moderate · OTC subscription, ~$150–200/mo · **SKIP for its stated indication**
*(A. muciniphila, C. butyricum, C. beijerinckii, A. hallii, B. infantis + chicory-root inulin)*
**Measure:** HbA1c; fasting insulin; CGM postprandial excursions if curious
**Cautions:** the chicory-root inulin is a fermentable prebiotic — stacked on tirzepatide-delayed gastric emptying it will likely worsen bloating and gas
**Why:** E2 — one RCT (Perraudeau 2020, *BMJ Open Diabetes Res Care*, NCT03893422): randomised, double-blind, placebo-controlled, 12 weeks, T2D on metformin ± sulfonylurea, HbA1c −0.6% and postprandial glucose AUC −33%. Genuinely better than what backs almost anything else in the supplement section. But the active arm was n=23 against n=26 placebo out of 76 randomised across three arms; **all seventeen authors were Pendulum employees**; the paper describes itself as proof-of-concept; and six years on there is still no independent replication — the one planned academic study (USC, NCT04228003) was withdrawn before enrolling anyone, "the funding and project never started." The 2022 *BMC Microbiology* follow-up showing circulating butyrate and ursodeoxycholate rose is mechanistically supportive but from the same group.

B2 — the indication mismatch is the larger problem. The studied population was T2D on metformin. You are on tirzepatide, which lowers HbA1c by roughly 2.0–2.4%. This is a 0.6% agent whose proposed mechanism, SCFA-driven **endogenous** GLP-1 secretion, is precisely the pathway your drug already saturates pharmacologically. Nobody has tested it on top of a GLP-1.

---

## 4. AMPK and energy sensing

The energy-sensor arm of the anti-growth side. AMPK activation opposes mTORC1, so everything here belongs in the same phase as §5 and out of phase with §6.

Worth stating up front: **exercise is the best-evidenced AMPK activator on this list, and it is free.** Every pharmacological entry in this section is competing against training, and losing.

#### Metformin
**2 × 2 = 4** · MONITOR · trivial · Rx · **SKIP**
**Target:** AMPK, complex I · **Measure:** HbA1c; B12 annually
**Cautions:** blunts exercise VO₂max and mitochondrial adaptation — see §Interactions, phase conflicts
**Why:** E2 — TAME remains unfunded; diabetes RCTs do not transfer to a normoglycemic 39-year-old. B2 — speculative. It competes with cardiorespiratory training, which scores 20 against its 4, for the same adaptation.

The training interaction is a **timing** problem rather than a permanent exclusion — see [growth cycling](anti-aging-inventory-revised.md#part-4--growth-cycling). Metformin's short half-life (~6 h) makes it the easiest item on the entire list to phase cleanly. That improves its schedulability without improving its evidence, so it still scores 4.

#### Berberine
**2 × 1 = 2** · **AVOID** · trivial · OTC · **SKIP**
**Target:** AMPK · **Measure:** HbA1c
**Cautions:** **potent CYP3A4 / P-gp inhibitor — raises statin, rapamycin and tadalafil exposure unpredictably**
**Why:** E2 — rodent and small human data. B1 — nothing a statin does not do better. AVOID because the interaction liability is real and it buys you nothing. This flag is pharmacokinetic and does not relax in any phase.

---

## 5. mTOR and nutrient sensing — the anti-growth arm

Everything in this section pushes the same direction: down-regulate mTORC1 and IGF-1 signalling, favour autophagy and catabolic housekeeping, reduce the substrate available for anabolic error.

**These items are not permanently incompatible with §6.** They are incompatible *simultaneously*. See [Part 4 of the main document](anti-aging-inventory-revised.md#part-4--growth-cycling) for the block-cycling structure that separates them in time; the scores below reflect each item on its own merits regardless of scheduling.

#### Rapamycin 5–6 mg weekly
**2 × 3 = 6** · MONITOR · low · Rx · **SKIP for now**
**Target:** mTORC1 · **Measure:** lipids; glucose; CBC; mouth ulcers; wound healing before any surgery
**Cautions:** blocks contraction-induced muscle protein synthesis; t½ ~62 h; berberine and quercetin raise exposure
**Why:** E2 — the best animal lifespan data of any molecule, but PEARL, the only RCT in normative aging, **missed its primary endpoint**, and its one significant efficacy finding was lean mass in **women** at 10 mg (n=114, ages 50–85). B3 — real if it translates. For a 39-year-old man PEARL establishes safety and little else.

**On the training interaction:** a single oral dose before resistance exercise completely blocked the contraction-induced rise in human muscle protein synthesis (~40% in controls), with S6K1 phosphorylation flat versus a 6-fold rise in controls. Rapamycin did *not* affect post-absorptive protein metabolism — it specifically suppresses the *response to a stimulus*. With a ~62 h half-life, weekly dosing does not cleanly separate from a 3×/week lifting schedule; ~13 days is five half-lives. That is an argument for **block scheduling rather than weekly dosing**, not an argument that the two can never coexist. Bitto 2016 (*eLife*) found transient 3-month rapamycin in middle-aged mice produced persistent lifespan benefit, which is the pharmacological precedent for pulsed use.

Score stays at 6 because the human evidence is what it is. If you run growth cycling, rapamycin belongs entirely inside the anti-growth block, dosed at its start, with the last dose ≥2 weeks before a pro-growth block opens.

#### Time-restricted feeding / periodic fasting-mimicking diet
**2 × 2 = 4** · OK · low · free
**Target:** amino acid response, FGF21, autophagy · **Measure:** FGF21; IGF-1; weight
**Cautions:** **ketoacidosis risk if combined with an SGLT2 inhibitor**
**Why:** E2 — human trials exist but measure surrogates over short horizons. B2 — modest. Listed mainly because it is the human-data version of the FGF21 signal you are chasing with methionine restriction, at a fraction of the risk.

**This is the item that most directly supports your cycling hypothesis**, and it is worth more attention than its score implies. FMD is *already* a cycle protocol: Longo's design is 5 days on, then refeeding, a few times a year. The refeeding phase is not downtime — in mice, fasting/refeeding cycles drove hematopoietic stem cell self-renewal and immune reconstitution (Cheng et al., *Cell Stem Cell*, 2014), which is the same regenerative endpoint TRIIM-X targets by a much more expensive and much less evidenced route. If you want a pro/anti-growth alternation with actual human trial infrastructure behind it, this is the cheap version.

#### Methionine reduction via food choice (protein held constant)
**2 × 2 = 4** · OK · low · food
**Target:** SAM/SAH, FGF21, IGF-1 · **Measure:** DEXA lean mass; plasma methionine; homocysteine
**Cautions:** cancelled by NAC/GlyNAC; do not combine with total protein restriction on a GLP-1
**Why:** E2 — rodent lifespan data is solid, human data is short-term and surrogate-only. B2 — plausible but unproven. This is the **safe version** of the proposed protocol: shift sources toward legumes, soy and dairy, which cut methionine 25–40% while total protein stays flat.

#### Methionine restriction <1 g/day, 5 days/week
**1 × 1 = 1** · **AVOID as specified** · moderate · food + supplement
**Target:** SAM/SAH, FGF21, IGF-1 · **Measure:** DEXA lean mass; grip
**Cautions:** compounds GLP-1 lean-mass loss; cancelled by NAC/GlyNAC
**Why:** E1 — Fanti, Longo et al. (*Cell Metabolism*, June 2026) found a low-protein diet **supplemented** with methionine reduced frailty without lean-mass loss; too little methionine caused frailty, too much abolished the benefit. B1 — this protocol aims at the frailty arm of that curve. Methionine is the initiator amino acid for all translation, so pushing it below requirement constrains protein synthesis globally rather than selectively throttling mTOR. The 5-on/2-off structure collects the muscle-loss debit reliably and the metabolic credit unreliably, because the rodent phenotype develops over days to weeks of sustained restriction.

The **scheduling** objection to the original design — restriction landing on the 48–72 h window when weekend training is still remodelling — is the one problem that block cycling actually fixes. See §5 of the main document. The other seven objections stand on their own.

#### Methioninase (oral rMETase)
**1 × 1 = 1** · **AVOID** · moderate · direct order only
**Target:** methionine degradation · **Measure:** plasma methionine
**Cautions:** cancels with NAC/GlyNAC; compounds GLP-1 lean-mass loss
**Why:** E1 — human oral evidence is **two case reports** in advanced cancer, from essentially one lab (Hoffman / AntiCancer Inc.) over thirty years. B1 — no plausible benefit at 39. It is a bacterial enzyme from *Pseudomonas putida*; the injectable form was strongly immunogenic in primates, requiring PEGylation, and caused reduced food intake, weight loss and transient hemoglobin decline. Sold as a "dietary supplement," which is a regulatory classification rather than a safety finding. Produces methanethiol (the principal compound behind severe oral and body malodor), α-ketobutyrate and ammonia, and requires co-administered pyridoxal-5′-phosphate. Functionally redundant: food selection achieves the same exposure reduction with a titration dial, a food log, an off switch and no immunogenic bacterial protein. Long-term safety data in healthy people is **absent**, not weak.

**This AVOID does not soften under any phase structure.** It is the one item in this section whose problem is the agent itself rather than its timing.

---

## 6. GH / IGF-1 and anabolism — the pro-growth arm

The counterweight to §5. Muscle and bone maintenance, tissue repair, immune reconstitution, and wound healing all require anabolic signalling, and a protocol that suppresses it continuously is buying protection from one set of failure modes with exposure to another.

**Framing note:** this section is not in permanent opposition to §5. The opposition is real *at any given moment* and dissolves when the two are separated in time — which is how several of these interventions were designed to be used in the first place. What follows scores each item on its own merits; the scheduling argument lives in [Part 4](anti-aging-inventory-revised.md#part-4--growth-cycling).

#### Resistance training 2–3×/week
**3 × 5 = 15** · OK · moderate · free
**Target:** mTORC1, myonuclear addition, bone loading · **Measure:** DEXA lean mass; grip strength
**Cautions:** rapamycin blocks contraction-induced MPS; methionine restriction removes the substrate
**Why:** E3 — RCTs are consistent but measure surrogates (strength, lean mass, function) rather than mortality. B5 — non-negotiable on a GLP-1, because it is the only thing that reliably protects the lean mass the drug puts at risk.

**This is the pro-growth phase.** Whatever else growth cycling includes, training plus protein is the component with real evidence behind it, and it is free. Note also that **maintenance requires far less volume than accumulation** — trained individuals hold strength and lean mass on roughly one-third of accumulation volume for months (Bickel 2011). A reduced-volume block during an anti-growth phase is physiologically defensible in a way that a full detraining block is not.

#### Protein 1.2–1.6 g/kg/day, distributed
**3 × 4 = 12** · OK · trivial · food
**Target:** muscle protein synthesis · **Measure:** DEXA lean mass; grip
**Cautions:** conflicts with the proposed methionine restriction protocol as originally specified
**Why:** E3 — RCTs are consistent but measure lean mass and strength, not mortality. B4 — on a GLP-1 this is the difference between losing fat and losing muscle. Distribution across meals beats bolus loading, and muscle protein synthesis has a per-meal ceiling and refractory period, so a week's intake cannot be banked into a weekend.

#### Creatine monohydrate 5 g/day
**3 × 3 = 9** · OK · trivial · OTC, ~$30/yr
**Target:** phosphocreatine, cell hydration · **Measure:** DEXA; grip; strength log · **Cautions:** none
**Why:** E3 — hundreds of RCTs, but on strength and lean mass rather than hard outcomes. B3 — modest alone, more valuable here because it directly counteracts GLP-1 lean-mass loss. The most conspicuous omission from the 128-row source list. Unflavored monohydrate only.

#### Block-periodized growth cycling (training-led, no rhGH)
**2 × 3 = 6** · OK · moderate · free
**Target:** phase separation of mTORC1/IGF-1 signalling · **Measure:** DEXA at each phase boundary; grip weekly; IGF-1; fasting insulin; ApoB
**Cautions:** SGLT2i AVOID does not relax in either phase; do not compress the washout between blocks
**Why:** E2 — no human trial has tested block alternation of pro- and anti-growth interventions against either arm run continuously. The supporting logic is mechanistic plus indirect: FMD is already a cycle protocol with human trial infrastructure; fasting/refeeding cycles drove HSC self-renewal in mice (Cheng 2014); transient rapamycin produced persistent benefit in mice (Bitto 2016); and exercise periodization is the same idea in a domain where it is uncontroversial. B3 — the realistic benefit is not additive lifespan but **avoided cost**: it recovers the muscle, bone and repair capacity that a continuously anti-growth protocol gives up, at no drug expense.

Scored at 6 rather than higher because it is a *scheduling structure*, not a therapy — most of its value is already counted in the rows it schedules. Scored at 6 rather than lower because it converts three of the phase conflicts in Part 3 from exclusions into calendar entries, which is a real gain.

#### rhGH-containing pro-growth block (TRIIM / TRIIM-X style)
**1 × 2 = 2** · MONITOR · high · trial is ages 40–80; you are 39
*(rhGH + DHEA + metformin)*
**Target:** thymus regeneration · **Measure:** thymic MRI; epigenetic clocks; IGF-1; fasting glucose; PSA
**Cautions:** raises IGF-1 supraphysiologically; the metformin in the cocktail exists to offset GH-induced insulin resistance the protocol itself creates
**Why:** E1 — original TRIIM was n=9, single-arm, **uncontrolled**, with ~2.5 years of epigenetic age reversal measured by clocks that are not validated mortality surrogates. Seven years on, no peer-reviewed TRIIM-X results exist; the only public data is a preliminary "sneak peek" from a Foresight Institute talk in May 2026. The trial is participant-funded and sponsor-run, which is a structurally weak evidence generator regardless of the underlying biology. B2 — thymic involution at 39 is modest and the immunosenescence rationale is built on 65-year-olds.

**MONITOR rather than AVOID.** The strongest case for an AVOID would rest on "directly opposes rapamycin, methionine restriction and every CR mimetic on this list" — which is a *simultaneity* argument, and block cycling answers it. Setting that aside leaves two concerns, both real and both MONITOR-grade rather than AVOID-grade: the evidence base is a single uncontrolled n=9 study, and exogenous rhGH raises IGF-1 into a range that training and protein do not, where the epidemiology associates elevated IGF-1 with increased prostate, colorectal and breast cancer risk.

That second point is worth stating precisely, because it is the crux of your hypothesis. **The cumulative-exposure argument cuts in your favour here.** If IGF-1 risk is a function of the integral of exposure over time, then two six-week blocks a year is roughly a 23% duty cycle, and the lifetime integral is far below continuous administration. That is a genuine and correct softening of the objection. What it does not do is create evidence that the protocol works — the pruning-then-rebuilding logic is attractive, and it is still a hypothesis.

**Practical position:** the thymic-regeneration goal is the interesting part, and rhGH is the weakest available route to it. You become eligible for NCT04375657 at 40, which is next year; if you want the trial, the honest reason to enroll is contributing data, not receiving treatment. Meanwhile FMD cycles target overlapping regenerative biology with better evidence and no drug cost.

#### Testosterone (absent hypogonadism)
**4 × 1 = 4** · MONITOR · moderate · Rx · **SKIP**
**Target:** androgen receptor · **Measure:** total and free T; SHBG; hematocrit; PSA
**Cautions:** raises hematocrit; suppresses fertility
**Why:** E4 — TRAVERSE established cardiovascular safety and, importantly, showed **no benefit in men who are not hypogonadal**. B1 — no route to changing your outcomes if your levels are normal. The score is low by design: the evidence is good and it says do not do this. This does not change under a cycling structure — an intervention with no benefit does not acquire one by being scheduled well.

---

## 7. Cellular senescence

#### Dasatinib + quercetin (D+Q)
**1 × 1 = 1** · MONITOR · moderate · Rx (D) · **SKIP**
**Target:** senolytic · **Measure:** none widely available
**Cautions:** quercetin inhibits CYP3A4 and raises dasatinib exposure — the protocol pairs them deliberately, but the interaction is real regardless
**Why:** E1 — no human outcome data. B1 — senescent-cell burden at 39 is low, so there is little to clear. Right idea, wrong decade. Revisit at 60.

#### Fisetin
**1 × 1 = 1** · OK · trivial · OTC · **SKIP**
**Target:** senolytic · **Measure:** none available · **Cautions:** none
**Why:** E1 — ITP result was null (−5 to +7%). B1 — no human outcome data. Mayo trials ongoing, none positive yet.

**On senolytics and cycling:** senolytics are already conceived as intermittent — hit-and-run dosing, weeks apart, because senescent cells take time to reaccumulate. If you ever run growth cycling, senolytics belong at the *end* of the anti-growth block, immediately before the regenerative phase, which is the sequence the underlying biology suggests: clear, then rebuild. That is a sensible design and it does not make either drug worth taking at 39.

---

## 8. NAD+ metabolism

#### NMN / NR
**2 × 1 = 2** · OK · moderate · OTC · **SKIP**
**Target:** NAD+ · **Measure:** none reliable · **Cautions:** redundant with niacin
**Why:** E2 — NR gave +5% in ITP; human trials raise NAD+ without downstream functional benefit. B1 — nothing measurable has followed the biochemistry. Expensive for the score. Three rows in the source table (NMN, NR, niacin) for one pathway; pick one or none.

---

## 9. Redox and hormesis

The organizing principle for this whole section: **the ROS burst after training is signal, not damage.** Suppressing it suppresses the adaptation. That makes every item here a timing question rather than a yes/no question.

#### Astaxanthin
**2 × 1 = 2** · OK · trivial · OTC · **SKIP**
**Target:** antioxidant · **Cautions:** blunts exercise adaptation
**Why:** E2 — an ITP hit (+12%) that **failed to replicate** at a different dose and start age in the April 2026 ITP report. B1 — no human outcome data. The replication failure is the point: it is why the rodent-lifespan column in the source table cannot be trusted.

#### NAC / GlyNAC / glutathione
**2 × 1 = 2** · OK · low · OTC · **SKIP**
**Target:** glutathione precursor
**Cautions:** **cysteine reverses essentially all metabolic effects of methionine restriction (Elshorbagy)**; blunts exercise adaptation
**Why:** E2 — small human trials on surrogates. B1 — no demonstrated outcome benefit in a healthy 39-year-old. Three separate rows in the source for one mechanism.

The methionine interaction is a genuine cancellation rather than a timing issue: cysteine supplementation reverses the entire metabolic phenotype of MR in rodents — adiposity, hepatic SCD1, insulin, leptin, triglycerides, adiponectin all revert to control. Elshorbagy's conclusion was that the anti-obesity effect of MR is driven by **low cysteine**, not low methionine per se. If you run methionine work in any form, NAC and GlyNAC come out.

#### Omega-3 (EPA/DHA)
**3 × 2 = 6** · OK · trivial · OTC · **CONTINUE**
**Target:** membrane, inflammation, triglycerides · **Measure:** omega-3 index
**Cautions:** additive bleeding with aspirin or nattokinase; AF signal at high dose
**Why:** E3 — VITAL, REDUCE-IT and STRENGTH give a mixed and dose-dependent picture. B2 — small. Already in your stack, no reason to stop, no reason to escalate the dose.

#### Sauna 3–4×/week
**2 × 2 = 4** · OK · moderate · varies · **OPTIONAL**
**Target:** heat shock proteins, vascular function · **Cautions:** none
**Why:** E2 — the Finnish cohort data is suggestive and heavily confounded by who uses saunas; no RCT. B2 — fine if you enjoy it, which is a legitimate reason.

---

## 10. Hemodynamic, vascular and antithrombotic

#### Blood pressure to <120 systolic
**5 × 4 = 20** · MONITOR · trivial · lifestyle; Rx generics if needed
**Target:** vascular load · **Measure:** home BP series; potassium and creatinine if on a drug · **Cautions:** none
**Why:** E5 — SPRINT plus dozens of RCTs with hard outcomes. B4 — enormous if you are hypertensive, near-zero if you are not, which is why the home cuff comes first. Absent from the source table entirely, which is its largest single omission.

#### Cardiorespiratory fitness training
**4 × 5 = 20** · OK · moderate · free
**Target:** mitochondrial biogenesis, vascular function, metabolic flexibility · **Measure:** VO₂max annually
**Cautions:** rapamycin and metformin blunt training adaptation; high-dose antioxidants blunt the hormetic signal
**Why:** E4 — RCTs with hard outcomes exist in cardiac and HF populations, plus an enormous consistent cohort literature in healthy adults. B5 — moves the #1 cause of death and the dementia risk curve simultaneously. Zone 2 ~3 h/wk plus 1–2 VO₂max intervals.

Note that this is the item the pharmacological AMPK activators (§4) are competing with, and it wins on every axis: better evidence, larger effect, no cost, no interactions.

#### Aspirin
**5 × 1 = 5** · **AVOID** · trivial · OTC
**Target:** COX-1 · **Cautions:** additive bleeding with fish oil or nattokinase
**Why:** E5 — extremely well studied. B1 — and the evidence says it does not help you. ASPREE showed net harm in healthy older adults and there is no primary-prevention indication at 39 without established risk. A high evidence score attached to a finding of no benefit.

---

## 11. Inflammation

#### Low-dose colchicine (Lodoco 0.5 mg)
**2 × 1 = 2** · MONITOR · low · Rx · **SKIP**
**Target:** IL-1β / NLRP3 · **Measure:** hsCRP; renal function
**Cautions:** interacts with CYP3A4 and P-gp inhibitors, including berberine and grapefruit
**Why:** E2 — COLCOT and LoDoCo2 were positive, but CLEAR SYNERGY/OASIS-9 (7,062 patients, ~3 years) was **neutral** (HR 0.99), and LoDoCo2 and COPS showed numerically higher non-cardiovascular death. Guidelines sit at class 2b. B1 — every trial is secondary prevention in established ASCVD; there is no primary-prevention indication at 39. A genuine geroscience-adjacent candidate missing from the source table, and the honest answer is still no.

#### Dental / periodontal care
**2 × 2 = 4** · OK · low · insurance
**Target:** *P. gingivalis*, systemic inflammation · **Measure:** periodontal exam 2×/yr · **Cautions:** none
**Why:** E2 — the CVD and dementia links are observational; intervention trials show surrogate improvement only. B2 — modest. You would do this anyway; it scores low because the *aging* claim is weak, not because dental care is optional.

---

## 12. Immune and infectious

#### Shingrix (recombinant zoster vaccine)
**3 × 4 = 12** · OK · low · Rx, age 50+ · **CALENDAR ITEM — not eligible at 39**
**Target:** VZV reactivation; possible off-target immune effects · **Cautions:** none
**Why:** E3 — the zoster efficacy RCTs are excellent, but the dementia finding rests on natural experiments (Wales, Australia, Canada) and cohort data, not an RCT. B4 — ~20–51% dementia risk reduction and ~23% lower CV events if it holds. Strongest new geroprotective signal in two years.

#### H. pylori stool antigen (test and treat)
**4 × 2 = 8** · OK · trivial · lab ~$60
**Target:** gastric cancer · **Cadence:** once, lifetime · **Cautions:** none
**Why:** E4 — test-and-treat RCTs reduce gastric cancer incidence, though mostly in high-incidence populations. B2 — US absolute risk is low. Scores modestly, but the effort is one stool sample and the cure is permanent.

#### Hepatitis C: one-time screening
**4 × 2 = 8** · OK · trivial · insurance
**Target:** chronic HCV, cirrhosis, HCC · **Cadence:** once, lifetime · **Cautions:** none
**Why:** E4 — USPSTF recommends one-time screening for all adults 18–79; direct-acting antivirals are curative in >95%. B2 — low prevalence, but the asymmetry is unusual: a single blood draw that can prevent cirrhosis and liver cancer outright.

#### Influenza vaccination, annual
**4 × 2 = 8** · OK · trivial · insurance
**Target:** infection; possible off-target CV benefit · **Cautions:** none
**Why:** E4 — efficacy RCTs are solid, and post-MI trials (IAMI) showed reduced all-cause death, hinting at cardiovascular benefit beyond infection itself. B2 — modest for a healthy 39-year-old. Belongs on the list mainly because the vaccine-and-dementia literature that makes Shingrix interesting is not obviously zoster-specific.

#### HPV vaccination
**4 × 2 = 8** · OK · low · Rx, approved through 45
**Target:** oncogenic HPV · **Cautions:** none
**Why:** E4 — RCTs on cancer-precursor endpoints plus registry data on cancer incidence. B2 — at 39 you have likely already been exposed, so residual benefit is modest. Scores low, but the window shuts at 45 and rising male oropharyngeal cancer makes it a reasonable cheap bet.

---

## 13. Neurological, sensory and mental health

#### Sleep 7–9 h
**3 × 5 = 15** · OK · trivial · free
**Target:** circadian, glymphatic, metabolic · **Measure:** tracker; HSAT if apnea suspected · **Cautions:** none
**Why:** E3 — strong and consistent observational plus Mendelian randomisation, but sleep-extension RCTs with hard outcomes do not exist. B5 — nothing else on this list works properly if this is broken. Reallocated time, not extra time.

#### Depression screening and treatment access
**4 × 4 = 16** · OK · trivial · insurance
**Target:** mood, suicide risk · **Measure:** PHQ-9 annually · **Cautions:** none
**Why:** E4 — screening plus access to treatment reduces morbidity, and treatment RCTs are solid. B4 — suicide is among the leading causes of death for US males aged 35–44, alongside unintentional injury. Its absence from every longevity list is the same blind spot that omits seatbelts: these lists optimise for the diseases of the old while ignoring what actually kills men in their forties.

#### Hearing protection
**3 × 3 = 9** · OK · trivial · ~$30
**Target:** dementia risk via hearing loss · **Measure:** audiogram q5y · **Cautions:** none
**Why:** E3 — rests on the hearing-loss-to-dementia cohort literature. B3 — the loss is irreversible, which is what makes cheap prevention worth it. Range, power tools, mowing, concerts.

#### Social connection
**3 × 3 = 9** · OK · low · free
**Target:** stress, behaviour, inflammation · **Cautions:** none
**Why:** E3 — observational only, but meta-analytic effect sizes for social isolation are in the same range as major behavioural risk factors. B3 — real and diffuse. The source table ranks the Ornish program at 11/11 pathways partly *because* it includes social support, so the mechanism is already implicitly in the document, just not as a row you could act on.

---

## 14. Diet composition

#### Fiber 35–40 g/day
**3 × 3 = 9** · OK · trivial · food
**Target:** microbiome, lipids, glycemia · **Measure:** intake log · **Cautions:** none
**Why:** E3 — large consistent cohorts plus RCTs on surrogates. B3 — among the strongest single diet-mortality signals in the literature. Absent from the source table.

#### Alcohol minimal or none
**4 × 3 = 12** · OK · trivial · free
**Target:** carcinogen exposure, sleep, BP · **Measure:** intake log; GGT · **Cautions:** none
**Why:** E4 — Mendelian randomisation has essentially dismantled the J-curve; the apparent benefit of moderate drinking was confounding. B3 — real but diffuse: cancer, sleep quality, blood pressure. Absent from the source document entirely.

*Protein and methionine source selection appear under [§5](#5-mtor-and-nutrient-sensing--the-anti-growth-arm) and [§6](#6-gh--igf-1-and-anabolism--the-pro-growth-arm).*

---

## 15. Environmental and external-cause exposure

#### Nicotine and tobacco: none
**5 × 5 = 25** · OK · trivial · free · **CONFIRM**
**Target:** carcinogen, endothelial, thrombotic · **Cautions:** none
**Why:** E5 × B5 — the single highest-value item in all of preventive medicine, conditional on being a user. Listed for completeness: a competing-risk inventory that omits it is not an inventory. Nicotine pouches are not a free pass — the cardiovascular and oral-mucosal exposures are real even without combustion.

#### Injury prevention
**4 × 4 = 16** · OK · trivial · free
**Target:** external-cause mortality · **Cautions:** none
**Why:** E4 — natural-experiment and case-control evidence for seatbelts, helmets and safe storage is overwhelming even without RCTs. B4 — unintentional injury is a leading cause of death for US males aged 35–44 *right now*. Absent from every longevity list including the source.

#### Radon test (home)
**4 × 3 = 12** · OK · trivial · ~$15 kit
**Target:** lung cancer · **Cadence:** once; retest after mitigation · **Cautions:** none
**Why:** E4 — consistent dose-response across miner cohorts and pooled residential analyses; no RCT is possible. B3 — for a never-smoker, mitigation removes roughly 1% absolute lifetime risk. Cook County is EPA Radon Zone 1.

#### Sun protection / UV avoidance
**4 × 2 = 8** · OK · trivial · ~$40/yr
**Target:** UV-induced DNA damage · **Measure:** annual skin exam · **Cautions:** none
**Why:** E4 — RCTs show reduced melanoma and squamous cell carcinoma incidence with regular sunscreen use. B2 — modest in mortality terms for a suburban Midwesterner, but skin cancer is the most common cancer and prevention is nearly free. The source table had "sun exposure" as a *positive* row with no mention of the downside.

#### Bedroom HEPA / PM2.5 awareness
**3 × 2 = 6** · OK · trivial · ~$150
**Target:** particulate exposure · **Measure:** PM2.5 monitor · **Cautions:** none
**Why:** E3 — air pollution epidemiology is strong; the specific benefit of consumer HEPA is inferred. B2 — small absolute effect at US suburban exposure levels. Cheap enough to do anyway.

---

## 16. Early detection

#### Cancer screening on schedule
**5 × 4 = 20** · OK · low · insurance
**Target:** early detection · **Cadence:** colonoscopy at 45; skin annually · **Cautions:** none
**Why:** E5 — sigmoidoscopy and FIT RCTs show mortality reduction; NordICC was intention-to-treat disappointing but per-protocol positive. B4 — cancer is the #2 lifetime cause. Mostly a calendar problem, not a decision problem.

---

## 17. No credible mechanism, or unregulated administration

#### Taurine
**1 × 1 = 1** · OK · trivial · OTC · **SKIP**
**Why:** E1 — **premise retracted.** Fernandez et al., *Science* 2025: longitudinal data across three human cohorts, rhesus monkeys and mice show taurine **rises or holds steady** with age, with interindividual variation exceeding any age effect. B1 — the rationale for supplementing it has been removed.

#### Resveratrol
**1 × 1 = 1** · OK · trivial · OTC · **SKIP**
**Why:** E1 — failed ITP, poor bioavailability, and the sirtuin mechanism itself is disputed. B1 — none. The Sinclair-era case has not held.

#### 17-alpha estradiol
**2 × 1 = 2** · MONITOR · low · not practically available · **WATCH, do not take**
**Why:** E2 — a male-specific ITP hit (+19%), genuinely one of the more interesting results in the field. B1 — zero human data.

#### Blood donation 2–3×/yr
**2 × 2 = 4** · OK · low · free · **OPTIONAL**
**Target:** iron, hemodilution · **Measure:** ferritin; hematocrit · **Cautions:** none
**Why:** E2 — observational only. B2 — weak in isolation. Jumps sharply in value if you ever start TRT, where it is the standard erythrocytosis management tool.

#### Methylene blue
**1 × 1 = 1** · **AVOID** · trivial · Rx
**Target:** mitochondrial electron carrier
**Cautions:** **potent MAO-A inhibitor — serotonin syndrome with any SSRI, SNRI or triptan**
**Why:** E1 — no human aging data. B1 — none. AVOID for the interaction alone: this is a hospitalisation-grade risk, not a caution. It is also the clearest illustration of why safety is a veto flag rather than an averaged term — the drug is cheap and quick to take, so any scoring that averages safety against cost dilutes a hospitalisation risk into a middling number.

#### Bisphosphonates, acipimox, pentoxifylline, azithromycin, piperlongumine, ACE-i/ARB, beta blockers
**1 × 1 = 1** · MONITOR · low · Rx · **change the trigger from "aging" to "diagnosis"**
**Why:** E1 for an *aging* indication — these have good evidence for the diseases they treat and none for healthy 39-year-olds. B1 — no route to benefit absent the diagnosis. Keep the rows, change the trigger condition.

#### Supplement bundle
**1 × 1 = 1** · OK · moderate · OTC · **SKIP**
*(AKG, spermidine, urolithin A, ergothioneine, apigenin, carnosine, lithium, C15:0, MitoQ, CoQ10, green tea extract, curcumin, ginger, ashwagandha, melatonin, generic multi-strain probiotics, butyrate, nattokinase, glucosamine, chondroitin, TA-65, Khavinson peptides, plasmalogens, GLYLO)*
**Cautions:** several blunt exercise adaptation; several are CYP inhibitors; nattokinase adds bleeding risk
**Why:** E1 — mechanism-level evidence only, and where ITP has tested these it has mostly returned nulls. B1 — no route to a measurable outcome. Individually harmless, collectively a tax on attention, adherence, liver and wallet. Roughly 35 source rows collapse here.

**Carve-out:** "probiotics" as a *category* belongs here at 1, but specific clinically-tested strain combinations do not. Evidence in this field attaches to named strains at named doses, not to the category — see §3c.

#### EDTA chelation, HBOT, mitochondrial transfusion, stem cells / exosomes / VSELs, follistatin and telomerase gene therapy, flagellin immunisation
**1 × 1 = 1** · **AVOID** · high · medical tourism or unregulated clinics
**Why:** E1 — no human aging evidence. B1 — none. Unregulated administration carries real procedural risk with nothing on the benefit side to justify it.
