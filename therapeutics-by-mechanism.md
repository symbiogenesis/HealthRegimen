# Therapeutic Detail Rows — grouped by mechanism

Companion to [anti-aging-inventory.md](anti-aging-inventory.md). This file holds the row-level reasoning for every scored item. The human loss- and gain-of-function variants standing behind these targets — and the somatic editing programs aimed at them — are in [genetic-pathways.md](genetic-pathways.md).

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

### DXA bone mineral density (same scan, same appointment)
**4 × 3 = 12** · OK · trivial · $0 marginal on a scan already booked
**Target:** hip and lumbar spine BMD, Z-score · **Cadence:** baseline, then annually · **Cautions:** same scanner, or the series is noise
**Why:** E4 — DXA is the reference method and the BMD-to-fracture gradient is among the better-characterised dose-responses in medicine, though the interventions built on it are validated in postmenopausal women rather than in men your age. B3 — fracture is not a top-five cause of death at 39 and this will not change that. It scores 12 because **three separate exposures in this regimen converge on the same tissue, and nothing else in the document would see it happen.**

**The three-way convergence is the whole argument for the row.** A vegan diet carries the largest fracture signal of any dietary pattern studied: EPIC-Oxford put vegan hip fracture at HR 2.31 against meat-eaters after adjustment for BMI and lifestyle, with total fracture also elevated, and the UK Biobank replication attributes only about 28% of the excess to lower BMI — the residual tracks calcium and protein intake rather than the diet label. Incretin-driven weight loss subtracts bone in proportion to the weight: a 52-week semaglutide RCT lost 2.6% at the hip and 2.1% at the lumbar spine against placebo, the SURMOUNT program shows the same pattern at somewhat larger magnitude because the weight loss is larger, and 2026 analyses find the BMD decline concentrated in participants **without** diabetes — which is you. And an anti-growth block is a period of reduced mechanical loading and reduced anabolic signalling, which is the third withdrawal stacked on the first two.

None of those three is individually alarming. Together they are the clearest example in this regimen of a cost that compounds silently, on a tissue with no symptom until it fractures, measured by an instrument you are already paying for twice a year. Add the bone readout to the body-composition scan and it costs nothing.

**What the number means at 39, and what to do about it.** Z-score, not T-score — T compares you to a young adult, which you nearly are, and is the wrong comparator until later. A Z-score above −1.0 and stable across a cycle is the pass condition. **The action if it falls is not a drug.** Bisphosphonates score 1 for an aging indication (§17) and there is no primary-prevention case for them in a 39-year-old man. The levers are the three exposures themselves: calcium and vitamin D to adequacy (§14), protein held at the floor that is already non-negotiable, impact and axial loading kept in the anti-growth block rather than dropped with the hypertrophy volume, and the tirzepatide dose cut. That is the same list the fuel floor already produces, which is the point — bone is one more readout on failure modes the regimen is already watching for, not a new front.

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

**The ladder:** HMG-CoA reductase (statin) → NPC1L1 (ezetimibe) → PCSK9 (four modalities) → apo(a) (not yet available). ACL (bempedoic acid) sits on the *same* rung as the statin — see §2d — rather than adding one.

**Why this family carries the longevity case, not just the cardiology case.** The geroprotective claim here rests on human data of a kind nothing else in this document has. Mendelian randomisation against parental lifespan puts 1 SD higher genetically proxied LDL-C at 1.2 years shorter life (95% CI −1.55 to −0.87; n≈1,012,240), with an odds ratio of 0.72 for surviving to the 90th versus the 60th percentile age. Target-by-target MR against lifespan finds the lipid-lowering alleles of *HMGCR*, *PCSK9*, *APOB* and *LPL* associated with longer life — though not with extreme longevity — and identifies *LDLR* as the strongest of them, with about 23% of the lifespan effect mediated through coronary disease specifically, meaning most of it is not. On the dementia end, drug-target MR plus observational meta-analysis across ~1M people finds *HMGCR*, *NPC1L1* and *CETP* variants all associated with lower dementia risk per mmol/L lower non-HDL-C; the *PCSK9* result there is inconsistent and should not be leaned on.

**And it works in people who are well.** CTT's 27-trial individual-participant meta-analysis found that at 5-year vascular risk under 10% — the tier you are in — each 1 mmol/L of LDL-C lowering still prevented about 11 major vascular events per 1,000 over five years, with no excess cancer incidence, cancer mortality or non-vascular mortality. A 2026 meta-analysis restricted to primary prevention (14 outcomes trials, ~98,500 participants, statins plus ezetimibe and bempedoic acid) puts the pooled effect at a 30% relative reduction in 4-point MACE per 1 mmol/L (RR 0.70, 95% CI 0.67–0.74).

**Where the 2026 ACC/AHA dyslipidemia guideline puts you.** The guideline's frame is "lower sooner": PREVENT 10-year *and* 30-year risk, Lp(a) once in a lifetime for everyone, CAC raised to a Class 1 recommendation for reclassification, and apoB used to intensify therapy when LDL-C is already at goal. Its apoB goals are <55, <70 or <90 mg/dL by risk tier, so <70 is the guideline number for primary prevention. The hook that applies at 39 is explicit: in adults 30–59 with low 10-year risk, a moderate-intensity statin is reasonable when LDL-C is 160–189 mg/dL **or 30-year ASCVD risk is ≥10%**. The <60 target used throughout this document is deliberately below guideline, and the justification is cumulative exposure rather than 10-year risk — 30 years of treatment is the thing being bought, and the guideline's own 30-year framing is what licenses reaching past its 10-year number.

### 2a. Targets

#### ApoB to <60 mg/dL
**5 × 5 = 25** · MONITOR · trivial · statin + ezetimibe, ~$60/yr
**Why:** E5 — three decades of RCTs with hard outcomes, and the effect holds in the low-risk tier rather than being borrowed from secondary prevention. B5 — ASCVD is the #1 lifetime cause of death and cumulative ApoB exposure is the driver. Ference's Mendelian randomisation puts 40 years of 1 mmol/L lower LDL-C at a 54.5% lower CHD risk against roughly 24% per mmol/L for a statin started in mid-life and run for five years — about 3× the effect from the same target, bought by starting earlier. Starting at 39 rather than 55 is the whole argument.

#### ApoB to <30 mg/dL (the increment beyond <60)
**4 × 4 = 16** · MONITOR · high · Rx; needs triple therapy
**Measure:** ApoB q8wk during titration; hsCRP; HbA1c
**Cautions:** requires a PCSK9 inhibitor, and payer criteria gate every agent in the class behind documented failure of statin plus ezetimibe at a baseline LDL-C you will not have — so it is a cash purchase; Lp(a) puts a fixed floor under the achievable number
**Why:** E4 — no RCT has ever *randomised* anyone to an ultra-low target. Support is post-hoc achieved-level analysis plus human genetics, and both are strong. In FOURIER-OLE, 1,604 patients (24% of 6,635) reached LDL-C <20 mg/dL and were followed a further median 5 years, with a monotonic relationship between lower achieved LDL-C and lower event risk that survived multivariable adjustment, and no safety separation from higher achieved levels; some participants held LDL-C under 20 for more than 8 years. The specific fears have been tested and have not materialised: EBBINGHAUS found no cognitive effect below 25 mg/dL, FOURIER found none in the 2,339 participants under 20, and the AHA scientific statement on aggressive LDL lowering and the brain concludes there is no dementia or intracerebral-haemorrhage penalty attributable to the LDL level itself. A 2026 systematic review taking the ten standing objections one at a time — cognition, cancer, haemorrhagic stroke, new-onset diabetes, cataract, hormonal effects, myopathy — finds none of them attributable to the achieved level, and a 2025 network meta-analysis of statins against PCSK9 inhibitors finds no intracerebral-haemorrhage excess in any patient category. The genetics point the same way — *PCSK9* nonsense carriers run ~28% lower LDL-C lifelong and have 88% less coronary heart disease (Cohen, NEJM 2006), the rare complete-deficiency cases sit near LDL-C 15 mg/dL with no overt phenotype, and over 200 heterozygous and 20 homozygous *ANGPTL3* loss-of-function carriers are described with ~40% lower ASCVD odds and no adverse cardiometabolic phenotype. Strong — but achieved-level and genetic evidence is a different class from a randomised target, so E4. B4 — the increment is real, and cumulative-exposure logic makes it *more* attractive at 39 than at 65, but it is the second slice of a shrinking pie taken from an already-reduced baseline. `high` effort because reaching it costs roughly 13× more per year.
**The relative benefit does not fade at the bottom; the absolute one does.** This is the distinction the row turns on, and it is easy to get backwards. A meta-analysis of trials whose participants *started* at a median LDL-C of 65.7 mg/dL and reached a median of 21 found the same ~22% reduction in major vascular events per 38.7 mg/dL as trials starting at 131.5 — the log-linear relationship holds all the way down, with no threshold and no attenuation, and no offsetting harm. What shrinks as you descend is the size of the pie, not the fraction you take from it. So the argument for stopping is never "it stops working"; it is that a constant fraction of a residual risk you have already cut in half is worth less than what the same money buys elsewhere, and that after 40 years at ApoB 45 the risk still standing is increasingly not atherosclerotic at all.
**What Lp(a) actually costs you here:** each Lp(a) particle carries one apoB-100, so Lp(a) contributes apoB mass that no LDL-directed drug can remove. The arithmetic is fixed — apoB-100 has a conserved molecular weight of 512 kg/mol, so 1 nmol/L of Lp(a) is about 0.05 mg/dL of apoB. At Lp(a) 75 nmol/L that is ~4 mg/dL; at 250 nmol/L it is ~13 mg/dL. Particle-counting studies agree: Lp(a) is ~3% of apoB particles on average and ~15% in the top decile. So a high Lp(a) does not make <30 unreachable, it spends up to half the budget before you start — and it does so with particles that are roughly 6-fold more atherogenic per particle than LDL, which is the real reason to measure it.
**The practical position:** treat <60 as the commitment and don't back away from a lower number the generics hand you for free. Rosuvastatin 10 mg plus ezetimibe lands many people near 45. Take that; just don't buy the last 15 points. The arithmetic on that last clause: both generics together run ~$300/year, and enlicitide lists at $315/month — ~$3,780/year, or about $150,000 undiscounted over the 40 years the cumulative-exposure case is asking you to commit to.
**What would reopen it:** ApoB still above 60 on both generics; Lp(a) above 125 nmol/L, which shifts the reason to want a PCSK9 inhibitor onto its ~20–25% Lp(a) lowering rather than the ApoB number; CAC above zero at any age; CORALreef Outcomes reporting; or an enlicitide cash-pay programme or generic. Safety is not on that list, and will not be — that question is settled in the direction of *lower is fine*, which means the reason to stop is price, not risk.

### 2b. HMG-CoA reductase

#### Rosuvastatin 10 mg (generic) — the default pick
**5 × 5 = 25** · MONITOR · trivial · Rx, $4–15/mo
**Measure:** ApoB at 8 weeks; ALT once at baseline
**Cautions:** do not stack with red yeast rice (same molecule); berberine raises exposure via CYP3A4
**Why:** E5 — three decades of RCTs with hard outcomes. B5 — moves a typical 39-year-old from roughly ApoB 100 to roughly 60 for about $60/year, the largest and cheapest increment available anywhere in this document. Hormone-stack reassurance: the 2024 meta-analysis (21 studies, 9,879 patients) found statins lower *total* testosterone by ~13 ng/dL in RCTs, not below the normal range, with no change in *free* testosterone, LH, estradiol or SHBG.
**Why 10 mg and not 5:** rosuvastatin 10 mg gives ~44–46% LDL-C reduction in trials against ~35–37% for atorvastatin 10 mg — it is roughly 1.5× as potent milligram-for-milligram, so 10 mg sits around atorvastatin 20–40 mg. Starting at 5 mg is a dose for someone already near target; you are starting from an untreated baseline and aiming under 60.

**Choosing between rosuvastatin and atorvastatin.** Both are generic, both are E5, and the head-to-head says the choice is a tiebreaker rather than an efficacy decision. LODESTAR randomised 4,400 adults with coronary disease to rosuvastatin or atorvastatin for three years: the composite of death, MI, stroke or revascularisation was 8.7% versus 8.2% (HR 1.06, 95% CI 0.86–1.30), so no difference that matters. Two signals did separate, both against rosuvastatin — new-onset diabetes requiring treatment 7.2% versus 5.3% (HR 1.39, 1.03–1.87) and cataract surgery 2.5% versus 1.5% (HR 1.66, 1.07–2.58) — alongside a slightly lower achieved LDL-C (1.8 versus 1.9 mmol/L), which is likely where at least the diabetes signal comes from, since statin dysglycaemia tracks potency.

**Rosuvastatin wins here on the specifics of your stack.** The diabetes signal is the one adverse effect you are already comprehensively insured against: you are on tirzepatide, which is doing far more to your glycaemia in the protective direction than 10 mg of a statin can do in the harmful one. What does not have an offset is the interaction surface — atorvastatin is a CYP3A4 substrate, rosuvastatin is metabolised mainly by CYP2C9 and largely excreted unchanged. That is the same axis the berberine AVOID flag (§4) turns on, and it is the one that keeps mattering as items get added. Atorvastatin 20 mg is a fully reasonable substitute if it is cheaper or better stocked; the cataract signal is a single-trial finding in an older coronary population and should not be the deciding factor either way. Pitavastatin is the third generic and the most glycaemically neutral of the class, which would matter if you were not on an incretin — you are, so it buys nothing for more money.

#### Red yeast rice / monacolins
**3 × 2 = 6** · **AVOID** · trivial · OTC
**Cautions:** **unstandardised lovastatin at an unknown dose — do not stack with a statin**
**Why:** E3 — it works, because it is a statin. B2 — same benefit as a prescription statin. AVOID only because the dose is unknown and unregulated. Take the actual statin.

### 2c. NPC1L1 (cholesterol absorption)

#### Ezetimibe (generic)
**4 × 4 = 16** · OK · trivial · Rx, ~$10/mo
**Measure:** ApoB at 8 weeks · **Cautions:** none
**Why:** E4 — IMPROVE-IT showed a real but modest hard-outcome benefit on top of statin, in a post-ACS population. B4 — CORALreef AddOn measured it directly against the alternatives on background statin and ezetimibe cut apoB 20.2%, for pocket change. Best value-per-dollar pairing in the document and absent from the source table entirely.
**Take it with the statin rather than after it.** RACING randomised 3,780 patients to moderate-intensity statin plus ezetimibe versus high-intensity statin alone: the same 3-year composite outcome (10.1% versus 10.3%), a *lower* achieved LDL-C (57 versus 65 mg/dL), and half the intolerance-driven discontinuation or dose reduction (3.9% versus 8.0%), with no difference in new-onset diabetes. Two mechanisms at moderate doses outperform one at a high dose on tolerability and land lower. RACING was run in established ASCVD, so the outcome equivalence is borrowed rather than demonstrated in primary prevention — but the LDL and tolerability results are what the sequencing decision turns on, and those transfer.
**One honest asymmetry:** NPC1L1 is the weakest of the lipid targets in lifespan MR — the *HMGCR* and *PCSK9* alleles associate with longer life and *NPC1L1* does not reach significance. That is most likely an instrument-strength problem rather than a biological one, and it runs against the dementia MR, where *NPC1L1* looks as protective as *HMGCR*. It is a reason not to claim a longevity effect for ezetimibe specifically, not a reason to skip a $10 drug that removes a fifth of your apoB.

### 2d. ATP citrate lyase

#### Bempedoic acid
**4 × 4 = 16** · MONITOR · moderate · Rx, ~$430–610/mo · **only if statin-intolerant**
**Measure:** ApoB; uric acid · **Cautions:** raises uric acid ~0.5–0.8 mg/dL, gout 3.2% versus 2.2% on placebo; tendon rupture 1.2% versus 0.9%
**Why:** E4 — CLEAR Outcomes (n=13,970, 40.6 months) showed a 13% MACE reduction, and its primary-prevention subgroup (n=4,206) showed a 27% reduction in all-cause mortality, 3.6% versus 5.2% (HR 0.73, 0.54–0.98) — the strongest mortality result in this family from anything resembling a prevention population. But that population was statin-intolerant, mean age 68, and two-thirds diabetic. B4 — meaningful apoB reduction *when it is the only thing on board*.
**Why it is not a rung on the ladder.** ACL sits two steps upstream of HMG-CoA reductase in the same cholesterol-synthesis pathway, and the 2×2 factorial Mendelian randomisation of *ACLY* against *HMGCR* (NEJM 2019) found the two lower LDL-C by the same mechanism, with the same effect on cardiovascular risk per unit LDL-C. Genetically, bempedoic acid *is* a statin with a different binding site. That prediction has now been measured: in CORALreef AddOn, on background statin, bempedoic acid reduced apoB by **5.4%** — against 20.2% for ezetimibe, 27.7% for the two together, and 54.6% for enlicitide. Adding it to a tolerated statin buys almost nothing, because the lever is already pressed. There is also no hard-outcome trial of bempedoic acid on top of a statin anyone tolerates; CLEAR Outcomes exists precisely because that population was excluded.
**Nexlizet** is bempedoic acid and ezetimibe in one tablet, ~$430–610/month retail with no generic. Since generic ezetimibe is ~$10/month, the marginal thing being purchased is the 5.4% component. If statin plus ezetimibe leaves you off target, the evidence points up the ladder to PCSK9 — the same trial that produced the 5.4% figure showed enlicitide beating bempedoic acid, ezetimibe and their combination — not sideways to ACL.

### 2e. PCSK9 — four modalities, one target

All four block PCSK9-mediated degradation of the LDL receptor, so LDL receptors recycle instead of being destroyed. Same target, same downstream effect, four delivery routes. They are separated here **only** by how far each has been carried through outcomes trials.

| Agent | Modality | Dosing | E × B | Outcomes trial |
|---|---|---|:---:|---|
| Evolocumab / alirocumab | monoclonal antibody | SC q2wk or q4wk | **5 × 5 = 25** | **Reported** — FOURIER, ODYSSEY, VESALIUS-CV |
| Inclisiran | siRNA | SC q6mo after loading | **4 × 5 = 20** | Pending — ORION-4, VICTORION-2P |
| Enlicitide (Lipfendra) | oral macrocyclic peptide | 20 mg daily, oral | **4 × 5 = 20** | Pending — CORALreef Outcomes |

#### Evolocumab / alirocumab
**5 × 5 = 25** · OK · high · Rx, ~$500–600/mo cash
**Measure:** ApoB; Lp(a) · **Cautions:** none known; additive with statin by design
**Why:** E5 — FOURIER and ODYSSEY established hard-outcome benefit, and VESALIUS-CV extended it to primary prevention: ~12,000 patients with no prior MI or stroke, median 4.6 years, a 31% relative reduction in major cardiovascular events on top of maximally tolerated statin, with nominal reductions of 32% in cardiovascular death and 24% in all-cause mortality. The benefit is therefore demonstrated in people who have not had an event, not inferred across from those who have. B5 — same target as the statin, deeper. Scores identically to the generic statin because on the merits it is that good; the entire difference is the effort tag and the coverage gate. Prior authorisation generally requires established ASCVD or HeFH, which you do not have — and note that VESALIUS-CV's "primary prevention" still meant documented atherosclerosis or high-risk diabetes plus LDL-C ≥90 mg/dL, which is a long way from a healthy 39-year-old. The drug is proven further than it is available to you, and further than it is needed by you.

#### Inclisiran
**4 × 5 = 20** · OK · high · Rx, ~$500–600/mo equivalent
**Measure:** ApoB; Lp(a) · **Cautions:** none known; additive with statin by design
**Why:** E4 — the monoclonals' justification ("FOURIER and ODYSSEY established hard-outcome benefit") does not apply here. Inclisiran was approved on LDL-C lowering alone; ORION-4 and VICTORION-2P have not reported. It sits in the same evidence position as enlicitide, not the same position as the monoclonals. B5 — same target, same depth of LDL receptor recycling. Note that two injections a year is arguably the *lowest* administration burden in this family, oral included; what keeps it at `high` effort is cost and prior authorisation, not logistics.

#### Enlicitide decanoate (Lipfendra), oral
**4 × 5 = 20** · OK · high · Rx, approved 15–16 Jul 2026, ~$315/mo list
**Measure:** ApoB; Lp(a) · **Cautions:** none known
**Why:** E4 — CORALreef Lipids gave 55.8% placebo-adjusted LDL-C reduction (n=2,904) and ~50% ApoB reduction; CORALreef HeFH gave 59.4%; CORALreef AddOn beat ezetimibe, bempedoic acid and their combination on background statin. These are surrogate endpoints and CORALreef Outcomes (>14,500 enrolled) has not reported — but the class prior here is unusually strong. PCSK9-mediated LDL lowering is one of the best-validated surrogates in medicine, and CTT plus Mendelian randomisation show benefit tracking absolute LDL-C reduction largely independent of the mechanism used to achieve it. A two-point penalty against the monoclonals would overstate the uncertainty; one point is right. B5 — removes the injection barrier for the best non-statin target in the family.
**The cheapest way into this family, and still not cheap.** At a $315/month list price it undercuts the monoclonals roughly two-fold, and its label is broad — primary hypercholesterolaemia, as an adjunct to diet and maximally tolerated statin, rather than gated on ASCVD or familial hypercholesterolaemia. The label is not the gate, though. Payer criteria require a documented eight-week failure of high-intensity statin plus ezetimibe with a baseline LDL-C at or above 70 mg/dL, which is a threshold a healthy 39-year-old on both generics is nowhere near. Treat it as a ~$3,780/year cash item until that changes.

### 2f. apo(a) / Lp(a)

#### Lp(a)-lowering therapy (pelacarsen, olpasiran, lepodisiran, muvalaplin)
**2 × 4 = 8** · OK · high · not yet approved · **WATCH**
**Measure:** Lp(a) once · **Cautions:** none
**Why:** E2 — no outcomes data yet for any agent in the class. B4 — if Lp(a) is elevated it is your single largest unaddressed genetic risk, and nothing currently available lowers it much; per apoB particle it is roughly 6-fold more atherogenic than LDL, which is why a modest-looking number matters. Lp(a)HORIZON (pelacarsen, n≈8,325) is the first CV outcomes trial for the class. It is event-driven and has run past its guided mid-2026 window without reporting; OCEAN(a) (olpasiran) has primary completion targeted for December 2026. This row exists so whichever readout lands first finds you already knowing your number.

---

## 3. Incretin and glucose handling

### 3a. Incretin receptor agonism

#### Tirzepatide
**4 × 4 = 16** · MONITOR · moderate · Rx · **CONTINUE**
**Measure:** DEXA fat mass index, appendicular lean mass index and visceral fat; HbA1c; ApoB
**Target:** FMI 2.5–3.5 kg/m² · ALMI ≥8.5 kg/m² · VAT <50 cm² · fuel floor: total testosterone ≥500 ng/dL
**Cautions:** **with an SGLT2 inhibitor, any week of vomiting or minimal intake becomes a euglycemic ketoacidosis risk**; hold before anesthesia; interacts with low-protein protocols
**Why:** E4 — SELECT showed ~20% MACE reduction with semaglutide in non-diabetic overweight adults, along with all-cause death at HR 0.81 (0.71–0.93); for tirzepatide specifically the hard-outcome trial has not reported. SURMOUNT-MMO (n≈15,000, obesity without diabetes, all-cause death inside the primary composite, completing October 2027) is the first incretin outcomes trial to cover primary as well as secondary prevention, and is the readout that would move this row to E5. B4 — the best-evidenced pharmacological item in your stack. Pair with protein and lifting or the lean-mass cost is real. This is the item that most constrains everything else on the list.

**Body fat percentage is the wrong instrument.** It is a ratio with two independent numerators, so it moves when fat changes, when lean changes, and identically for both — 15% at 55 kg of lean mass and 15% at 62 kg are different bodies with different prognoses, and the number cannot tell them apart. Worse, on this drug the two move together in the direction that hides the problem: lose fat and lean in the same proportion and the percentage does not budge. Index both to height and track them separately. **FMI 2.5–3.5 kg/m²** is the fat target; at a solid ALMI it corresponds to roughly 12–15% body fat, and it stays honest when lean mass changes. **ALMI ≥8.5 kg/m²** sits near the young-adult male mean and far above the 7.0 kg/m² sarcopenia cutoff — the margin is sized for the fact that this lean mass has to survive both the drug and the anti-growth blocks, and the direction across a full cycle matters more than the level on any one scan. **VAT <50 cm²** is the aggressive number of the three: visceral fat is the depot carrying the causal metabolic risk, the exposure-outcome relationship has no identified floor within the achievable range, and it keeps falling after the other two have stalled. There is no reason to stop at the conventional 100 cm² "not elevated" line. Scanner-specific and calibration-dependent — the same machine every time, or the series is noise.

**Where the evidence actually runs out.** The move from 20% body fat to 15% is well supported: VAT falls, insulin sensitivity improves, ApoB and blood pressure follow. From 15% to 12% there is no mortality evidence in either direction, because nobody has run it — the epidemiology at the low end is dominated by illness-driven weight loss and by people whose leanness is low lean mass rather than low fat, which is the opposite phenotype. So FMI 2.5–3.5 with ALMI held at 8.5 is a bet on mechanism, not a finding. It is a defensible one: the intervention is reversible within weeks, the failure modes announce themselves, and the alternative is a target set by population averages that already include the outcome being avoided. FMI 2.5–3.5 sits at or below the low end of the NHANES reference band by design. That is the point of it, and it is also why the floor below has to be functional rather than numeric.

**The floor is function, not a percentage.** In men, sustained energy deficit degrades gonadal, thyroid and skeletal function well before any percentage becomes dangerous, and the sequence is reliable: libido and morning erections go, sleep fragments, training output falls at unchanged volume, resting heart rate drops with cold extremities, and total testosterone slides. Below roughly 8–10% these become likely; between 10% and 12% they are individual. Which means the number cannot be set in advance — 12% is fine for most men and untenable for some, and the only way to know is to watch the markers on the way down. Total testosterone under 500 ng/dL is the lab version of the same signal, drawn at each phase boundary alongside IGF-1. Any of them tripping outranks every target above it.

**The cycle sets the range.** A permanent caloric deficit and a genuine pro-growth block are mutually exclusive, so a single year-round fat target contradicts the structure of the protocol. FMI runs to the bottom of the band coming out of an anti-growth block and drifts to the top through accumulation. The floor is a trough, not a set point.

**Why the drug continues past target.** SURMOUNT-4 answered this directly: after a 36-week lead-in averaging ~21% weight loss, participants randomised to continue lost a further 5.5% over the next year while those switched to placebo regained 14% — roughly half the loss, inside twelve months, with blood pressure, lipids and inflammatory markers tracking back up alongside it. The trials also treat the drug as chronic; SELECT's MACE benefit accrued on continued therapy, and SURMOUNT-MMO is designed the same way. Reaching target is the point at which the dose becomes a maintenance dose, not the point at which it stops.

**Brown adipose is not one of the reasons.** GIP receptor agonism increases energy expenditure in rodents with a brown-fat component to the effect, and it is a plausible piece of why a dual agonist outperforms GLP-1 alone. It does not transfer cleanly to a 39-year-old human: adult BAT is a few tens of grams, highly variable, and human energy-expenditure measurements on incretin agonists have not shown thermogenesis beyond what the weight loss itself predicts. The human effect is dominated by intake. Continued dosing is worth defending on regain and on maintained cardiometabolic control — both measured in humans on hard endpoints — rather than on thermogenesis.

#### Retatrutide
**3 × 2 = 6** · MONITOR · moderate · not approved · **WATCH — no action before the body-composition readout**
**Target:** GLP-1, GIP and glucagon receptors
**Measure:** if it is ever started, DEXA on the tirzepatide schedule and against the same FMI, ALMI and VAT targets; resting heart rate; ALT
**Cautions:** carries the whole GLP-1 caution set — hold before anesthesia, euglycemic ketoacidosis risk alongside an SGLT2 inhibitor in any week of vomiting or minimal intake — plus two of its own: dysesthesia, and a resting heart rate rise of roughly 5–10 bpm
**Why:** E3 — the phase 3 program is large and consistent, and entirely surrogate. TRIUMPH-1 (n=2,339, obesity or overweight without diabetes) gave 28.3% mean weight loss at 80 weeks on 12 mg against 19.0% on 4 mg, with 45.3% of the 12 mg arm past 30% and 65.3% brought under a BMI of 30; the BMI ≥35 continuers reached 30.3% at 104 weeks. TRIUMPH-4 gave 28.7% at 68 weeks, TRANSCEND-T2D-1 16.8% with HbA1c −2.0% at 40 weeks. Weight is not a surrogate that has earned E4 status the way LDL-C has, and TRIUMPH-Outcomes (n≈10,000, cardiovascular and kidney endpoints in obesity) does not complete until February 2029. B2 — you are already on the drug this would replace, and the axis it wins on is the magnitude of weight loss, which is not what tirzepatide is in the stack for. The 12 mg arm lost 31.9 kg on average; the lean fraction of that has not been published, so there is no way to score a switch against an ALMI floor of 8.5 kg/m² and a >1 kg-per-block stopping rule. The incremental case narrows to two situations, neither of which currently applies.

**What the glucagon arm buys, and what it costs.** Glucagon receptor agonism raises energy expenditure and mobilizes hepatic fat — the one mechanism here that a dual agonist does not have, and the reason a triple agonist should beat tirzepatide in MASLD specifically. The cost is tolerability and cardiac chronotropy: discontinuation rose with dose to 11.3% at 12 mg against 4.9% on placebo, dysesthesia appears as a signal fairly specific to this molecule, and resting heart rate rises roughly 5–10 bpm, peaking near week 24 before declining, which is the class pattern at a larger magnitude. Systolic pressure falls over the same window — 7.4 mmHg across the program, 14.0 mmHg at 68 weeks on 12 mg in TRIUMPH-4 — so net vascular loading is ambiguous rather than plainly adverse. Against a 105–115 systolic target the pressure effect is welcome and the heart rate is the thing to watch.

**Approval is not the readout.** Filing is guided for Q4 2026, which puts an FDA decision no earlier than mid-to-late 2027 and access in 2027–2028. That decision will turn on the weight-loss endpoint, which is already known, so it resolves nothing here. The number that decides this row is the TRIUMPH-1 body-composition substudy — lean versus fat mass in the 12 mg arm. If lean-mass retention is no better than tirzepatide's, the larger absolute loss makes retatrutide actively worse for a protocol measured on DEXA, and the score stands. Retention meaningfully better than tirzepatide's would be the surprise that moves it.

**When the calculus changes:** a weight target tirzepatide has not reached, or MASLD, where the glucagon arm is doing something the current drug cannot.

### 3b. SGLT2 inhibition

#### Empagliflozin / canagliflozin
**3 × 2 = 6** · MONITOR · low · Rx · **optional; incompatible with fasting cycles**
**Measure:** ketones (home β-hydroxybutyrate meter); volume status; genital exam
**Cautions:** **euglycemic ketoacidosis — precipitated by fasting, carbohydrate restriction, vomiting, dehydration or surgery, not by the GLP-1 alone; glucose reads normal so it is routinely missed.** Hold for any FMD cycle, any illness with poor oral intake, and 3 days pre-procedure
**Why:** E3 — ITP canagliflozin gave **+14% median lifespan in males only**, the largest male effect in ITP history, concordant across all three test sites, with 90th-percentile survival up 9%. On the human side the decisive fact is that **DAPA-HF, DAPA-CKD and EMPA-KIDNEY enrolled non-diabetics and the benefit held in that subgroup** — so this is not a glucose-lowering effect riding on baseline hyperglycemia. Large cohorts also show ~30% lower dementia incidence versus DPP-4 inhibitors, consistent across meta-analyses but observational. What still caps it at E3: every trial is in T2D, HF or CKD, where much of the benefit is hemodynamic and renal, and none is in metabolically healthy adults. B2 — for a 39-year-old with no HF, CKD or T2D and ApoB already controlled by a statin, the absolute benefit is speculative and substantially redundant with tirzepatide, which delivers the metabolic effect with hard-outcome data behind it. The source table ranked this #1 on a 12/12 gerotherapeutics score; that score means "most deserves a trial," which entails that the human aging evidence does not yet exist.

**Why MONITOR rather than AVOID.** Ketoacidosis risk tracks insulin deficiency, not weight and not the GLP-1 per se. In DAPA-HF and DAPA-CKD, ketoacidosis events occurred **only** in participants with type 2 diabetes — none among the non-diabetic participants, over several thousand patient-years. The T2D trial base rate is 0.6–2.2 events per 1,000 patient-years. Euglycemic ketoacidosis in true non-diabetics is documented and has its own case literature, but it is rare and almost always precipitant-driven. Being lean does not by itself protect: the published SGLT2i-plus-tirzepatide case is a 35-year-old man with a BMI of 20.7.

**What the flag is actually about: fasting, not phase.** An SGLT2 inhibitor is a caloric-restriction mimetic and belongs conceptually in an anti-growth block. The incompatibility is narrower and sharper than the block — it is the **FMD cycles inside it**, plus any tirzepatide week with vomiting or minimal intake. Those are the states that produce relative insulin deficiency on top of a drug already driving lipolysis and ketogenesis. So the choice is between the two, not between the phases: run the FMD cycles, or run an SGLT2 inhibitor, not both in the same block.

**Which agent.** The lifespan data is canagliflozin; the cleaner safety record is empagliflozin, which carries no CANVAS-style amputation signal. There is no way to have both, and the amputation signal is human while the lifespan signal is mouse.

**When the calculus changes:** with type 2 diabetes, CKD or heart failure, SGLT2 inhibitors become first-line and genuinely excellent. Same row, trigger changes from "aging" to "diagnosis."

**The trial that would settle the E3.** VITAL-H, inside the ARPA-H PROSPR program, is the first phase 3 study to test geroprotection in adults who are not sick: 726 generally healthy people aged 60–65 randomised to rapamycin, dapagliflozin, semaglutide or placebo, with Intrinsic Capacity — cognition, locomotion, psychological, vitality, sensory — as the primary construct. It is the missing arm for this row and for rapamycin (§5) simultaneously: the same objection caps both scores, and this is the study designed to remove it. Nothing here changes until it reports.

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

**The published record on this formulation, in full:** Perraudeau 2020 in *BMJ Open Diabetes Res Care*, a CGM crossover in *JMIR Formative Research*, and the 2022 *BMC Microbiology* mechanism paper. That is the whole list, and it is the same list Pendulum's own clinical-trials page carries. There is no NEJM, *Lancet*, *Nature Medicine* or *Cell Metabolism* trial of WBF-011 — the high-tier microbiome papers associated with the brand belong to the row above: Depommier 2019 and Mount 2026 (*Nature Medicine*) and Zhang 2025 (*Cell Metabolism*) all tested **pasteurized single-strain MucT**, a different preparation from the live multi-strain blend. Note also where the headline p-value sits: postprandial AUC came in at p=0.0500, on the line rather than under it.

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

The training interaction is a **timing** problem rather than a permanent exclusion — see [growth cycling](anti-aging-inventory.md#part-4--growth-cycling). Metformin's short half-life (~6 h) makes it the easiest item on the entire list to phase cleanly. That improves its schedulability without improving its evidence, so it still scores 4.

#### Berberine
**2 × 1 = 2** · **AVOID** · trivial · OTC · **SKIP**
**Target:** AMPK · **Measure:** HbA1c
**Cautions:** **potent CYP3A4 / P-gp inhibitor — raises statin, rapamycin and tadalafil exposure unpredictably**
**Why:** E2 — rodent and small human data. B1 — nothing a statin does not do better. AVOID because the interaction liability is real and it buys you nothing. This flag is pharmacokinetic and does not relax in any phase.

---

## 5. mTOR and nutrient sensing — the anti-growth arm

Everything in this section pushes the same direction: down-regulate mTORC1 and IGF-1 signalling, favour autophagy and catabolic housekeeping, reduce the substrate available for anabolic error.

**These items are not permanently incompatible with §6.** They are incompatible *simultaneously*. See [Part 4 of the main document](anti-aging-inventory.md#part-4--growth-cycling) for the block-cycling structure that separates them in time; the scores below reflect each item on its own merits regardless of scheduling.

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
**Cautions:** **do not run while on an SGLT2 inhibitor — this is the precipitant that makes that combination dangerous**
**Why:** E2 — human trials exist but measure surrogates over short horizons. B2 — modest. Listed mainly because it reaches the FGF21 signal by a route that never pushes an amino acid below requirement, and because the fasting/refeeding cycle carries regenerative data that no dietary composition change does.

**This is the item that most directly supports your cycling hypothesis**, and it is worth more attention than its score implies. FMD is *already* a cycle protocol: Longo's design is 5 days on, then refeeding, a few times a year. The refeeding phase is not downtime — in mice, fasting/refeeding cycles drove hematopoietic stem cell self-renewal and immune reconstitution (Cheng et al., *Cell Stem Cell*, 2014), which is the same regenerative endpoint TRIIM-X targets by a much more expensive and much less evidenced route. If you want a pro/anti-growth alternation with actual human trial infrastructure behind it, this is the cheap version.

#### Methionine source shifting (protein held constant)
**2 × 1 = 2** · OK · low · food
**Target:** amino acid composition — SAM/SAH, FGF21, IGF-1 · **Measure:** DEXA lean mass; homocysteine
**Cautions:** cancelled by NAC/GlyNAC; do not combine with total protein restriction on a GLP-1
**Why:** E2 — the rodent data is solid, and the intermittent form of it works: four days replete against three days restricted cut IGF-1 40–56% and raised FGF21 42–87 fold, matching continuous restriction, with more lean mass and more bone retained than the continuous arm (Plummer, *Aging Cell*, 2022). B1 — the human trial run at the depth a plant-based diet can actually reach is negative. In 59 adults with overweight over 8 weeks, both arms on plant-based whole foods at ~2 g/day sulfur amino acids against ~5.6 g/day, IGF-1 rose in both groups with no separation (p=0.46), FGF-21 did not move (p=0.66), fat mass did not differ (p=0.27), and the restricted arm lost *more* fat-free mass (−0.69 kg, p=0.013) for 1.14 kg more total weight (*J Transl Med*, 2024). Both mediators the intervention is supposed to run on failed to appear.

**The gap between the rodent and human results is dose.** The mouse protocols that work use 0.12% methionine, or methionine-free days, against 0.86% controls — an 80–100% cut, with the methionine-free arm the stronger of the two. That is frank deficiency rather than composition. Plummer's mice still sat 11–22% below controls on lean body mass, and IGF-1 returned to control levels within four days of repletion. The signal is real and steeply dose-dependent, and the dose is not reachable at a sufficiency-respecting intake.

**On a vegan diet the lever is already pulled.** EPIC-Oxford puts vegan methionine intake at 0.88 g/day against 1.67 for meat-eaters, and total sulfur amino acids at 2.3 g/day against 6.8 on a high-protein Western pattern. The 2024 trial's *restricted* arm was a whole-food plant-based diet; its control arm was constructed by adding methionine and cysteine capsules on top of the same base. A vegan eats the intervention year-round, in both phases — which is also why it cannot be the thing that distinguishes them.

**Plasma methionine is not a usable readout.** Diet-group differences in EPIC-Oxford span −13% to +16%, and eight weeks of an 80% dietary cut in rats produced no plasma difference at all. Homeostatic buffering absorbs it. Homocysteine and DEXA are what this row is measured on.

**It is the anti-growth dietary lever most compatible with an SGLT2 inhibitor, though not an inert one.** Euglycemic ketoacidosis requires insulinopenia plus volume depletion, and its precipitants are carbohydrate deficit, fasting and reduced intake — none of which is amino acid composition at constant calories and carbohydrate. But restriction raised β-hydroxybutyrate by 117 µmol/L against controls in the 2024 trial, so running both stacks a mild ketogenic pressure rather than none. Keep the ketone meter if you do.

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

**Framing note:** this section is not in permanent opposition to §5. The opposition is real *at any given moment* and dissolves when the two are separated in time — which is how several of these interventions were designed to be used in the first place. What follows scores each item on its own merits; the scheduling argument lives in [Part 4](anti-aging-inventory.md#part-4--growth-cycling).

#### Resistance training 2–3×/week
**3 × 5 = 15** · OK · moderate · free
**Target:** mTORC1, myonuclear addition, bone loading · **Measure:** DEXA lean mass; grip strength
**Cautions:** rapamycin blocks contraction-induced MPS
**Why:** E3 — RCTs are consistent but measure surrogates (strength, lean mass, function) rather than mortality. B5 — non-negotiable on a GLP-1, because it is the only thing that reliably protects the lean mass the drug puts at risk.

**This is the pro-growth phase.** Whatever else growth cycling includes, training plus protein is the component with real evidence behind it, and it is free. Note also that **maintenance requires far less volume than accumulation** — trained individuals hold strength and lean mass on roughly one-third of accumulation volume for months (Bickel 2011). A reduced-volume block during an anti-growth phase is physiologically defensible in a way that a full detraining block is not.

#### Protein 1.2–1.6 g/kg/day, distributed
**3 × 4 = 12** · OK · trivial · food
**Target:** muscle protein synthesis · **Measure:** DEXA lean mass; grip
**Cautions:** conflicts with the proposed methionine restriction protocol as originally specified
**Why:** E3 — RCTs are consistent but measure lean mass and strength, not mortality. B4 — on a GLP-1 this is the difference between losing fat and losing muscle. Distribution across meals beats bolus loading, and muscle protein synthesis has a per-meal ceiling and refractory period, so a week's intake cannot be banked into a weekend.

**Hitting the floor is the hard part on a vegan diet, and it is the most likely point of failure in the whole regimen.** Appetite suppression from tirzepatide meets lower protein density and lower leucine per gram, and the two compound. Soy, seitan and pea isolate are the dense options; whole-food legumes carry a lot of volume per gram of protein, which is exactly the wrong property under a GLP-1. Treat the number as tracked rather than assumed — this is the line that the DEXA stopping rule is really testing.

#### Creatine monohydrate 5 g/day
**3 × 3 = 9** · OK · trivial · OTC, ~$30/yr
**Target:** phosphocreatine, cell hydration · **Measure:** DEXA; grip; strength log · **Cautions:** none
**Why:** E3 — hundreds of RCTs, but on strength and lean mass rather than hard outcomes. B3 — modest alone, more valuable here because it directly counteracts GLP-1 lean-mass loss. The most conspicuous omission from the 128-row source list. Unflavored monohydrate only. Larger effect on a vegan diet than the score implies: dietary creatine is essentially all animal-derived, muscle stores start well below omnivore levels, and the response in vegetarians and vegans is consistently the biggest in the trial literature.

#### Block-periodized growth cycling (training-led, no rhGH)
**2 × 3 = 6** · OK · moderate · free
**Target:** phase separation of mTORC1/IGF-1 signalling · **Measure:** DEXA at each phase boundary; grip weekly; IGF-1; fasting insulin; ApoB
**Cautions:** an SGLT2 inhibitor and the FMD cycles cannot occupy the same block; do not compress the washout between blocks
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

#### Myostatin / activin blockade (bimagrumab, apitegromab)
**2 × 2 = 4** · MONITOR · high · not approved · **WATCH — no action while the lean-mass floor holds**
**Target:** ActRII signalling — myostatin and activin A
**Measure:** if it is ever started, DEXA ALMI and FMI on the tirzepatide schedule, with grip and the strength log as the read that carries the weight; lipase; amylase; ALT
**Cautions:** dose-dependent transient lipase, amylase and ALT elevations alongside a GLP-1 that already carries a pancreatitis warning; muscle spasms, diarrhea, acne; IV administration on a half-life measured in weeks, which is what makes it unphaseable
**Why:** E2 — two randomized phase 2 trials, both reporting body composition and nothing else. BELIEVE (n=507, 48 weeks, obesity without diabetes) gave 22.1% weight loss on bimagrumab 30 mg/kg plus semaglutide 2.4 mg, of which 92.9% was fat: fat mass fell 45.7% and lean mass 2.9%, against 27.8% and 7.4% on semaglutide alone. Bimagrumab alone gained 2.5% lean mass with 100% of the weight loss coming from fat. EMBRAZE (apitegromab plus tirzepatide, 24 weeks) reproduces the finding on the drug actually in the stack — 1.9 kg more lean mass retained, p=0.001, an 85/15 fat-to-lean split against 70/30 — and it also prices the trade, since total weight loss was 12.3% against 13.4%. B2 — the axis it wins on is the one this regimen is measured on, and it is the same axis already covered by training, protein and creatine at no cost and no risk. The incremental benefit exists only in the branch where those have failed.

**Mass is the surrogate, not the endpoint.** Bimagrumab's older indications are the cautionary set. It raised muscle mass in sarcopenia, in recovery after hip fracture, and in sporadic inclusion body myositis, and in each case gait speed and strength moved minimally or not at all. Blocking ActRII adds tissue reliably; that the added tissue does the work of trained muscle is an assumption, and the obesity trials report DEXA compartments with no functional endpoint, so they do not test it either. A protocol that treats ALMI as a proxy for capacity is exposed to exactly this gap.

**Phasing is the structural objection.** ActRII blockade is a continuous anabolic signal delivered intravenously with a half-life in weeks, so it cannot be confined to a six-week pro-growth block the way rapamycin can be confined to an anti-growth one. Run it and the anti-growth block still carries a pro-growth drug, which collapses the alternation the calendar exists to produce. It also disables the instrument: ALMI is simultaneously the stopping rule and the judge of whether the structure works, and a drug that raises ALMI on its own makes a stable number uninformative — an adequate block and a failing one would read the same. Grip and the strength log are what remain unconfounded, and they are a coarser instrument than the one being given up.

**When it becomes a live question:** ALMI below 8.5 kg/m², or lean mass down more than 1 kg across a full anti-growth block, with protein documented at ≥1.2 g/kg and maintenance-volume lifting held, at a tirzepatide dose that has already been cut. That is the failure of the two highest-scoring rows in this section, and it is the only situation in which an antibody buys something the free interventions are not already buying.

**The molecule and the mechanism are not the same bet.** Lilly acquired bimagrumab with Versanis and then terminated its phase 2b bimagrumab-plus-tirzepatide trial in type 2 diabetes in September 2025, citing strategic business reasons; a phase 2 in obesity without diabetes runs to January 2027. No agent in the class has a phase 3 in obesity. This row tracks ActRII blockade rather than bimagrumab specifically — apitegromab has the more relevant trial and trevogrumab is on the same axis, and which one arrives first is open.

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
**Why:** E3 — VITAL, REDUCE-IT and STRENGTH give a mixed and dose-dependent picture. B2 — small. Already in your stack, no reason to stop, no reason to escalate the dose. On a vegan diet the source is algal oil rather than fish oil, and the item moves from optional-continue toward baseline adequacy: ALA-to-EPA conversion runs at a few percent and DHA conversion lower still, so flax, chia and walnuts do not substitute. Dose to an omega-3 index in the 4–8% band.

#### Cold water immersion / cold plunge
**2 × 1 = 2** · OK · low · **SKIP as a therapy — and if you do it anyway, it is a phase item**
**Target:** claimed: brown adipose, norepinephrine, hormesis · **Cautions:** blunts hypertrophy when it follows resistance training
**Why:** E2 — human trials exist and measure surrogates over short horizons; the mood and alertness effects are the best-supported thing about it and are acute rather than durable. B1 — no route to a measurable outcome at 39, and the brown-adipose argument fails here for the same reason it fails for GIP agonism in §3a: adult BAT is a few tens of grams and human energy expenditure does not move beyond what the intervention's other effects predict.

**It earns a row anyway because it has a real interaction, and it is the one hormesis item that fits the cycling calendar cleanly.** Post-exercise cold immersion attenuates resistance-training adaptation — Roberts' work showed blunted satellite cell and p70S6K responses acutely and reduced strength and hypertrophy gains over 12 weeks against active recovery, and the meta-analytic picture has held: the effect is on hypertrophy and strength specifically, not on endurance adaptation, which cold leaves intact or occasionally helps. The mechanism is the same one that governs the antioxidant rows — the post-training inflammatory and ROS signal is what the adaptation is built from, and cold suppresses it.

**So it is not a yes-or-no question but a calendar question, and the calendar already exists.** Cold immersion belongs in anti-growth blocks, where cardio is the emphasis and hypertrophy is not being pursued, and out of pro-growth blocks entirely — or at minimum kept more than four hours away from a lifting session and never on the same day as a heavy one. Sauna (below) does not carry this problem and is the better-evidenced of the two heat-and-cold items; if you are going to do one for enjoyment, that is the one that does not tax the block you are in.

#### Sauna 3–4×/week
**2 × 2 = 4** · OK · moderate · varies · **OPTIONAL**
**Target:** heat shock proteins, vascular function · **Cautions:** none
**Why:** E2 — the Finnish cohort data is suggestive and heavily confounded by who uses saunas; no RCT. B2 — fine if you enjoy it, which is a legitimate reason.

---

## 10. Hemodynamic, vascular and antithrombotic

#### Blood pressure: aim 105–115 systolic, drug over 120
**5 × 4 = 20** · MONITOR · trivial · lifestyle; Rx generics if needed
**Target:** vascular load · **Measure:** home BP series; potassium and creatinine if on a drug · **Cautions:** none
**Why:** E5 — SPRINT plus dozens of RCTs with hard outcomes. B4 — enormous if you are hypertensive, near-zero if you are not, which is why the home cuff comes first. Absent from the source table entirely, which is its largest single omission.
**Why the threshold and the aim are different numbers:** 120 is where the trials stopped, not where the benefit stops. SPRINT, ESPRIT (n=11,255) and BPROAD (n=12,821) all randomise <120 against <140 and land at ~119–121, so nothing below 120 has ever been tested pharmacologically. Everything else in the evidence base keeps going down: the Prospective Studies Collaboration (1M adults) found no threshold to at least 115/75, with the steepest relative slope at exactly this age; BPLTTC (48 trials, ~345,000) found the proportional benefit per 5 mmHg undiminished at baselines below 120/70; Mendelian randomisation puts *lifelong* 10 mmHg lower at roughly 50% less CHD against ~20% for five years of drug therapy; and unwesternised populations sit there permanently — Yanomami adults average 95/63 with no rise from age 2 to 60, Tsimane men gain 0.91 mmHg per decade. The rise with age is environmental, not biological. What does not transfer is the drug arm: SPRINT and ESPRIT bought their benefit with excess syncope, hypotension, electrolyte disturbance and acute kidney injury, and those harms track drug count. So 105–115 reached through cardio, sodium and leanness is the goal — a compliant artery as well as a low cuff — while a second agent to chase a healthy 39-year-old from 118 to 106 is unsupported by any trial. Two fears do not apply here: intensive treatment *reduces* orthostatic hypotension rather than causing it (Juraschek, 9 trials, >18,000 participants), and the diastolic J-curve in the SPRINT post-hoc appeared only in participants with pre-existing cardiovascular or renal disease. Diastolic perfusion is a stiff-artery problem; at 39, 105/65 is a low-pressure system rather than an underperfused one. Past ~115, brachial systolic is also the wrong instrument — cfPWV predicts events independently of it, and the levers that move arterial stiffness are the same lifestyle ones.
**Drug choice:** the number carries almost all of the benefit and class differences on hard outcomes are small, so pick on tiebreakers. RAS blockade is the only antihypertensive mechanism with any lifespan signal in normotensive animals — ITP captopril, enalapril surfacing on the Gehan re-analysis, AT1-receptor knockout mice — and ARBs match ACE inhibitors on outcomes with far less cough and angioedema (ONTARGET). **Telmisartan 40–80 mg** takes it within the class on the longest half-life and partial PPAR-γ agonism, which improves insulin sensitivity where a thiazide degrades it. Second agent: **amlodipine** (ACCOMPLISH beat a thiazide combination); chlorthalidone offers no advantage over hydrochlorothiazide (Diuretic Comparison Project) and both cost glucose, urate and potassium. Recheck potassium and creatinine after starting — a legume-heavy vegan diet is already potassium-rich and an ARB pushes the same way.
**If you are on an ARB, it has to be held for the fasting cycles.** This is the interaction the fasting-mimicking rows create that the SGLT2 discussion tends to crowd out. An ARB works by removing the angiotensin II-mediated efferent arteriolar tone that defends glomerular filtration when renal perfusion falls, so it is specifically the drug class whose harm profile depends on volume status. A five-day FMD cycle delivers exactly that state — low intake, low sodium, natriuresis, and a systolic that is already being driven to 105–115 — and the standard "sick day" rule for RAS blockade exists for the same physiology. Hold the ARB through any FMD cycle and any tirzepatide week with vomiting or poor intake, restart with normal eating, and expect the held days to need no substitute, because the fast is lowering the number by itself. Symptomatic orthostasis during a fast on an ARB means stop the fast, not push through it.
**One measurement artifact worth knowing before it confuses a lab.** Creatine supplementation raises serum creatinine by a small amount through the ordinary conversion of creatine to creatinine, with no change in glomerular filtration — enough to move an eGFR by a few points and to look, on a report, like early renal impairment. Stacked on an ARB, that is a false alarm sitting on top of a real monitoring requirement. If a creatinine comes back unexpectedly, cystatin C settles it, because it does not share the pathway.

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

#### Vitamin K1 (phylloquinone) and K2 (MK-7, MK-4)
**2 × 1 = 2** · OK · trivial · OTC · **SKIP as a supplement — K1 is already oversupplied by the diet**
**Target:** γ-carboxylation of matrix Gla protein (arterial) and osteocalcin (bone) · **Measure:** dp-ucMGP, if you ever want the biomarker
**Cautions:** antagonises warfarin, which is the one real interaction and does not apply to you. Nattokinase, in the §17 bundle, is the fibrinolytic enzyme from natto and is not vitamin K2 — the two are not substitutes in either direction.
**Why:** E2 — a specific, well-characterised mechanism plus consistent cohorts, and RCTs that reliably move the biomarker without moving the endpoint. B1 — the endpoint it aims at is arterial calcification, and at 39 with ApoB handled there is nothing there yet to act on.

**This has the best mechanism of any supplement in the document, and it still fails.** Matrix Gla protein is the principal local inhibitor of arterial calcification, it is inert until vitamin K carboxylates it, and *Mgp*-null mice die within weeks of aortic calcification and rupture. The biomarker behaves exactly as the mechanism predicts: MK-7 lowers dephosphorylated-uncarboxylated MGP dose-dependently, and functional insufficiency by that marker (dp-ucMGP >500 pmol/L) runs about 31% of a general population at mean age 53 in PREVEND, rising toward 50% with hypertension, diabetes or CKD. So there is a prevalent, measurable, correctable biochemical deficit with a named target. That is more than NMN or astaxanthin can claim, and it is why this gets its own row rather than collapsing into the bundle at §17.

**The trials that tested the endpoint came back null.** AVADEC gave 720 µg/day MK-7 plus vitamin D for two years to ~300 men in their seventies: the aortic valve calcification primary endpoint was neutral, and the coronary calcium endpoint was neutral too — 203 AU progression on treatment against 254 AU on placebo, p = 0.089. The result that reached the trade press was the CAC ≥400 subgroup at p = 0.047, which is a subgroup of a null trial in the highest-burden stratum. In CKD and dialysis, where the calcification burden is worst and the vitamin K deficit most severe — the population where the mechanism should be easiest to demonstrate — meta-analyses find no effect on calcification progression and none on mortality.

**What is positive is one rung lower on the surrogate ladder.** Knapen's three-year trial of 180 µg/day MK-7 in 244 postmenopausal women improved carotid-femoral pulse wave velocity, and a one-year trial published in 2025 reports its stiffness and blood-pressure effects in a post-hoc stratum of women with high baseline stiffness. Arterial stiffness is a surrogate that has not earned the status ApoB has — nothing has causally validated it to outcomes by RCT and Mendelian randomisation together — so this does not reach the E4 carve-out in [Part 1](anti-aging-inventory.md#the-scoring-model).

**The cohort signal is a dietary pattern.** Rotterdam (n=4,807, ten years) found the top tertile of dietary menaquinone at RR 0.43 for CHD mortality, 0.74 for all-cause mortality and OR 0.48 for severe aortic calcification, with **phylloquinone associated with none of it.** The menaquinone in that population came from cheese, egg yolk and organ meat, so the exposure being measured is as much a way of eating as a vitamer, and no trial has since recovered the effect.

**Bone repeats the shape.** ECKO gave 5 mg/day of K1 for two to four years to 440 osteopenic postmenopausal women and found no protection against BMD decline; fracture and cancer differences appeared only in underpowered secondary analyses. The meta-analyses reporting hip fracture odds ratios near 0.23 rest almost entirely on small Japanese menatetrenone 45 mg trials, and the largest of them (the OF study, n=4,378) did not reproduce the fracture benefit — the standard signature of small-study effects.

**Which menaquinone, given that the choice is pharmacokinetic rather than ethical.** Both forms are vegan: MK-7 is made by *B. subtilis natto* fermentation and MK-4 is chemically synthesised, so neither is animal-derived and sourcing does not decide it. Pharmacokinetics does, and it decides against MK-4. A single 420 µg dose of MK-4 was undetectable in the serum of every subject at every timepoint, and 60 µg/day for a week raised serum MK-4 not at all, while the same doses of MK-7 peaked at 6 h and remained detectable at 48 h — hours of half-life against roughly three days. The vitamer that reaches extrahepatic tissue at steady state is the one already tested and found null. MK-4's own supplement-dose evidence is a single uncontrolled dose-escalation in 13 young men, where undercarboxylated osteocalcin fell at ≥600 µg/day — a bone biomarker, no placebo arm, one rung below the calcification endpoint that matters here.

**And the MK-4 dose in the literature is not the dose on the label.** The Japanese menatetrenone fracture trials ran 45 mg/day — 45,000 µg, thirty to several hundred times a typical 100–1,500 µg supplement, and a prescription drug in Japan rather than a supplement anywhere. So the marketing borrows the evidence of a pharmaceutical dose for a nutritional one, and the evidence being borrowed is the weak literature described above.

**The deeper reason MK-4 is the wrong thing to swallow:** UBIAD1 builds it *in situ*, in the tissues where MGP and osteocalcin are carboxylated, from dietary phylloquinone. Circulating MK-4 is near-absent in healthy people at any intake because it is a tissue product rather than a transport form. Supplementing it orally pushes from plasma what the cell already makes on site from a precursor that greens supply.

**The statin question, since it is specific to you.** UBIAD1 builds MK-4 from dietary K1 using geranylgeranyl pyrophosphate, a mevalonate-pathway intermediate that statins deplete; lipophilic statins also inhibit UBIAD1 directly, and atorvastatin reduced renal MK-4 in mice. That is cell-culture and rodent work against a drug carrying 25 on hard human outcomes, and no human study shows statin users with impaired carboxylation or accelerated calcification. If it ever turns out to matter, the move it argues for is rosuvastatin rather than atorvastatin — hydrophilic, equally generic, already interchangeable on the ladder in §2 — not adding a supplement.

**And the vitamin D pairing.** The claim that supplementing D without K drives calcification has no trial behind it. AVADEC ran D and K2 together, in older men with established calcification, and returned a null. Dose D to the lab value and leave K out of the decision.

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

#### Sleep regularity — same bed and wake time, ±30 min, seven days a week
**3 × 4 = 12** · OK · trivial · free
**Target:** circadian entrainment · **Measure:** Sleep Regularity Index from the tracker you already wear · **Cautions:** none
**Why:** E3 — observational, but at unusual scale and with objective exposure measurement: 60,977 UK Biobank participants and over 10 million hours of accelerometry, which removes the self-report problem that weakens most sleep epidemiology. B4 — the effect size is the reason this is a separate row rather than a clause on the one above. Across the top four SRI quintiles against the least regular, all-cause mortality ran 20–48% lower, cancer mortality 16–39% lower, and cardiometabolic mortality 22–57% lower — and **regularity predicted mortality more strongly than duration did**, in nested models where duration was allowed to compete.

**The practical consequence is that the 7–9 hour row is the wrong target to optimise once it is met.** Seven hours at a fixed time beats eight hours at a drifting one, weekend catch-up sleep is a symptom of the exposure rather than a treatment for it, and the intervention is free, requires no device beyond the one already on your wrist, and takes no time — it reallocates time that is already allocated. That combination is rare enough on this list to be worth acting on despite the evidence tier.

**Where the honest doubt sits:** irregular sleep is also what illness, shift work, alcohol, untreated apnea and depression produce, so a fraction of this is reverse causation and confounding that adjustment will not fully remove. The reason to act anyway is asymmetry rather than certainty — the intervention has no cost and no failure mode, which is not true of most rows scoring 12.

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

#### Vegan adequacy set — B12, calcium, algal EPA+DHA, iodine, D3, taurine
*Unscored* · OK · trivial · OTC, ~$100/yr
**Target:** nutrients the diet removes · **Measure:** B12, ferritin, zinc annually; omega-3 index; 25-OH-D; DXA BMD with the body-composition scan
**Cautions:** none at these doses

These are not geroprotectors and the `E × B` model does not apply to them — nothing here extends anything. They close gaps the diet opens, and they belong in the regimen for the same reason a seatbelt does: cheap, certain, and the downside of skipping them is the whole point.

- **B12, 2000 µg/week or 50–100 µg/day.** The one nutrient with no plant source at all. Deficiency is a demyelinating neuropathy that can outrun the hematologic signs, so the megaloblastic anemia is not a reliable early warning. Non-negotiable, and the only item in this set with a disabling failure mode.
- **Calcium to 1,000 mg/day, food first and supplement to close the gap.** The item in this set with the best-evidenced hard endpoint attached to it, and the one most often skipped because the diet feels healthy. Vegan intake averages well below every other dietary pattern — dairy is the dominant source in Western diets and the plant substitutes are either low-density or poorly absorbed, since oxalate in spinach, chard and beet greens binds most of the calcium they list. What absorbs is fortified soy milk, calcium-set tofu (check the coagulant — calcium sulfate, not nigari), low-oxalate greens like kale, bok choy and broccoli, tahini, almonds and fortified juices. EPIC-Oxford found the vegan fracture excess concentrated in participants eating under 525 mg/day, which puts the risk in intake rather than in the diet label. Split doses at 500 mg or below, since fractional absorption falls above that, and take it with a meal. Do not exceed roughly 1,000–1,200 mg/day from supplements: supplemental calcium above the requirement has its own cardiovascular signal, and the target here is adequacy, not a large intake.
- **Algal EPA+DHA, ~500 mg/day.** ALA-to-EPA conversion runs a few percent and DHA lower still, so flax, chia and walnuts do not substitute. Same evidence base as the omega-3 row in [§9](#9-redox-and-hormesis) — the change is the source, not the case.
- **Iodine, 150 µg/day** from iodized salt or a supplement. Sea vegetables carry it but dose across two orders of magnitude between species and batches, which makes them a poor delivery vehicle in either direction.
- **Vitamin D as lichen-derived D3.** Standard D3 is lanolin-extracted; D2 raises 25-OH-D less efficiently and less durably.
- **Taurine, 500 mg–1 g/day** — full reasoning at the row in [§17](#17-no-credible-mechanism-or-unregulated-administration), where it sits because the *aging* claim is dead. The nutritional claim is independent and holds.

**Carnitine looks like taurine and is decided the other way, which is worth stating here rather than only at its row.** Both are animal-tissue compounds absent from plants, both run lower in vegan plasma, and both have a synthetic route from amino acids. The difference is that carnitine synthesis from lysine and methionine is fully competent in adults where CSAD is not, so there is no gap of the kind taurine has — and that roughly 90% of an oral carnitine dose, in any ester including acetyl-L-carnitine, comes back as TMAO. A repletion argument only works when repletion is free, and this one is not. The full case, including why the vegan microbiome's protection against TMAO does not survive chronic supplementation, is at the [carnitine row in §17](#carnitine--l-carnitine-acetyl-l-carnitine-propionyl-l-carnitine).

Iron and zinc are monitored rather than supplemented: non-heme iron absorbs at a fraction of heme iron and phytate binds zinc, so both run lower on a plant diet without necessarily running short. Ferritin also gates the blood donation row in §17. Selenium is the third of these — US wheat carries enough that frank deficiency is rare, and a single Brazil nut most days closes any gap without the selenosis risk of a handful. Creatine and protein are handled in [§6](#6-gh--igf-1-and-anabolism--the-pro-growth-arm), where both carry vegan-specific notes.

**Bone is where this diet has its one genuine hard-endpoint liability, and it is the reason calcium sits in the list above rather than being assumed.** Every other item here prevents a deficiency syndrome that is rare, reversible, or both. Fracture is neither: EPIC-Oxford puts vegan hip fracture at HR 2.31, the excess concentrates at low calcium intake, and hip fracture in later life carries mortality and disability out of all proportion to how it sounds. Set against that, the diet's cardiovascular and cancer advantages are real and larger — this is a reason to fix the calcium and watch the DXA, not a reason to reconsider the diet. It matters more here than it would for most vegans because two further exposures load the same tissue at the same time; the arithmetic is in [§1](#1-measurement-and-diagnostics) under the bone density row.

**Vitamin K sits at the edge of this set, and what decides it is greens rather than veganism.** K1 is concentrated, not distributed: leaves carry it and a few oils carry it, while legumes, grains, nuts, fruit, tofu and seitan largely do not. A vegan eating greens most days sits at the top of the national intake distribution; a vegan living on beans, grains and faux meat can sit under the 120 µg/day AI, which 43% of US men already do. Two things stop that from being a deficiency. The AI is an observed-intake figure rather than a functional requirement — there is no EAR for vitamin K — and the criterion behind it is hepatic clotting-factor synthesis, which on any varied diet is close to impossible to compromise without malabsorption or an anticoagulant. What a low-greens intake actually buys is a position at the high-dp-ucMGP end of the extrahepatic reserve, which is precisely the marker the MK-7 trials in [§10](#10-hemodynamic-vascular-and-antithrombotic) corrected without changing an endpoint.

**Preparation matters more than volume, because the food tables overstate leaves.** K1 in a leaf is bound into chloroplast thylakoid membranes and absorbs at a small fraction of the rate from an oil or a tablet; fat in the same meal roughly triples it. A large raw salad under a fat-free dressing can deliver less than a modest serving of greens cooked in oil.

**If greens are genuinely low, the fix is food, and the vitamin K is the least of what it buys.** Cooked greens carry potassium and nitrate — both serving the 105–115 systolic aim in §10 — plus folate, lutein and fiber, and fiber alone scores 9. One serving cooked in oil two or three times a week clears the AI by itself. The other lever is the cooking oil: soybean at roughly 25 µg per tablespoon and canola at 10 µg are real sources, while olive oil at a few µg is not. A plain K1 tablet around 100 µg is a legitimate fallback — same class as taurine, repletion toward adequacy with no outcome to expect from it, and vitamin K has no established upper limit — but it buys one item out of that package and none of the rest.

**Low greens is an argument for more K1, not for K2.** Menaquinone intake on a plant diet genuinely is low, since the dietary K2 sources are cheese, egg yolk and meat and the only substantial plant source is natto at ~1,000 µg MK-7 per 100 g. Supplement supply is not the constraint — fermentation-derived MK-7 and synthetic MK-4 are both vegan — so nothing here turns on sourcing. But there is no defined deficiency state for menaquinone as distinct from vitamin K, and UBIAD1 builds MK-4 from dietary phylloquinone in the tissues where MGP and osteocalcin are carboxylated — so less K1 also means less substrate for the endogenous route, and the deficit points back at the same food. The real pharmacological argument for MK-7 is its half-life, days against hours for K1, which is what gets it to extrahepatic tissue at steady state; that is the argument the trials in §10 tested and failed to convert into an endpoint. K2 is skipped on outcome, not on veganism.

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

#### Microplastic exposure reduction
**2 × 2 = 4** · OK · trivial · ~$40 for a filter pitcher and steel containers
**Target:** ingested and inhaled polymer particles · **Measure:** none exists · **Cautions:** none
**Why:** E2 — one prospective human study with a hazard ratio large enough to demand attention and methodology weak enough to prevent acting hard on it. Marfella's NEJM cohort followed 257 patients after carotid endarterectomy and found polyethylene in 58.4% of excised plaques; those with detectable micro- and nanoplastics had an HR of 4.53 (2.00–10.27) for MI, stroke or death at 34 months. The criticism is specific and serious rather than generic: no pre-analytical anticontamination protocol was used, and an operating theatre is full of plastic, so some unknown share of the signal may have entered the specimen after the patient did. B2 — the exposure is plausibly causal, universal, and currently unquantifiable in any individual, which is a combination that supports cheap avoidance and nothing stronger.

**What makes this row worth having rather than folding into the supplement bundle is that the actions are free and independently justified.** The dominant modifiable sources are heating food in plastic, drinking from single-use bottles, and abraded synthetic textiles. Do not microwave in plastic or run it through a dishwasher's heated cycle, use glass or steel for hot and fatty foods, filter tap water rather than buying bottled — bottled water carries substantially more particulate than filtered tap, which inverts the intuition most people have — and ventilate while cooking, which the PM2.5 row already argues for. Every one of those is a one-time purchase or a habit, none of them costs anything ongoing, and none depends on the hazard ratio being right.

**What this row does not license.** There is no test worth buying, no chelation or "detox" protocol with any evidence behind it, and no supplement that removes plastic from tissue — that entire market is downstream of exactly this paper. Blood and plasma "microplastic panels" sold direct to consumers have no validated reference range and no action attached to a result.

---

## 16. Early detection

#### Cancer screening on schedule
**5 × 4 = 20** · OK · low · insurance
**Target:** early detection · **Cadence:** colonoscopy at 45; skin annually · **Cautions:** none
**Why:** E5 — sigmoidoscopy and FIT RCTs show mortality reduction; NordICC was intention-to-treat disappointing but per-protocol positive. B4 — cancer is the #2 lifetime cause. Mostly a calendar problem, not a decision problem.

#### Multi-cancer early detection blood test (Galleri)
**3 × 1 = 3** · OK · high · ~$950 cash, not covered · **SKIP — and the trial is why**
**Target:** circulating tumour DNA methylation across cancer types · **Cautions:** a positive result commits you to a diagnostic workup with its own risks; a negative result is not reassurance
**Why:** E3 — the evidence here is unusually good for a consumer product and the verdict is still no, which is the useful part. NHS-Galleri is the first and only randomised controlled trial of an MCED test: 142,250 participants aged 50–77, annual screening for three years on top of standard care. It **missed its primary endpoint.** The full results reported at ASCO in May 2026 are genuinely good on everything except the thing the trial was built to show — a roughly four-fold higher overall cancer detection rate, more stage I and II diagnoses among deadly cancers, substantially fewer stage IV diagnoses, specificity of 99.6%, just over half of positives confirmed as cancer, and no serious related adverse events. What it did not demonstrate is the reduction in late-stage incidence it was powered for, which is the surrogate standing in for mortality benefit.

**That gap is the entire decision, and it is the oldest one in screening.** Detecting more cancer earlier is not the same as preventing death from cancer, because some of the additional detection is overdiagnosis and some is lead time without a change in outcome — the history of PSA and of neuroblastoma screening is exactly this shape, and both looked like this at the same stage. A stage-shift result this clean is a strong reason to expect the mortality readout to be positive and not a substitute for having it.

**B1 is the binding constraint regardless.** The trial enrolled from 50; you are 39, where cancer incidence is low enough that even excellent specificity produces a positive predictive value far below the trial's, because PPV falls with prevalence no matter how good the assay is. At your age the expected yield of a positive is dominated by false alarms and by workups you would not otherwise have had. Revisit when the mortality endpoint reports and when you are inside the age band the test was validated in — both conditions, not either.

#### Whole-body MRI screening (Prenuvo and similar)
**1 × 1 = 1** · MONITOR · high · ~$2,500 cash · **SKIP**
**Target:** incidental detection of anything · **Cautions:** the harm here is the workup, not the scan
**Why:** E1 — no randomised trial, no mortality data, and no evidence in asymptomatic adults that it changes an outcome. The published yield studies find clinically significant findings in a low single-digit percentage of scans against incidental findings in something closer to a third to a half, and gadolinium-free protocols do nothing about that ratio. B1 — at 39 the base rate makes it worse, not better: the same arithmetic that sinks MCED sinks this harder, because MRI has no specificity figure to defend itself with. What you are buying is a high probability of finding something ambiguous in an organ you were not worried about, followed by a biopsy or a surveillance schedule with real complication rates, in exchange for a small probability of a finding that matters.

**It is on the list because it is the most heavily marketed item in consumer longevity and it is the one an inventory like this is expected to have an answer for.** The answer is that guideline screening scores 20 and this scores 1, and the money is better spent on the colonoscopy at 45.

---

## 17. No credible mechanism, or unregulated administration

#### Taurine
**1 × 1 = 1** · OK · trivial · OTC · **SKIP as a geroprotector; take 500 mg–1 g/day as nutritional repletion on a vegan diet**
**Target:** none as an aging intervention; taurine status on a plant diet · **Measure:** none needed at this dose · **Cautions:** none
**Why:** E1 — **premise retracted.** Fernandez et al., *Science* 2025: longitudinal data across three human cohorts, rhesus monkeys and mice show taurine **rises or holds steady** with age, with interindividual variation exceeding any age effect. B1 — the rationale for supplementing it *for aging* has been removed, and the score reflects that claim alone.

The nutritional case is separate and does not depend on the aging literature. Taurine occurs almost exclusively in animal tissue — shellfish, fish, meat, and dairy in smaller amounts — with plant foods carrying trace quantities, so vegan intake is near zero against roughly 40–400 mg/day for an omnivore. Vegans measure lower plasma taurine and much lower urinary excretion than omnivores. Endogenous synthesis from cysteine via CDO and CSAD covers the gap in adults, but human CSAD activity is low, and a plant diet is simultaneously low in the sulfur amino acid substrate. No deficiency syndrome has been demonstrated in adult vegans — the cat cardiomyopathy and retinal degeneration model does not transfer, since cats cannot synthesize taurine at all — so this is repletion toward the omnivore range at trivial cost, with no outcome to expect from it.

**It does not conflict with methionine work.** Taurine is the terminal product of cysteine catabolism and is not converted back to cysteine, so it carries none of the cancellation problem that removes NAC and GlyNAC from the list.

#### Carnitine — L-carnitine, acetyl-L-carnitine, propionyl-L-carnitine
**2 × 1 = 2** · MONITOR · trivial · OTC · **SKIP as a geroprotector — and unlike taurine, it is not a vegan adequacy item either**
**Target:** the CPT1/CPT2 shuttle that carries long-chain fatty acids into the mitochondrial matrix, plus acyl-group buffering of the CoA pool
**Measure:** plasma TMAO, if it is taken chronically anyway — one of the few supplement assays in this document with an action attached to the result
**Cautions:** roughly 90% of an oral dose returns as TMAO; peripheral antagonist of thyroid hormone action; INR rise reported with warfarin; fishy body odour at gram doses is the TMA pathway announcing itself
**Why:** E2 — mechanism plus a set of small, old, mostly single-sponsor RCTs in disease populations, and no lifespan test in a mammal that survived independent replication. B1 — nothing here has a route to an outcome in a healthy 39-year-old, and the one exposure it reliably adds runs against the top-scoring family in this document.

**What Ames actually showed, and where the case stops.** Three back-to-back *PNAS* papers in 2002 from Hagen, Liu and Ames fed acetyl-L-carnitine and R-α-lipoic acid to 24–28-month F344 rats and reported restored mitochondrial membrane potential, recovered hepatocyte oxygen consumption, improved carnitine acetyltransferase substrate-binding affinity, more ambulatory activity and better memory performance. That is a striking set of results and it is also the high-water mark of the case: the endpoint throughout is function in old rodents, and lifespan was not the measure. Ames and Hagen founded Juvenon in 1999 to license the University of California patent on the combination, and Ames chaired its scientific advisory board — disclosed in the papers themselves, and worth naming because the advocacy and the company are the same object. When lifespan was tested directly, Spindler's independent mouse cohorts found the ALCAR/lipoic acid cocktail did not extend it. The ITP has never run carnitine in any form, so the strongest rodent claim available is a functional one from a lab with a financial position in the answer.

**The variants differ in where they go, not in what they do.** All of them deliver the same carnitine backbone to the same shuttle; the ester decides the tissue and the indication.

| Variant | Where the ester takes it | Best human evidence | What it is actually a drug for |
|---|---|---|---|
| **L-carnitine** | plasma; muscle only through an insulin-gated transporter | 13-trial post-MI meta-analysis (n=3,629): 27% lower all-cause mortality | haemodialysis, valproate toxicity, genetic OCTN2 deficiency |
| **Acetyl-L-carnitine** | crosses the blood–brain barrier — the only real differentiator | depressive symptoms (12 RCTs, n=791); diabetic neuropathic pain; MCI and mild AD (21 trials) | named neurological and psychiatric conditions, symptomatically |
| **Propionyl-L-carnitine** | vascular endothelium; the propionyl group is anaplerotic | claudication walking distance | peripheral arterial disease |
| **L-carnitine L-tartrate** | muscle, through the same gate | recovery markers after resistance exercise | a sports supplement |

The cardiac meta-analysis is the biggest number in that column and the weakest. Its trials are small, largely pre-reperfusion-era, and the pooled effect exceeds what modern secondary-prevention drugs achieve on a far larger evidence base — which is the standard signature of bias rather than of an overlooked therapy, and it was the substance of the published criticism at the time. Nothing in the reperfusion era has retested it.

**Acetyl-L-carnitine does not dodge the TMAO problem — it is worse on that axis.** The intuition is that the acetyl ester is absorbed as a unit and never meets the microbiome. The pharmacokinetics say the opposite. Head-to-head in healthy volunteers at 0.5 and 1.5 g, acetylcarnitine's plasma ΔAUC came in **7.7-fold lower** than carnitine's, and roughly **90% of both** was recovered as TMAO, reaching ~50 µM in plasma. Lower bioavailability means *more* of the dose stays in the colon for the microbes, and the deacetylated backbone is the same substrate: carnitine → γ-butyrobetaine → TMA → hepatic FMO3 → TMAO. The one advantage ALCAR has — a molecule that reaches brain tissue — is bought at the cost of the one disadvantage you were trying to avoid.

**The vegan position is genuinely different, and it is not durable.** This is the part of the standard TMAO warning that does not apply to you as written. Koeth's carnitine challenge showed omnivores generating **more than 20-fold** more labelled TMAO than long-term vegans and vegetarians, because the converting taxa are diet-selected and a plant diet does not maintain them. So a single carnitine exposure in a vegan mostly passes through. The CARNIVAL trial then asked the question that actually matters for supplementation — 500 mg/day of L-carnitine tartrate for two to three months — and found that chronic exposure **induces the pathway**, enhancing the rate-limiting γBB→TMA step by up to 10-fold, with circulating TMAO rising in both dietary groups. The protection is a property of the microbiome you currently have, and taking the supplement is the intervention that removes it. Occasional exposure is fine; the thing being proposed is not occasional.

**Why it is not in the vegan adequacy set, when taurine is.** Preformed carnitine is essentially absent from plants, so intake on this diet is near zero against 60–180 mg/day for an omnivore, and plasma runs measurably lower — the same shape as the taurine argument. It resolves differently for two reasons. Endogenous synthesis from lysine and methionine, via trimethyllysine and SAM-derived methyl groups, is fully competent in adults rather than the low-capacity backstop CSAD is for taurine; no functional deficit has been demonstrated in vegan adults, and the deficiency states that do exist are Mendelian (*SLC22A5*/OCTN2) or secondary to dialysis and valproate. And the repletion carries a cost that taurine's does not: taurine at 1 g is inert, while carnitine at any dose is 90% converted into a metabolite with a plausible atherogenic mechanism, in someone whose entire top tier is built around not accelerating atherosclerosis. Adequacy arguments justify closing a gap at trivial cost; this gap does not close for free. Legume-forward plant protein is lysine-rich, which supports the synthetic route the diet actually uses.

**The muscle and mitochondrial rationale does not reach the tissue anyway.** Oral bioavailability of L-carnitine is under 20%, and skeletal muscle uptake runs through OCTN2 against a large concentration gradient in an insulin-dependent manner — plain oral dosing does not raise muscle carnitine at all. What works is Wall and Stephens' loading protocol: 2 g of carnitine co-ingested with roughly 80 g of carbohydrate, twice daily, for 12 to 24 weeks, for about a 15–20% rise in muscle content. That protocol is close to unavailable on a GLP-1 — it requires ~160 g/day of carbohydrate taken specifically to spike insulin, against appetite suppression and a body-composition target. Whatever the mitochondrial fatty-acid-oxidation argument is worth, the delivery problem forecloses it here, and the creatine row in [§6](#6-gh--igf-1-and-anabolism--the-pro-growth-arm) is the ergogenic supplement that does reach muscle and does have the trials.

**Where the trigger changes.** The depression and diabetic-neuropathy meta-analyses are the most respectable evidence carnitine has, and they belong to the same category as the ARBs and beta blockers below: real drugs for real diagnoses, scoring 1 as aging interventions. If a depressive episode ever needs treating, ALCAR's tolerability profile makes it a reasonable adjunct to raise with a clinician — the PHQ-9 in the annual panel is what would surface it. That is a different decision from the one on this row, and it is the only route by which carnitine enters the picture.

#### Partial epigenetic reprogramming (OSK / Yamanaka factors)
**1 × 4 = 4** · **AVOID any clinic offering it** · high · not available · **WATCH**
**Target:** epigenetic age reversal without loss of cell identity · **Measure:** none applicable
**Cautions:** the teratoma and dedifferentiation risk is the reason the field moved to partial and transient expression; systemic delivery in humans is unsolved
**Why:** E1 — mouse only for the systemic claim. Optic nerve regeneration in aged and glaucomatous mice, partial rejuvenation in progeroid models, and functional restoration in several tissues, all with cyclic or transient factor expression. In humans there is one cleared IND: ER-100, cleared by FDA in January 2026 for optic nerve disease, which is a **local, single-organ, disease indication** and not a systemic aging intervention. B4 — if reprogramming works in humans the way it works in mice, it is a different category of intervention from everything else in this document, and the B score reflects that rather than any expectation of availability.

**It belongs in this document precisely because it is the field's largest bet and there is nothing to do about it.** The gap between "rejuvenation has been demonstrated in mice" and "rejuvenation is available" is delivery, dose control and oncogenic risk, and none of the three is close to resolved for systemic use. A partial-reprogramming row scoring 4 and an NMN row scoring 2 are saying different things with similar numbers: NMN is available and does not work, this may work and is not available. The scoring model separates those on the E and B axes, which is what it is for.

**The AVOID attaches to the clinics, not the science.** Offshore and unregulated providers already market "reprogramming," "Yamanaka factor," and gene-therapy rejuvenation packages. They sit with EDTA, HBOT and stem cell clinics at the bottom of this section for the same reason: unregulated administration of an intervention whose principal risk is oncogenic, with no dose control and no follow-up. Watching this field costs nothing; buying into it now is the single worst risk-adjusted decision available in the whole inventory.

#### Resveratrol
**1 × 1 = 1** · OK · trivial · OTC · **SKIP**
**Why:** E1 — failed ITP, poor bioavailability, and the sirtuin mechanism itself is disputed. B1 — none. The Sinclair-era case has not held.

#### Calcium alpha-ketoglutarate (Ca-AKG)
**1 × 1 = 1** · OK · low · OTC · **SKIP**
**Target:** claimed — TCA intermediate; obligate cosubstrate for the TET and JmjC dioxygenases; IL-10 induction · **Measure:** none available — no assay tells you whether an oral dose reached any compartment that matters
**Cautions:** roughly 200 mg elemental calcium per gram of the salt, which counts toward the vegan calcium target rather than against it; GI upset at multi-gram doses; history of calcium oxalate stones is the one condition that makes the calcium load a real question
**Why:** E1 — one unreplicated mouse study and one single-arm human series, against two ITP nulls. B1 — no route to a measurable outcome at 39.

**The mouse result is female-driven, and the ITP has now failed to reproduce it twice.** Asadi Shahmirzadi's *Cell Metabolism* 2020 study fed Ca-AKG to C57BL/6 mice from 18 months of age and reported compression of morbidity — a 46% reduction in frailty and roughly 41% more healthspan — on top of lifespan gains. Those gains were **significant in females only**: median +16.6% and 90th-percentile +19.7% in females, against +9.6% and +12.8% in males, neither of which reached significance. One inbred strain, one site. The ITP then ran the compound in UM-HET3 mice across three sites at two starting ages — first mirroring the 18-month start of the original design, then, after that returned nothing, a 7-month start reported in the April 2026 GeroScience paper. **No lifespan effect in either sex at either starting age.**

That is a harder negative than either of the two comparable rows. Resveratrol has one ITP null; astaxanthin was an ITP *hit* that failed to replicate under protocol variation. Ca-AKG was never an ITP hit at all: the positive finding lives entirely in a single inbred-strain experiment that the field's only blinded, multi-site, genetically heterogeneous arbiter has now contradicted twice. And the direction of the sex effect matters here specifically. Most recent ITP hits are male-only, a quirk this document elsewhere notes happens to favour you; the one positive Ca-AKG lifespan result runs the other way.

**The human evidence is a customer survey with a p-value on it.** Demidenko et al., *Aging* 2021: 42 people who had been buying a commercial Ca-AKG formulation for an average of seven months showed an average 8-year reduction in methylation age (p = 6.5×10⁻¹²). There is no control arm, no randomisation, and no blinding; the cohort is self-selected purchasers; the clock is a proprietary consumer assay; and the product is not Ca-AKG — it is Ca-AKG plus a sex-specific vitamin blend, so nothing in the design can attribute an effect to the molecule in the title. A p-value of that size from a single-arm self-selected cohort is measuring who enrolled, not what the capsule did. The authors state the limitation themselves.

**The mechanism is signed in both directions on this document's central axis.** AKG is the obligate cosubstrate for the TET DNA demethylases and the JmjC histone demethylases, which is where the epigenetic-rejuvenation story comes from, and for the prolyl hydroxylases that degrade HIF-1α. It is also the glutaminolysis product that loads RagB and activates mTORC1 (Duran, 2012) — the opposite of what §5 is trying to do — while the *C. elegans* lifespan result (Chin, 2014) attributes the effect to inhibiting ATP synthase and TOR. A molecule that is claimed to suppress TOR in worms and is known to activate it in mammalian cells has no settled sign, and nothing in the human record breaks the tie.

**Nothing establishes that an oral dose reaches the compartment the mechanism requires.** Enterocytes consume AKG as a preferred fuel, and the one serious human pharmacokinetic effort — dose-finding for AKG as a cyanide antidote — needed 20 g, split and taken with water, to reach roughly 40% bioavailability. Against endogenous TCA flux, a 1 g oral dose is small; no study has shown it raises intracellular or nuclear AKG in any human tissue. The proposed mechanisms all operate on nuclear α-KG concentration, which is the one number nobody has measured after supplementation.

**What would move it.** Two placebo-controlled RCTs are running: ABLE (n=120, 1 g/day sustained-release Ca-AKG versus placebo for 6 months in adults aged 40–60 whose methylation age exceeds their chronological age, with grip and leg strength, arterial stiffness, VO₂ and inflammatory markers as secondaries) and NCT07114536 (12 weeks, PhenoAge primary). Neither has reported. Note what a positive result would and would not buy: a methylation clock is a surrogate with no RCT- or MR-validated causal link to any outcome, so a clean win on the primary endpoint lands at E2–E3, not higher. **The secondary endpoints are the ones worth watching** — grip strength, leg extension and arterial stiffness are the measures that could show the compound doing something to a person rather than to an algorithm.

**The only defensible ingredient in the capsule is the calcium.** On a vegan diet that is a real target with a hard endpoint behind it, and calcium carbonate supplies it at a fraction of the price — the branded AKG formulation runs several hundred dollars a year, bulk powder considerably less, and neither buys anything the ITP could detect.

#### 17-alpha estradiol
**2 × 1 = 2** · MONITOR · low · not practically available · **WATCH, do not take**
**Why:** E2 — a male-specific ITP hit (+19%), genuinely one of the more interesting results in the field. B1 — zero human data.

#### Blood donation 2–3×/yr
**2 × 2 = 4** · OK · low · free · **OPTIONAL**
**Target:** iron, hemodilution · **Measure:** ferritin; hematocrit
**Cautions:** ferritin first on a plant diet — non-heme iron absorbs at a fraction of heme iron and stores refill slowly
**Why:** E2 — observational only. B2 — weak in isolation. Jumps sharply in value if you ever start TRT, where it is the standard erythrocytosis management tool. The vegan case cuts the other way: the mechanism claimed for donation is iron depletion, and a diet that already lowers iron stores is being asked to pay for the same effect twice.

#### Methylene blue
**1 × 1 = 1** · **AVOID** · trivial · Rx
**Target:** mitochondrial electron carrier
**Cautions:** **potent MAO-A inhibitor — serotonin syndrome with any SSRI, SNRI or triptan**
**Why:** E1 — no human aging data. B1 — none. AVOID for the interaction alone: this is a hospitalisation-grade risk, not a caution. It is also the clearest illustration of why safety is a veto flag rather than an averaged term — the drug is cheap and quick to take, so any scoring that averages safety against cost dilutes a hospitalisation risk into a middling number.

#### Bisphosphonates, acipimox, pentoxifylline, azithromycin, piperlongumine, ACE-i/ARB, beta blockers
**1 × 1 = 1** · MONITOR · low · Rx · **change the trigger from "aging" to "diagnosis"**
**Why:** E1 for an *aging* indication — these have good evidence for the diseases they treat and none for healthy 39-year-olds. B1 — no route to benefit absent the diagnosis. Keep the rows, change the trigger condition. The 1 is the score for taking an ARB with normal blood pressure; taking one *because* blood pressure is above target scores in the BP row at 20, and the ITP captopril result is a tiebreaker within that decision rather than a reason to start the drug.

#### Supplement bundle
**1 × 1 = 1** · OK · moderate · OTC · **SKIP**
*(spermidine, urolithin A, ergothioneine, apigenin, carnosine, lithium, C15:0, MitoQ, CoQ10, green tea extract, curcumin, ginger, ashwagandha, melatonin, generic multi-strain probiotics, butyrate, nattokinase, glucosamine, chondroitin, TA-65, Khavinson peptides, plasmalogens, GLYLO)*
**Cautions:** several blunt exercise adaptation; several are CYP inhibitors; nattokinase adds bleeding risk; **high-dose green tea extract carries an idiosyncratic hepatotoxicity signal** — EFSA drew its line around 800 mg EGCG/day, and brewed tea is not the exposure at issue
**Why:** E1 — mechanism-level evidence only, and where ITP has tested these it has mostly returned nulls. B1 — no route to a measurable outcome. Individually harmless, collectively a tax on attention, adherence, liver and wallet. Roughly 35 source rows collapse here.

**Carve-out:** "probiotics" as a *category* belongs here at 1, but specific clinically-tested strain combinations do not. Evidence in this field attaches to named strains at named doses, not to the category — see §3c.

**Three of these are here for an aging indication only, and would move on a different trigger.** CoQ10 is an electron-transport-chain carrier before it is an antioxidant; statins deplete its synthesis, and Q-SYMBIO found a mortality signal in heart failure with reduced ejection fraction. Ergothioneine's distinguishing feature is a dedicated transporter (OCTN1/SLC22A4) and tissue concentration under oxidative load — its case is conditional-deficiency, supported by observational associations between low plasma levels and cardiovascular mortality, not added scavenging capacity. Green tea extract is not usefully an antioxidant *in vivo* at all: catechins are poorly bioavailable and rapidly methylated and glucuronidated, and what survives is hormetic Nrf2 induction plus direct target binding. None of the three has a route to benefit in a healthy 39-year-old, so all three score 1 — but they fail for three different reasons, and only CoQ10 has a diagnosis that would change the answer.

#### EDTA chelation, HBOT, mitochondrial transfusion, stem cells / exosomes / VSELs, follistatin and telomerase gene therapy, flagellin immunisation
**1 × 1 = 1** · **AVOID** · high · medical tourism or unregulated clinics
**Why:** E1 — no human aging evidence. B1 — none. Unregulated administration carries real procedural risk with nothing on the benefit side to justify it.

**The two gene therapies fail on their own genetics as well as on their clinics**, and [genetic-pathways.md](genetic-pathways.md) works both through: follistatin overexpression is unphaseable and irreversible on the axis where the [ActRII antibodies](#myostatin--activin-blockade-bimagrumab-apitegromab) are already only a WATCH, and telomere lengthening runs against the human evidence rather than with it, since long-telomere syndromes (*POT1*, *TERT* promoter) cause melanoma, CLL and glioma.
