# Anti-Aging Therapeutic Inventory

**Target:** healthy male, age 38, US, vegan, currently on tirzepatide
**9 August 2026**
**Source:** AgingBiotech.info "Available Therapeutics" survey table (128 rows)
**Detail rows:** [therapeutics-by-mechanism.md](therapeutics-by-mechanism.md) · **Human genetics behind the targets:** [genetic-pathways.md](genetic-pathways.md)

**How this document is arranged**

1. **Three files.** This one holds the framework, the grouped inventory, the interaction analysis and the two protocol write-ups; the row-level reasoning behind every score lives in [therapeutics-by-mechanism.md](therapeutics-by-mechanism.md); the loss- and gain-of-function variants behind the drug targets, and the somatic editing programs that would install them, live in [genetic-pathways.md](genetic-pathways.md).
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

- **Failed to extend lifespan:** resveratrol, NR, fisetin (−5 to +7%), green tea extract, and eleven further compounds in the April 2026 report — among them alpha-ketoglutarate, nulled at two different starting ages in both sexes.
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

For a US male currently 38, lifetime cause-of-death is dominated by atherosclerotic cardiovascular disease (roughly a quarter), then cancer (roughly a fifth), then dementia, metabolic disease, and — in the next decade specifically — unintentional injury. Nothing on the geroscience list moves those numbers as much as the boring interventions do.

The decisive asymmetry at your age is **exposure-time leverage**. Ference's Mendelian randomization puts 40 years of 1 mmol/L lower LDL-C at a 54.5% lower CHD risk, against roughly 24% per 1 mmol/L for a statin started in mid-life and followed for five years. Same molecule, same target — about **three times the effect** because the clock started earlier. The lifespan version of the same analysis is blunter still: 1 SD higher genetically proxied LDL-C costs about 1.2 years of life, with an odds ratio of 0.72 for reaching the 90th versus the 60th percentile age. Starting ApoB control at 38 rather than 55 is, on its own, plausibly worth more than every supplement in the source table combined.

The same logic runs the other way for the speculative agents: at 38 you have the *most* time for an unrecognized harm to compound. Risk tolerance should be lower now, not higher.

**Exposure-time leverage also cuts a third way.** If risk is an integral of exposure over time, then *duty cycle* is a lever, not just dose. An intervention run six weeks a year carries roughly a quarter of the cumulative exposure of the same intervention run continuously — for benefit and for harm alike. That observation is what makes Part 4 worth taking seriously rather than dismissing.

### Antagonistic pleiotropy and hyperfunction — why the list is age-staged

Two theories do most of the conceptual work in this document, and neither is named in the source table. They are worth stating explicitly, because between them they explain the *shape* of the ranking — not just which items score well, but why so many rows carry a trigger age rather than a yes or a no.

**Antagonistic pleiotropy** (Williams, 1957): selection optimises for reproductive success, so a pathway that pays early is retained even when it charges late. Selection pressure falls away roughly with the reproductive schedule, which puts you at 38 near the top of the fading curve. Three operating rules follow.

*First, the sign of an intervention can flip with age, so "no" and "not yet" are different verdicts and have to be written differently.* Senolytics at 38 are not a bad idea, they are an idea aimed at a burden you have not accumulated — which is why every skip row in this document that is age-conditional carries the condition, and why the trigger belongs in the row rather than in your memory. Nothing on the skip list should require re-deriving from scratch at 50.

*Second, where a trait has no early-life upside, antagonistic pleiotropy has nothing to say — and those are the rows at the top.* Lifetime apoB exposure, blood pressure, tobacco, unintentional injury and Lp(a) are not costs charged for a youth benefit; nothing is being traded away by lowering them at 38. That is a structural reason to be confident about the top of the list and cautious about the middle, independent of the evidence grades. The interventions that pull against a real evolutionary trade-off — everything in the growth arms — are exactly the ones where the trade needs pricing.

*Third, the trade-off is the reason growth cycling exists rather than a permanent anti-growth setting.* Somatotropic signalling is the textbook antagonistically pleiotropic axis: high IGF-1 builds and repairs tissue when tissue is being built, and associates with cancer incidence and shorter life when it is not. At 38 you are near the crossover, which is precisely where a fixed setting in either direction is least defensible and a duty cycle is most.

**Human genetics has run the extreme version of that experiment, and the result is why the anti-growth arm is a phase rather than a setting.** The Ecuadorian Laron cohort carries lifelong growth hormone receptor deficiency, and it has near-total protection from diabetes and near-zero cancer incidence across decades — and **did not live longer**, because other causes filled the gap. That is the single most useful data point in this document for calibrating how hard to push the anti-growth side: it is simultaneously the strongest human evidence that suppressing growth signalling protects against two major killers, and the strongest human evidence that doing so does not straightforwardly buy years. The [GHR/IGF1R row](genetic-pathways.md#24-growth-signalling-and-the-longevity-loci) works this through, and the same asymmetry is what keeps the rhGH block at MONITOR rather than AVOID in both directions.

**Hyperfunction** (Blagosklonny): aging as quasi-programmed continuation of developmental growth programs that were never switched off, rather than accumulated molecular damage. It does not have to be right to be useful — it makes a prediction that is testable against this document's own evidence base, and the prediction has largely held. If aging is driven by excess signalling rather than by damage, then **suppressing the signal should outperform repairing the damage**, and that is what the trial record shows: mTOR and nutrient-sensing interventions carry the best animal lifespan data in the field, while the damage-repair programs — NAD+ repletion, antioxidants, senolytics at low senescent burden — repeatedly raise their biomarker and then fail to move anything downstream. NMN raises NAD+, MK-7 carboxylates matrix Gla protein, NAC raises glutathione, and none of them changes an endpoint. That pattern is the single most useful sorting heuristic on the supplement side of this inventory, and it is why the whole of §2.6's redox and NAD+ families collapse to skip.

**What both theories agree on, and where this document parts company with them.** Both frame aging as something with a cause worth addressing at the root. Neither justifies acting past the evidence: the strongest hyperfunction-derived intervention available to you is rapamycin, and it scores 6, because PEARL missed its primary endpoint and no phase 3 has tested geroprotection in people who are not sick. VITAL-H is the trial that would change that, for rapamycin and the SGLT2 inhibitors simultaneously. The theories tell you where to look and what to discount; they do not substitute for the readout.

**And the honest cost of taking them seriously.** An antagonistic-pleiotropy reading of this regimen finds three places where it is spending youth capital to buy late-life benefit, and they should be named rather than assumed away. Driving fat mass to the bottom of the reference band trades a small metabolic gain against gonadal and skeletal function, which is why the fuel floor in Part 4 is written as symptoms rather than a percentage. Suppressing mTORC1 and IGF-1 for most of the year trades repair capacity against anabolic error. And the GLP-1 that makes the leanness reachable costs lean mass and bone density in direct proportion to the weight it removes. Each of those is a defensible bet at 38 and none of them is free — the measurement plan exists to price them, and the stopping rules exist because the theories cannot say in advance which way any individual case runs.

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

**BENEFIT (1–5) — if the evidence is right, how much does it change *your* outcome at 38?**

| | |
|---|---|
| **5** | Moves a top-two lifetime cause of death, with an effect measured in years; **or** it is load-bearing for the regimen, in the sense that its failure degrades several other rows at once |
| **4** | Moves a top-five cause of death, or a large effect on a moderate one |
| **3** | Meaningful healthspan or function effect |
| **2** | Small or narrow effect |
| **1** | No plausible route to changing your outcomes at 38 |

**SCORE = EVIDENCE × BENEFIT**, integers 1–25.

The second clause on B5 exists because two rows genuinely earn it and neither moves a cause of death by itself. **Resistance training** is the thing that decides whether tirzepatide's weight loss comes off fat or off muscle, which sets whether the GLP-1 row, the bone row and the entire growth-cycling structure work as scored. **Sleep** is the row that, when broken, degrades training output, appetite regulation, mood and blood pressure simultaneously. Those two, and nothing else in this document, are B5 on the second clause — it is a narrow carve-out for prerequisites, not a general licence to promote items that feel important. Cancer screening stays at B4 despite acting on a top-two cause, because the effect is measured in months rather than years: Bretthauer's meta-analysis of 18 long-term RCTs across 2.1 million people found sigmoidoscopy the only screening test with a significant lifetime gain, at 110 days (95% CI 0–274), with colonoscopy, FIT, mammography, PSA and lung CT not reaching significance. That is a real benefit and it is not a B5 one.

**SAFETY is a flag, not a score:** `OK` · `MONITOR` (specific lab or symptom check, named in the row) · `AVOID` (serious harm plausible in your situation — overrides the score entirely).

**EFFORT is a tag, not a score:** `trivial` (<$300/yr and <5 min/wk) · `low` · `moderate` · `high` (>$2,000/yr out of pocket, or >4 h/wk). The thresholds are annual out-of-pocket cost, which is why tirzepatide sits at `moderate` on a covered price and would be `high` on cash, and why a generic pair running ~$300/year stays trivial while bempedoic acid at ~$430–610/month does not.

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
| **12** | 4×3 | DXA bone mineral density | ok | trivial | free on the body-composition scan; vegan diet, the GLP-1 and anti-growth blocks all withdraw from the same tissue |
| **6** | 3×2 | Vitamin D (25-OH) | ok | trivial | VITAL largely null; correcting frank deficiency has better support |
| **6** | 3×2 | hsCRP | ok | trivial | gates the residual-inflammation question |
| **6** | 3×2 | Baseline audiogram | ok | trivial | a baseline to detect drift against |
| **6** | 3×2 | Grip dynamometer | ok | trivial | cheapest weekly readout during any restriction phase |
| **6** | 3×2 | APOE genotype / CAD PRS | ok | low | **GINA covers health insurance but NOT life, disability or LTC** — insure first |
| **5** | 5×1 | Coronary artery calcium | ok | low | *defer to 45–50* — most 38-year-olds score zero and zero doesn't exclude soft plaque |
| **4** | 2×2 | Homocysteine, B12, folate | ok | trivial | only the correct readout if you pursue methionine work |

### 2.1 ApoB and the lipoprotein pathway

The highest-yield family on the list. Four molecular targets, one coherent ladder: **HMG-CoA reductase → NPC1L1 → PCSK9 → apo(a)**. ACL is the same rung as the statin, reached from a different direction.

It is also the only family here whose longevity claim rests on human data rather than mouse data. Mendelian randomisation against parental lifespan puts 1 SD higher genetically proxied LDL-C at 1.2 years shorter life (95% CI −1.55 to −0.87), with an odds ratio of 0.72 for reaching the 90th versus the 60th percentile age; target-by-target, the lipid-lowering alleles of *HMGCR*, *PCSK9*, *APOB* and *LPL* all associate with longer lifespan, and only about 23% of the *LDLR* effect is mediated through coronary disease, so most of it is something broader. Drug-target MR plus observational meta-analysis across ~1M people adds lower dementia risk for *HMGCR*, *NPC1L1* and *CETP*. And it works in people who are well: CTT's 27-trial individual-participant meta-analysis found ~11 fewer major vascular events per 1,000 over five years per mmol/L even at 5-year risk under 10%, with no cancer or non-vascular mortality signal, and a 2026 meta-analysis confined to primary prevention (14 trials, ~98,500 participants) puts the pooled effect at a 30% relative MACE reduction per mmol/L (RR 0.70, 0.67–0.74). No supplement in the source table has anything of this class behind it.

| Score | E×B | Item | Target | Safety | Effort |
|---:|:---:|---|---|:---:|:---:|
| **25** | 5×5 | ApoB to <60 mg/dL *(the target)* | — | monitor | trivial |
| **25** | 5×5 | Rosuvastatin 10 mg, generic | HMG-CoA reductase | monitor | trivial |
| **25** | 5×5 | Evolocumab / alirocumab | PCSK9 (mAb) | ok | high |
| **20** | 4×5 | Inclisiran | PCSK9 (siRNA) | ok | high |
| **20** | 4×5 | Enlicitide (Lipfendra), oral | PCSK9 (macrocyclic peptide) | ok | high |
| **16** | 4×4 | Ezetimibe, generic | NPC1L1 | ok | trivial |
| **16** | 4×4 | Bempedoic acid | ATP citrate lyase | monitor | high |
| **16** | 4×4 | ApoB to <30 mg/dL *(the increment)* | — | monitor | high |
| **8** | 2×4 | Lp(a) agents — pelacarsen, olpasiran, lepodisiran, muvalaplin | apo(a) | ok | high |
| **6** | 3×2 | Red yeast rice / monacolins | HMG-CoA reductase | **AVOID** | trivial |

**Within the PCSK9 subfamily**, all four agents block PCSK9-mediated LDL-receptor degradation. Same target, same downstream effect, four delivery routes. They separate on exactly one axis:

| Agent | Modality | Dosing | E×B | Outcomes trial |
|---|---|---|:---:|---|
| Evolocumab / alirocumab | monoclonal antibody | SC q2wk–q4wk | **25** | **Reported** — FOURIER, ODYSSEY, VESALIUS-CV |
| Inclisiran | siRNA | SC q6mo after loading | **20** | Pending — ORION-4, VICTORION-2P |
| Enlicitide | oral macrocyclic peptide | 20 mg daily | **20** | Pending — CORALreef Outcomes |

Three grading points are worth stating explicitly, because grouping is what makes them visible.

**The monoclonals hold E5 on primary-prevention evidence, not borrowed evidence.** VESALIUS-CV randomised 12,257 patients with no prior MI or stroke and cut 3-point MACE by 25% over a median 4.6 years on top of maximally tolerated statin (HR 0.75, 1.8% absolute), with 4-point MACE down 19% (HR 0.81) and MI alone down 36% (HR 0.64). All-cause mortality ran 7.9% against 9.7%, which the investigators label hypothesis-generating on hierarchical testing rather than a demonstrated mortality benefit. Read the entry criteria before reading any of it across, though: qualifying meant documented atherosclerosis or high-risk diabetes plus LDL-C ≥90 mg/dL. The drug is now proven further than it is *available* to you, and further than it is *needed* by you.

**Inclisiran sits at E4, not E5.** "FOURIER and ODYSSEY established hard-outcome benefit" is a statement about the monoclonals, not about inclisiran. Inclisiran was approved on LDL-C lowering alone and its outcomes trials have not reported. It belongs in the same evidence position as enlicitide.

**Enlicitide also sits at E4, one point below the monoclonals rather than two.** CORALreef Lipids gave 55.8% placebo-adjusted LDL-C reduction and ~50% ApoB reduction, and CORALreef AddOn beat ezetimibe, bempedoic acid and their combination on background statin. Those are surrogate endpoints — but PCSK9-mediated LDL lowering is a surrogate that has been causally validated to outcomes by both RCT and Mendelian randomization, with benefit tracking absolute LDL-C reduction largely independent of the mechanism used to achieve it. A two-point penalty would overstate the residual uncertainty for a same-target agent with an unusually strong class prior.

**On the effort tag:** the binding constraint for every member of this family is prior authorization and cash price, not administration. All four sit at `high` for that reason — enlicitide included, despite listing at ~$315/month against ~$500–600 for the injectables, because the payer criteria are the same across the class: a documented failure of statin plus ezetimibe at a baseline LDL-C at or above 70 mg/dL. Cheapest door into the family is still a ~$3,780/year cash door. But note the ranking that follows if you strip cost out: inclisiran is **two injections a year**, which is a lighter administration burden than a daily pill. The oral advantage over the monoclonals is real; the oral advantage over inclisiran is not.

**Why ACL is the same rung and not the next one.** The 2×2 factorial Mendelian randomization of *ACLY* against *HMGCR* found the two lower LDL-C by the same mechanism, with the same effect on cardiovascular risk per unit LDL-C — genetically, bempedoic acid is a statin with a different binding site two steps upstream in the same pathway. CORALreef AddOn then measured the prediction: on background statin, bempedoic acid reduced apoB by **5.4%**, against 20.2% for ezetimibe, 27.7% for the pair, and 54.6% for enlicitide. Adding it to a statin you tolerate buys almost nothing, because the lever is already pressed — which is also why no hard-outcome trial of the combination exists. CLEAR Outcomes deliberately enrolled the statin-intolerant, and it earned its E4 there on the 13% MACE reduction in the whole trial. The headline prevention number is one level weaker: a *post-hoc* analysis of the 4,206-patient primary-prevention cohort found 27% lower all-cause mortality (HR 0.73, 0.54–0.98) and a 30% reduction in the primary composite — a mortality signal that did not appear in the trial overall, which is the standard reason to treat a subgroup result carefully. It is the best mortality result in this family from anything resembling a prevention population, and it is still post-hoc, in statin-intolerant 68-year-olds, two-thirds of them diabetic. Hence the condition attached to the row: **only if you cannot take a statin.**

**Which statin, and at what dose:** **rosuvastatin 10 mg.** Rosuvastatin is roughly 1.5× atorvastatin milligram-for-milligram (~44–46% LDL-C reduction at 10 mg against ~35–37% for atorvastatin 10 mg), so 10 mg sits around atorvastatin 20–40 mg and is the right opening dose from an untreated baseline. LODESTAR randomised 4,400 people head-to-head for three years and found no outcome difference (8.7% versus 8.2%, HR 1.06), but two signals against rosuvastatin: new-onset diabetes 7.2% versus 5.3% (HR 1.39) and cataract surgery 2.5% versus 1.5% (HR 1.66). The diabetes signal is the one you are already insured against — tirzepatide is moving glycaemia far harder in the protective direction than 10 mg of a statin can move it the other way. What has no offset is the interaction surface: atorvastatin runs through CYP3A4, rosuvastatin does not, and that is the axis the berberine AVOID flag turns on. Atorvastatin 20 mg is a fine substitute on price or stock.

**Sequence:** ApoB + Lp(a) → **rosuvastatin 10 mg and ezetimibe 10 mg together** → reassess ApoB at 8 weeks → escalate within the PCSK9 family only if off target or Lp(a) is high. Both generics together cost under $25/month and get most people to target; reaching for a $6,000/year drug before trying a $300/year one is the definition of a poor bang-for-buck decision. Starting both at once rather than titrating the statin first is what RACING supports, and it tested the exact regimen recommended here: rosuvastatin 10 mg plus ezetimibe 10 mg against rosuvastatin 20 mg alone, n=3,780. The 3-year composite came in at 9.1% against 9.9% (absolute difference −0.78%), non-inferior, while the combination put 72% of patients under LDL-C 70 mg/dL at three years against 58% on monotherapy, with intolerance-driven discontinuation or dose reduction at 4.8% against 8.2%. Two mechanisms at moderate doses beat one at a high dose on tolerability and land lower.

**Why <60 is the commitment and <30 is only a row.** The two targets score differently because the second slice is taken from an already-reduced baseline and costs roughly 13× more per year to reach: both generics together run ~$300/year, and the cheapest PCSK9 inhibitor — enlicitide, at a $315/month list price — is ~$3,780/year, which no payer will cover for you, since the criteria across the class require documented failure of statin plus ezetimibe at a baseline LDL-C you will not have.

Note what is *not* in that reasoning. The relative benefit does not fade at the bottom: trials whose participants started at a median LDL-C of 65.7 mg/dL and reached a median of 21 show the same ~22% reduction in major vascular events per 38.7 mg/dL as trials starting at 131.5, with no threshold and no offsetting harm. Nor is safety the constraint — a 2026 review works through cognition, cancer, haemorrhagic stroke, new-onset diabetes, cataract, hormonal effects and myopathy and attributes none of them to the achieved level. Lower keeps working and lower stays safe; it is the absolute pie that shrinks, and the money that stops being worth it. The corollary runs the other way too: don't back off a lower number the generics hand you for free. Rosuvastatin 10 mg plus ezetimibe lands many people near 45, which is well under the commitment and well over the point where money starts buying the difference. Take it and stop there.

**Where Lp(a) changes it:** if Lp(a) comes back >125 nmol/L — the 2026 guideline's risk-enhancer threshold, carrying ~1.4× risk, with ≥250 nmol/L carrying ~2× — the case strengthens considerably, because statins slightly *raise* Lp(a) while PCSK9 inhibitors lower it ~20–25%. It also puts a fixed floor under your achievable apoB, though a smaller one than the phrase suggests: apoB-100 has a conserved molecular weight of 512 kg/mol, so 1 nmol/L of Lp(a) is ~0.05 mg/dL of apoB — ~4 mg/dL at Lp(a) 75, ~13 mg/dL at 250. Particle counting agrees, with Lp(a) at ~3% of apoB particles on average and ~15% in the top decile. That is a floor worth knowing, not a wall. The reason to care is per-particle potency: Lp(a) is roughly 6-fold more atherogenic per apoB particle than LDL. Lp(a)HORIZON (pelacarsen, n≈8,325) is the first CV outcomes trial for any Lp(a)-lowering therapy; it is event-driven and has run past its guided mid-2026 window, with OCEAN(a) (olpasiran) targeting primary completion in December 2026. **Measuring Lp(a) now costs $30 and tells you whether to care** — and the 2026 guideline makes it a once-in-a-lifetime test for everyone, not a specialist add-on.

**Where the 2026 ACC/AHA guideline puts a healthy 38-year-old.** Its frame is "lower sooner": PREVENT 10-year *and* 30-year risk, universal one-time Lp(a), CAC promoted to Class 1 for reclassification, and apoB used to intensify therapy when LDL-C is already at goal. Its apoB goals are <55, <70 or <90 mg/dL by risk tier, making <70 the primary-prevention number. The clause that applies at your age is explicit: in adults 30–59 with low 10-year risk, a moderate-intensity statin is reasonable when LDL-C is 160–189 mg/dL **or 30-year ASCVD risk is ≥10%**. The <60 target used throughout this document is deliberately tighter than guideline, and it is bought with cumulative exposure rather than 10-year risk — which is the same logic the guideline itself adopted when it added the 30-year horizon. Run PREVENT for both horizons; the 30-year number is the one that will argue your case.

### 2.2 Incretin and glucose handling

| Score | E×B | Item | Target | Safety | Effort |
|---:|:---:|---|---|:---:|:---:|
| **16** | 4×4 | Tirzepatide *(continue)* | GLP-1 / GIP receptor | monitor | moderate |
| **9** | 3×3 | Pasteurized *A. muciniphila* (MucT) *(watch)* | Amuc_1100 / gut barrier | ok | moderate |
| **6** | 3×2 | Empagliflozin / canagliflozin | SGLT2 | monitor | low |
| **6** | 3×2 | Retatrutide *(watch)* | GLP-1 / GIP / glucagon receptor | monitor | moderate |
| **4** | 2×2 | Pendulum Glucose Control (WBF-011) | live multi-strain / SCFA → endogenous GLP-1 | ok | moderate |

**The two incretin agents, side by side.** Retatrutide adds glucagon receptor agonism to tirzepatide's GLP-1/GIP, and it wins decisively on the one endpoint you are not taking an incretin for: 28.3% mean weight loss at 80 weeks in TRIUMPH-1, against roughly 20–22% for tirzepatide in SURMOUNT-1. What separates the scores is everything else. Tirzepatide holds E4 because SELECT established MACE and all-cause mortality benefit for the class in non-diabetic adults — though in adults who already had cardiovascular disease, which is why SURMOUNT-MMO rather than SELECT is the readout that would take this to E5; retatrutide's own outcomes trial does not complete until February 2029, and the glucagon arm is exactly the reason that class inference does not transfer cleanly in the meantime. So the newer drug is an evidence step *down* bought with an endpoint that this regimen spends a protein floor, a lifting schedule and a DEXA stopping rule defending against. The number that would decide a switch is the body-composition split, and it is not published.

**The SGLT2 subfamily, in one place.** The source table ranked this #1 on a 12/12 gerotherapeutics score with the note "top scoring candidate for TAME-like trial." That note is doing more work than it appears: **the score means "most deserving of a trial," which entails that the human aging evidence does not yet exist.**

What the evidence supports is nonetheless the strongest non-tirzepatide case in this section. ITP canagliflozin gave **+14% median lifespan in males only**, no effect in females — the largest male effect in ITP history, concordant across all three test sites, with 90th-percentile survival up 9%. It happens to be your sex. On the human side the decisive detail is easy to miss: **DAPA-HF, DAPA-CKD and EMPA-KIDNEY enrolled non-diabetics, and the benefit held in that subgroup.** Whatever SGLT2 inhibition is doing, it is not simply lowering glucose in the hyperglycemic. Large cohorts add a consistent ~30% reduction in dementia incidence versus DPP-4 inhibitors, replicated across several meta-analyses — observational, confounded by indication, but pointing the same direction.

What still caps it at E3: every trial is in **type 2 diabetes, heart failure, or chronic kidney disease**, where a substantial part of the benefit is hemodynamic and renal, and none is in metabolically healthy adults.

B2 is the binding constraint, not E. You have no heart failure, no CKD, no diabetes, and ApoB is being handled by a statin. The population where this drug has proven itself is the population you are trying not to join, and the metabolic benefit you'd be reaching for is largely what tirzepatide is already delivering with hard-outcome data behind it.

What it costs: genital mycotic infection in roughly 1 in 10 men, volume depletion and orthostasis, 20–40 g/day glucosuria, Fournier's gangrene (rare but labeled), and euglycemic ketoacidosis.

**Why MONITOR rather than AVOID.** Ketoacidosis risk tracks relative insulin deficiency, not body weight and not the GLP-1 by itself. In DAPA-HF and DAPA-CKD, ketoacidosis events occurred **only** among participants with type 2 diabetes — none among the non-diabetic participants, across several thousand patient-years — and the T2D trial base rate is 0.6–2.2 events per 1,000 patient-years. Euglycemic ketoacidosis in true non-diabetics is real and has its own case literature, but it is rare and nearly always precipitant-driven: fasting, ketogenic diet, surgery, dehydration, acute illness, impaired renal ketone clearance. Being lean is not itself protective — the published SGLT2i-plus-tirzepatide case is a 35-year-old man with a BMI of 20.7, five weeks into the combination, tipped over by nausea and poor intake.

**The real incompatibility is fasting, not the anti-growth block** — see Part 3. An SGLT2 inhibitor is a caloric-restriction mimetic and belongs conceptually in an anti-growth phase; what it cannot share a calendar with is the FMD cycles inside that phase, or any tirzepatide week with vomiting or minimal intake. Those are choices, so this is an either/or rather than a permanent exclusion: run the fasting cycles or run the drug. The two are not equivalent halves of that choice — the drug holds the anti-growth state continuously and the cycles supply the transitions, which is the distinction Part 4 is built on. The dietary methionine work can share the calendar with it, but is not quite neutral either: sulfur amino acid restriction raised β-hydroxybutyrate by 117 µmol/L against controls over 8 weeks in humans, which is a small push in the same direction rather than none.

**Which agent.** The lifespan data is canagliflozin; the cleaner human safety record is empagliflozin, which carries no CANVAS-style amputation signal. You cannot have both, and the amputation signal is human evidence while the lifespan signal is mouse.

**When the calculus changes:** if you ever develop type 2 diabetes, CKD, or heart failure, SGLT2 inhibitors become first-line and genuinely excellent. Keep the row, change the trigger from "aging" to "diagnosis."

**On the microbiome pair:** these are two separate rows, because the product and its headline ingredient are on different trajectories. Pendulum is a 0.6% HbA1c agent tested in T2D on metformin, whose mechanism — SCFA-driven *endogenous* GLP-1 secretion — is the pathway tirzepatide already saturates pharmacologically, and its trial was authored end to end by seventeen company employees with no independent replication six years on. Its entire published record is *BMJ Open Diabetes Res Care*, *JMIR Formative Research* and *BMC Microbiology*; the *Nature Medicine* and *Cell Metabolism* trials people associate with the brand are not trials of this product. Pasteurized MucT is a different preparation with three RCTs behind it, including Mount et al. (*Nature Medicine*, 2026, n=90, run across Maastricht, Copenhagen and Wageningen and funded by the manufacturer), which is the only positive RCT anywhere on this inventory aimed at **post-weight-loss regain** — the one problem GLP-1 users actually face. Buying Pendulum does not get you the trial you just read about. Skip it now; put pasteurized MucT on the taper plan.

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
| **2** | 2×1 | Methionine source shifting *(protein constant)* | amino acid composition — SAM/SAH, FGF21, IGF-1 | ok | low |
| **1** | 1×1 | Methionine restriction <1 g/day, 5 days/week | SAM/SAH, FGF21, IGF-1 | **AVOID as specified** | moderate |
| **1** | 1×1 | Methioninase (oral rMETase) | methionine degradation | **AVOID** | moderate |

Everything here pushes the same direction: down-regulate mTORC1 and IGF-1 signalling, favour autophagy and catabolic housekeeping, reduce the substrate available for anabolic error. This is the arm your hypothesis calls the pruning phase, and the framing is fair.

Three things are worth flagging inside the family. **Rapamycin's ~62 h half-life is an argument for block scheduling rather than weekly dosing** — five half-lives is about 13 days, so weekly dosing never cleanly separates from a 3×/week lifting schedule, while a block structure separates them completely. Bitto 2016 (*eLife*) found transient 3-month rapamycin in middle-aged mice produced persistent lifespan benefit, which is the pharmacological precedent for pulsed use.

And **FMD is already a cycle protocol** — 5 days on, then refeeding, a few times a year. Its score of 4 understates its relevance to Part 4, because it is the only item in this family with human trial infrastructure built around alternation rather than continuous administration. It is also the only item here that is a transition rather than a state: everything else in the family holds mTORC1 and IGF-1 down for as long as it is administered, where a fasting cycle depletes and then repopulates. Part 4 turns on that distinction, and it is why an SGLT2 inhibitor taken in place of these cycles is not the same block with a different lever.

**The methionine rows all score low, for two different reasons.** The sub-gram protocol and methioninase score 1 because they aim past the far edge of Longo's curve, where too little methionine causes frailty. Source shifting scores 2 for the opposite reason: on a vegan baseline there is nothing left to shift. Vegan methionine intake already runs 0.88 g/day against 1.67 for meat-eaters, and the one adequately powered human trial — 8 weeks, n=59, both arms on plant-based whole foods — separated the arms by *adding* methionine and cysteine to the control and still found no IGF-1 effect, no FGF-21 effect, no fat-mass effect, and more fat-free mass lost in the restricted arm. The restricted arm of that trial is an ordinary vegan diet. You are eating it already, in both phases.

Two practical consequences follow. Methionine work is **not** a substitute for the fasting cycles, and cannot carry an anti-growth block on its own: the FGF21 and IGF-1 mechanisms overlap in rodents at deficiency-grade doses, but at achievable intakes the human trial shows neither moving, and nothing in the dietary-composition literature touches the hematopoietic and immune reconstitution that fasting/refeeding produces. It is **largely** compatible with an SGLT2 inhibitor, since composition at constant calories and carbohydrate is not a ketoacidosis precipitant — though restriction did raise β-hydroxybutyrate 117 µmol/L in that trial, so the pairing is low-risk rather than no-risk. Methionine work runs in the anti-growth block either way; it is not the variable in the choice below, and it is not load-bearing.

### 2.5 GH / IGF-1 and anabolism — the pro-growth arm

| Score | E×B | Item | Target | Safety | Effort |
|---:|:---:|---|---|:---:|:---:|
| **15** | 3×5 | Resistance training 2–3×/wk | mTORC1, myonuclear addition, bone loading | ok | moderate |
| **12** | 3×4 | Protein 1.2–1.6 g/kg/day, distributed | muscle protein synthesis | ok | trivial |
| **9** | 3×3 | Creatine monohydrate 5 g/day | phosphocreatine, cell hydration | ok | trivial |
| **6** | 2×3 | **Block-periodized growth cycling** *(training-led, no rhGH)* | phase separation of mTORC1/IGF-1 | ok | moderate |
| **4** | 4×1 | Testosterone (absent hypogonadism) | androgen receptor | monitor | moderate |
| **4** | 2×2 | Myostatin/activin blockade (bimagrumab, apitegromab) | ActRII — myostatin, activin A | monitor | high |
| **2** | 1×2 | rhGH-containing pro-growth block (TRIIM/TRIIM-X style) | thymus regeneration; GH/IGF-1 axis | monitor | high |

This section is the counterweight to 2.4. Muscle and bone maintenance, tissue repair, immune reconstitution and wound healing all require anabolic signalling. A protocol that suppresses it continuously is buying protection from one set of failure modes by accepting exposure to another — sarcopenia, osteopenia, impaired repair, blunted immune reconstitution. That cost is real and it belongs in the ledger.

Note the internal ranking. **The best pro-growth intervention here is resistance training at 15, and the second is protein at 12.** Both are free, both are better evidenced than anything else in the family, and both are already on your do-now list. Any pro-growth phase you construct should be built on those two; the pharmacology is optional garnish on top of a foundation that carries the actual evidence.

**The muscle-preserving antibodies are the family most likely to be mistaken for a fit.** ActRII blockade aims at precisely the metric this protocol is judged on — lean mass held through GLP-1 weight loss — which is the reason to watch the class and also the reason it cannot be added to the structure. It raises ALMI on its own and cannot be phased out of an anti-growth block, so it would take the DEXA series, which is the only instrument the cycle has, and make it unreadable. It scores 4 rather than lower because the effect is real and the trials are clean; 4 rather than higher because training, protein and creatine already cover the same axis for free, and the antibody only earns consideration where those have measurably failed.

Three items are worth reading in full in the detail file: [block-periodized growth cycling](therapeutics-by-mechanism.md#block-periodized-growth-cycling-training-led-no-rhgh), [the rhGH block](therapeutics-by-mechanism.md#rhgh-containing-pro-growth-block-triim--triim-x-style) and [myostatin/activin blockade](therapeutics-by-mechanism.md#myostatin--activin-blockade-bimagrumab-apitegromab). The first two are argued out in Part 4.

### 2.6 Everything else, by family

**Senescence** — D+Q (1, monitor, skip) · fisetin (1, ok, skip). Senescent-cell burden at 38 is low; there is little to clear. Right idea, wrong decade. Note that senolytics are *already* designed as intermittent hit-and-run agents, and if you ever run growth cycling they belong at the end of an anti-growth block, immediately before the regenerative phase.

**NAD+** — NMN / NR (2, ok, skip). Human trials raise NAD+ without downstream functional benefit. Three source rows for one pathway.

**Redox and hormesis** — omega-3 (6, continue) · sauna (4, optional) · astaxanthin (2, skip — an ITP hit that failed to replicate) · NAC/GlyNAC/glutathione (2, skip) · cold water immersion (2, skip as a therapy — and if you do it for enjoyment, it belongs in anti-growth blocks, because post-training cold blunts hypertrophy and strength while leaving endurance adaptation intact). Organizing principle: the ROS burst after training is signal, not damage. Every item here is a timing question rather than a yes/no question — except NAC with methionine work, which is a genuine cancellation rather than a timing issue.

**Hemodynamic and vascular** — blood pressure, aiming 105–115 systolic and adding a drug over 120 (20, monitor — the threshold is where the trials stopped, the aim is where the epidemiology and the unwesternised populations sit) · cardiorespiratory training (20, also listed under 2.3) · aspirin (5, **AVOID** — a high evidence score attached to a finding of no benefit; ASPREE showed net harm in healthy older adults) · vitamin K1/K2 (2, skip — the best mechanism of any supplement here, and the clearest illustration that a mechanism is not a result: MK-7 carboxylates matrix Gla protein exactly as predicted, and the calcification endpoint does not move).

**Inflammation** — low-dose colchicine (2, skip — CLEAR SYNERGY/OASIS-9 was neutral at n=7,062) · dental/periodontal care (4, do anyway).

**Immune and infectious** — Shingrix (12, **calendar item at 50**) · H. pylori test-and-treat (8) · hepatitis C one-time screening (8) · influenza vaccination (8) · HPV vaccination (8, **window shuts at 45**).

**Neurological, sensory, mental health** — depression screening and access (16 — suicide is among the leading causes of death for US males 35–44, and its absence from every longevity list is the same blind spot that omits seatbelts) · sleep 7–9 h (15) · **sleep regularity, same bed and wake time seven days a week (12)** · hearing protection (9) · social connection (9). Regularity is a separate row from duration because in the only large study with objective exposure measurement it **outpredicted duration** — 60,977 UK Biobank participants, 20–48% lower all-cause mortality across the top four regularity quintiles. Once 7–9 hours is met, consistency is the remaining lever, and it is free.

**Diet composition** — alcohol minimal or none (12 — MR has dismantled the J-curve) · fiber 35–40 g/day (9) · vegan adequacy items: B12, **calcium**, algal EPA+DHA, iodine, taurine, and ferritin/zinc/selenium monitoring (unscored — these prevent deficits the diet creates rather than extending anything, and the scoring model does not apply to them). **Calcium is the one with a hard endpoint behind it**: vegan hip fracture runs at HR 2.31 in EPIC-Oxford, and among participants clearing ~525 mg/day the rate ratio is 1.00 — the excess sits in the intake rather than in the diet. **Vitamin K1 is conditional rather than automatic** — greens supply it, veganism does not, so a low-greens plant diet can sit under the AI without that constituting a deficiency.

**Environmental and external-cause** — nicotine and tobacco: none (25, confirm) · injury prevention (16) · radon test (12) · sun protection (8) · bedroom HEPA (6) · microplastic exposure reduction (4 — one prospective study with an HR of 4.53 and a contamination-control problem serious enough to cap it at E2; the actions are free, so the weak evidence does not have to carry much).

**Early detection** — cancer screening on schedule (20) · multi-cancer early detection blood tests (3, skip) · whole-body MRI (1, skip). The two consumer screening products fail for the same reason and it is not assay quality: at 38 the base rate is low enough that positive predictive value collapses regardless of specificity. NHS-Galleri is now a real RCT — 142,250 participants, four-fold higher detection, fewer stage IV diagnoses — and it **missed its primary endpoint**, which is the distinction between finding more cancer and preventing death from it.

**No credible mechanism, or not yet reachable** — **carnitine in every ester, including acetyl-L-carnitine (2, monitor, skip — and the one item here that fails the vegan-adequacy test taurine passes)** · taurine (1, premise retracted by Fernandez 2025; it stays in the regimen on a vegan diet as nutritional repletion, which is an adequacy argument rather than a gerotherapeutic one) · resveratrol (1) · **Ca-AKG (1, skip — the single positive mouse study was female-only in one inbred strain, and the ITP nulled it in both sexes at two starting ages; the human data is a 42-person single-arm survey of buyers of a multi-ingredient product)** · 17α-estradiol (2, watch, do not take) · blood donation (4, optional) · **partial epigenetic reprogramming (4, watch — the field's largest bet, mouse-only for systemic use, and the clinics selling it now are an AVOID)** · methylene blue (1, **AVOID** — MAO-A inhibitor) · disease-indication drugs with no aging indication (1, change trigger to diagnosis) · the ~35-row supplement bundle (1) · EDTA/HBOT/stem cells/gene therapy (1, **AVOID**).

**Carnitine is the interesting one in that list, because the case for it is the best-argued of any supplement here and it still loses.** Ames's ALCAR-plus-lipoic-acid work restored mitochondrial function, activity and memory in old rats, which is more than resveratrol or NMN ever managed — but the endpoint was function, not lifespan, the lab held the patent and founded the company selling the combination, and an independent mouse cohort found no lifespan effect. Two facts then close it for you specifically. Acetyl-L-carnitine does not escape the TMAO pathway: its bioavailability is 7.7-fold *lower* than plain carnitine, so more of the dose reaches the microbes, and ~90% of either ester returns as TMAO. And the vegan microbiome's near-immunity to that conversion — a real 20-fold advantage on a single challenge — is exactly what chronic supplementation trains away. It sits at 2 rather than 1 because the human trials in depression and diabetic neuropathy are real; those are diagnoses, not an aging indication.

### 2.7 Flat ranked list

Score-ordered, all families collapsed.

| Score | Item | Family | Safety | Effort |
|---:|---|---|:---:|:---:|
| 25 | ApoB *(measure)* | diagnostics | ok | trivial |
| 25 | ApoB to <60 mg/dL | lipoprotein | monitor | trivial |
| 25 | Rosuvastatin 10 mg | lipoprotein | monitor | trivial |
| 25 | Evolocumab / alirocumab | lipoprotein (PCSK9) | ok | high |
| 25 | Nicotine and tobacco: none | environmental | ok | trivial |
| 20 | Blood pressure to 105–115 | vascular | monitor | trivial |
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
| 16 | Bempedoic acid *(if statin-intolerant)* | lipoprotein | monitor | high |
| 16 | ApoB to <30 mg/dL | lipoprotein | monitor | high |
| 16 | Tirzepatide *(continue)* | incretin | monitor | moderate |
| 15 | Sleep 7–9 h | neurological | ok | trivial |
| 15 | Resistance training 2–3×/wk | anabolic | ok | moderate |
| 12 | Alcohol minimal or none | diet | ok | trivial |
| 12 | Protein 1.2–1.6 g/kg/day | anabolic | ok | trivial |
| 12 | Radon test | environmental | ok | trivial |
| 12 | Shingrix *(at 50)* | immune | ok | low |
| 12 | VO₂max *(measure)* | diagnostics | ok | low |
| 12 | DXA bone mineral density *(measure)* | diagnostics | ok | trivial |
| 12 | Sleep regularity | neurological | ok | trivial |
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
| 6 | Retatrutide *(watch)* | incretin | monitor | moderate |
| 6 | Red yeast rice | lipoprotein | **AVOID** | trivial |
| 5 | Coronary artery calcium *(defer)* | diagnostics | ok | low |
| 5 | Aspirin | vascular | **AVOID** | trivial |
| 4 | Metformin · TRF/FMD · sauna · blood donation · dental · homocysteine panel | various | ok–monitor | trivial–moderate |
| 4 | Pendulum Glucose Control | incretin | ok | moderate |
| 4 | Testosterone (absent hypogonadism) | anabolic | monitor | moderate |
| 4 | Myostatin/activin blockade *(watch)* | anabolic | monitor | high |
| 4 | Microplastic exposure reduction | environmental | ok | trivial |
| 4 | Partial epigenetic reprogramming *(watch)* | no credible mechanism yet | **AVOID clinics** | high |
| 3 | Multi-cancer early detection blood test | early detection | ok | high |
| 2 | Astaxanthin · NAC/GlyNAC · NMN/NR · 17α-estradiol · colchicine · vitamin K1/K2 · methionine via food · cold water immersion · carnitine / ALCAR | various | ok–monitor | trivial–moderate |
| 2 | rhGH-containing pro-growth block | anabolic | monitor | high |
| 2 | Berberine | AMPK | **AVOID** | trivial |
| 1 | Fisetin · resveratrol · taurine · Ca-AKG · D+Q · supplement bundle · disease-indication drugs · whole-body MRI | various | ok–monitor | trivial–high |
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

**The choice is not between equals, though the safety statement is symmetric.** An SGLT2 inhibitor holds the anti-growth state continuously; an FMD cycle is a transition. Taking the drug removes the transitions from the year rather than replacing them, which is a design cost the ketoacidosis arithmetic says nothing about. [Part 4.5](#45-a-concrete-calendar-if-you-run-it) works through what it comes to.

**2. Methylene blue + any serotonergic agent** (SSRI, SNRI, triptan, MAOI) → serotonin syndrome. Methylene blue is a potent MAO-A inhibitor. Hospitalization-grade, not a caution.

**3. Berberine + rapamycin / statins / tadalafil** → berberine inhibits CYP3A4 and P-glycoprotein, raising exposure to all three unpredictably.

**4. Quercetin + dasatinib** → quercetin is itself a CYP3A4 inhibitor and raises dasatinib exposure. The senolytic protocol pairs them deliberately; the interaction is real regardless.

**5. Aspirin + fish oil + nattokinase** → additive bleeding risk with no offsetting indication at your age.

**6. GLP-1 agonist + procedures under anesthesia** → retained gastric contents and aspiration risk. Tell any surgeon, dentist or endoscopist that you are on one; that part is unconditional. What follows from it is not a blanket hold. The 2024 multisociety guidance — AGA, ASMBS, ISPCOP and SAGES — replaced the earlier stop-everything position with risk stratification and shared decision-making between you, the proceduralist and whoever prescribes it. Holding is indicated where risk is elevated: the dose-escalation phase rather than maintenance, higher doses, weekly formulations, active nausea, vomiting or constipation, and comorbid gastroparesis or bowel dysmotility. Where it is indicated the interval is the day of surgery for daily agents and **a week for weekly ones, which is what tirzepatide is** — and weekly dosing is itself one of the listed risk factors. The alternatives to holding are a clear-liquid diet for at least 24 hours beforehand and rapid-sequence induction, with point-of-care gastric ultrasound where it is available. The reason this matters rather than being someone else's protocol: a reflexive week-long hold is not free either, and the guidance exists because the metabolic cost of stopping has to be weighed against the aspiration risk rather than assumed away.

**6b. ARB + fasting cycles → hold the drug, not the fast.**
This one is created by the regimen itself and is easy to miss because the SGLT2 discussion absorbs all the attention paid to fasting interactions. RAS blockade works by removing the angiotensin II-mediated efferent arteriolar tone that defends glomerular filtration when renal perfusion falls, which makes it the antihypertensive class whose harm profile depends directly on volume status. A five-day FMD cycle supplies low intake, low sodium and natriuresis on top of a systolic already being driven toward 105–115. Hold telmisartan through any FMD cycle and any tirzepatide week with vomiting or poor intake, and restart with normal eating — the fast is lowering the number by itself, so the held days need no substitute. Symptomatic orthostasis during a fast on an ARB is a reason to stop the fast rather than push through it. Unlike conflict 1, this is a hold rule and not an either/or: the ARB and the fasting cycles can coexist on the calendar, just not in the same week.

**7. NAC or GlyNAC + methionine restriction → mutually cancelling.**
Cysteine supplementation reverses essentially the entire metabolic phenotype of methionine restriction in rodents — adiposity, hepatic SCD1 expression, insulin, leptin, triglycerides, adiponectin all revert to control. Elshorbagy's conclusion was that the anti-obesity effects of MR are driven by **low cysteine**, not low methionine per se.

This one is listed as hard rather than phase-based deliberately. You could in principle alternate them, but there is no reason to: the cancellation is complete, neither has outcome evidence, and running both in alternation would be funding opposite sides of the same experiment on a schedule instead of simultaneously.

**8. Myostatin/activin blockade + block cycling → the scheduling fix is unavailable, and the instrument breaks.**
ActRII blockade is an anabolic drug given intravenously with a half-life in weeks. Every other pro-growth item in this document can be confined to a pro-growth block; this one cannot, so an anti-growth block run alongside it is anti-growth in diet and training and pro-growth in pharmacology. That is why it sits here rather than under phase conflicts — the conflict is real and the usual remedy does not reach it.

The second half is measurement. ALMI is doing double duty as the stopping rule and as the evidence that the cycle works at all, and an agent that raises ALMI independently of training makes a healthy-looking number compatible with a block that is failing. Grip strength and the training log survive as unconfounded readouts, which is a weaker instrument than the DEXA series it would displace — and weaker in the specific way the class's history warns about, since bimagrumab's sarcopenia and inclusion-body-myositis trials added mass without moving function.

### Phase conflicts — real, but scheduling problems rather than exclusions

None of these is a reason not to combine two interventions at all. What each says is *do not run these in the same window*.

**9. Rapamycin + resistance training.**
A single oral dose of rapamycin before resistance exercise **completely blocked** the contraction-induced rise in human muscle protein synthesis (~40% in controls), with S6K1 phosphorylation flat versus a 6-fold rise in controls. Notably, rapamycin did *not* affect post-absorptive protein metabolism — it specifically suppresses the *response to a stimulus*.

The half-life is roughly 62 hours, so five half-lives is about 13 days. **Weekly dosing cannot separate from a 3×/week lifting schedule — but a block structure separates them completely.** The correct conclusion is not "don't use rapamycin," it is "weekly dosing is the wrong administration pattern if you also lift." If you run it, run it inside an anti-growth block with the last dose ≥2 weeks before training volume comes back up.

Note the scores: resistance training 15, rapamycin 6, so on the merits training wins any contest for the same window. Cycling means you don't have to hold that contest.

**10. Metformin + exercise training.**
Same structure, easier fix. Metformin blunts VO₂max and mitochondrial adaptation, and the intervention with the evidence (cardiorespiratory training, 20) loses to accommodate the one without it (metformin, 4). Metformin's half-life is ~6 hours, making it the most cleanly phaseable item in the document. It still scores 4 — good schedulability is not evidence.

**11. High-dose antioxidants + exercise training.**
NAC, high-dose vitamin C/E, MitoQ, astaxanthin. The ROS burst after training is signal, not damage; suppressing it suppresses the adaptation. This is a *window* problem at the scale of hours, not a block problem — keep antioxidants away from the post-training window, or drop them. Given that none of them have outcome evidence, dropping them is simpler.

**11b. Cold water immersion + resistance training.**
The same mechanism arriving by temperature rather than by chemistry, and the one that most cleanly fits the calendar. Post-exercise cold blunts the satellite cell and p70S6K response acutely and reduces strength and hypertrophy gains over 12 weeks against active recovery, while leaving endurance adaptation intact or slightly improved. So the conflict is specific to the pro-growth block and to lifting days, not to cold exposure generally. Cold plunging belongs in anti-growth blocks, where cardio carries the emphasis and hypertrophy is not being pursued, and out of pro-growth blocks entirely. Sauna does not carry this problem and is the better-evidenced of the two, which makes it the better choice if only one is happening for enjoyment.

**12. IGF-1-raising agents + mTOR/IGF-1-lowering agents.**
The general case, and the one your hypothesis is aimed at. rhGH raises IGF-1; rapamycin, methionine restriction and the CR mimetics exist to lower it and to lower mTOR signalling. Run simultaneously, you are paying two premium prices to push one dial in opposite directions, and then measuring the result with an epigenetic clock that cannot tell you which one won.

Run in **alternating blocks**, that objection largely dissolves, and what remains is a real question about whether the alternation itself is beneficial. That question is Part 4.

### Redundancies — you're paying twice for one mechanism

- NAC + glutathione + GlyNAC (NAC is the precursor; pick one)
- NMN + NR + niacin (same pathway)
- Statin + red yeast rice (same molecule)
- **Statin + bempedoic acid** (same pathway, two steps apart — MR shows *ACLY* and *HMGCR* lowering LDL-C by the same mechanism with the same risk effect per unit, and on background statin bempedoic acid moves apoB only 5.4%). **Nexlizet** is this redundancy sold as a fixed-dose tablet with generic ezetimibe attached: ~$430–610/month against ~$10 for the half that is doing the work
- MitoQ + astaxanthin + CoQ10 (three lipid-phase scavengers; the chemistry differs — MitoQ is not an ETC carrier and is not a CoQ10 substitute — but they fail together if oxidative damage isn't rate-limiting, and they share the exercise-timing problem above). CoQ10's real case is statin depletion or a cardiac diagnosis, not aging: change the trigger rather than stacking it.
- Glucosamine + chondroitin (weak individually, not additive)
- Multiple simultaneous senolytics
- Pendulum + separately-purchased *Akkermansia* (different preparations, overlapping intent — pick the one with the trial you actually want)

### Synergies worth noting

- **Statin + ezetimibe** — different mechanisms, additive ApoB reduction, both generic. Best value pairing in the document, and worth starting together rather than in sequence: in RACING the moderate-dose pair put 72% of patients under LDL-C 70 mg/dL against 58% on high-intensity statin alone, with intolerance-driven discontinuation at 4.8% against 8.2%.
- **Resistance training + adequate protein + creatine** — the only combination that reliably protects lean mass during GLP-1 weight loss, and the foundation of any pro-growth phase.
- **PCSK9 inhibitor + statin** — statins slightly *raise* Lp(a); PCSK9 inhibitors lower it ~20–25%. Complementary if Lp(a) is elevated.
- **Senolytic at the end of an anti-growth block, immediately before a regenerative phase** — clear, then rebuild, which is the sequence the underlying biology suggests. Sensible design; does not make either senolytic worth taking at 38.
- **TRT + blood donation** (if TRT ever applies) — donation is the standard management for TRT-induced erythrocytosis.

### Monitoring requirements

| Agent | Watch |
|---|---|
| Rapamycin | Lipids, fasting glucose, CBC, mouth ulcers, wound healing before any surgery |
| Metformin | B12 annually |
| GLP-1/GIP | **DEXA FMI, ALMI and VAT** against the 2.5–3.5 / ≥8.5 kg/m² / <50 cm² target; **BMD on the same scan**, Z-score above −1.0 and stable; **the fuel floor** — total testosterone ≥500 ng/dL, libido, sleep, training output; gallbladder symptoms; declare it before any procedure under sedation, where the hold is risk-stratified rather than automatic |
| Telmisartan or any ARB | Potassium and creatinine after starting; **hold for FMD cycles and any week of poor intake**; note that creatine supplementation raises creatinine without changing filtration — cystatin C settles an unexpected result |
| SGLT2i (if used) | Home β-hydroxybutyrate meter; genital mycotic infection; volume status. **Hold for any illness with poor oral intake, any fasting or FMD cycle, and 3 days pre-procedure** |
| Statin | ALT at baseline and once; CK only if symptomatic |
| rhGH (if ever) | IGF-1, fasting glucose and insulin, PSA, carpal tunnel symptoms, joint swelling |
| Any growth-cycling protocol | DEXA at every phase boundary; grip weekly; IGF-1 and fasting insulin at phase midpoints, where the block-to-block difference is the amplitude of the swing rather than a reading taken mid-transition |
| Any FMD cycle | Protein logged back to 1.6 g/kg/day within 48 h of the refeed — the gate on running the next one |

---

## Part 4 — Growth cycling

**Your hypothesis, as stated:** the anti-growth interventions — rapamycin, fasting, calorie and protein restriction, senolytics — are about pruning senescent cells, avoiding cancer, and getting into an efficient metabolic state that limits byproducts. But growth also matters, for muscle and bone preservation, tissue repair, and thymic regeneration. So rather than running one arm continuously, alternate: a ~6-week pro-growth block (TRIIM-X, heavy strength training, high protein, all anti-growth items suspended), then return to a mostly anti-growth lifestyle with reduced-volume training.

**The structural claim is sound.** Treating pro- and anti-growth as permanently opposed would justify an AVOID flag on TRIIM-X and a rejection of your methionine plan on scheduling grounds — but both of those arguments are about *simultaneity*, and both weaken considerably once the two arms are separated in time. The scoring below prices them that way.

What follows separates the hypothesis into three parts, because they have different evidence and deserve different answers: **the cycling structure**, **the pro-growth phase content**, and **the rhGH question specifically**.

### 4.1 What supports the cycling structure

Nothing here is a trial of block alternation itself — that trial does not exist. What exists is a set of adjacent results that make the structure mechanistically credible rather than merely appealing.

**Pulsed mTOR inhibition already has a precedent.** Bitto et al. (*eLife*, 2016) gave middle-aged mice rapamycin for three months and found lifespan benefit that persisted after withdrawal. Weekly rapamycin dosing in humans is itself a pulse strategy, adopted specifically to get mTORC1 inhibition without continuous immunosuppression. The field's own dosing convention concedes that continuous is not obviously better.

**Fasting protocols are already cycle protocols, and the refeeding phase does work.** Longo's FMD design is 5 days on, then refeeding, a few times a year — the alternation is the intervention, not a compromise. And the refeeding phase is not downtime: Cheng et al. (*Cell Stem Cell*, 2014) found that fasting/refeeding cycles drove hematopoietic stem cell self-renewal and immune reconstitution in mice. That is regeneration triggered by the *transition*, which is precisely the mechanism your hypothesis proposes.

**If the transition is the active ingredient, the structure has two clocks rather than one, and they do different jobs.** The macro cycle is about accretion: its length is set by how fast tissue accumulates, which runs in weeks to months, and six weeks is a hypertrophy accumulation block. The micro cycle is the 5-day FMD and its refeed, and its length is set by autophagic flux and stem-cell kinetics, which run in days. Those are not one intervention at two sizes. A fasting cycle is not anti-growth *content* poured into the block to make it sufficiently restrictive — it is a complete prune-and-regrow in miniature, and neither half works without the other. Cheng's mechanism is that fasting itself lowers IGF-1 and PKA signalling, and that is what drives stem-cell self-renewal; the reconstitution then happens on refeeding. The fast supplies the signal, the refeed supplies the rebuild, and it is the cycle rather than either state that is the unit of the intervention. Two things downstream follow from reading it that way: where the cycles belong in the calendar (§4.5), and what an SGLT2 inhibitor is actually displacing when it takes their place (Part 3).

Note what this means for your thymus goal specifically. **The regenerative endpoint you want from TRIIM-X has adjacent support from a protocol that is free, has human trial infrastructure, and does not require rhGH.** If you only take one thing from this section, take that one.

It is also the weakest node in the structure and worth saying so plainly: the regenerative data is Cheng's mice, and the only human protocol with thymic imaging attached is the rhGH one §4.4 declines. The cycling frame has its best support on muscle and metabolic endpoints and its thinnest exactly where you most want it. That argues for placing the fasting cycles where their refeed is fully exploited, not for treating them as one interchangeable lever among several.

**Exercise periodization is the same idea in a field where it is uncontroversial.** Nobody trains at maximum volume continuously; accumulation and deload blocks alternate because the adaptation happens in the trough. Applying that logic to metabolic signalling is an analogy, not evidence — but it is a reasonable analogy, and the burden of proof that continuous is better has never been discharged either.

**The duty-cycle argument is arithmetically correct.** Two six-week pro-growth blocks a year is a ~23% duty cycle. If the risk of elevated IGF-1 is a function of cumulative exposure — which is the standard framing, and the same framing this document uses in your favour for ApoB — then the lifetime IGF-1 integral under cycling is roughly a quarter of continuous administration, while the anabolic stimulus during the block is undiminished. That materially blunts the IGF-1 exposure objection, and it is your strongest argument. It rests on linearity, though, and that should be conceded rather than assumed: an integral is the right model where risk accumulates with exposure — IGF-1 and cancer initiation, and the same model this document uses in your favour for ApoB — and the wrong one for anything governed by a threshold or a peak. Nothing in the somatotropic literature settles which shape applies, so the argument is strong rather than airtight.

**It solves your own scheduling problem.** The single sharpest criticism of your original methionine plan was that 5-on/2-off put restriction directly on top of the 48–72 h remodelling window after weekend training — stimulus delivered, then substrate withdrawn. Block cycling fixes that completely: weeks of restriction, then weeks of building, with no interleaving. Whatever else is true, the block version is a strictly better design than the weekly version.

### 4.2 What is not established

**No human trial has tested block alternation against either arm run continuously.** Everything above is mechanism plus adjacent results. Evidence tier 2. That is why the row scores 6 and not 15.

**The optimal block length is guesswork.** Six weeks is a reasonable guess for a hypertrophy accumulation block, which is probably where the number came from, and it is defensible for that reason. But the timescales that matter for the anti-growth arm are different and mostly unmeasured in humans — autophagic flux, senescent-cell clearance, FGF21 kinetics. Nobody knows whether six weeks off rapamycin loses the benefit or preserves it.

**Washout is a real constraint on the transitions, and it is asymmetric.** Rapamycin needs ~2 weeks to clear five half-lives; a pro-growth block that starts 3 days after the last dose is not a clean pro-growth block. Metformin clears in a day. IGF-1 takes 1–2 weeks to normalize after rhGH withdrawal, so the anti-growth block does not truly begin the day the injections stop. Budget roughly two weeks of transition at each boundary, which means a 6-week pro-growth block occupies about 8 weeks of calendar.

**There is a plausible failure mode where you get the costs of both arms and the benefits of neither** — never sustaining training volume long enough to accumulate tissue, while the anti-growth arm delivers only what its weakest lever can. The restriction side of that worry is the smaller half: dietary restriction phenotypes establish within days, not weeks, and reverse just as fast, so a block is more than long enough. Tissue accretion is the slow variable, which is what argues for 6–12 week blocks rather than 2–3.

**Cancer risk is the asymmetry that does not average out.** The pruning logic — clear damaged cells during restriction, then rebuild — assumes the clearing happens first and completely. If a pro-growth block instead supplies substrate and signalling to a lesion that the anti-growth block did not clear, the two phases are not symmetric in their consequences. This is speculative in both directions and there is no data to resolve it, but it is the reason to keep the pro-growth blocks anabolic rather than pharmacologically supraphysiologic, and the reason to keep cancer screening (which scores 20) on schedule regardless.

### 4.3 The pro-growth phase content

Here is the part where the analysis is unambiguous.

**Resistance training scores 15. Protein scores 12. Creatine scores 9. rhGH scores 2.** The pro-growth block that carries almost all of the available benefit is *training plus protein plus creatine plus sleep*, and it is free. Adding rhGH to that adds a poorly evidenced drug on top of a well-evidenced foundation, and the marginal contribution is unmeasured.

Two practical findings support running it hard:

**Maintenance is much cheaper than accumulation.** Trained individuals hold strength and lean mass on roughly one-third of accumulation volume for months (Bickel 2011 and the broader minimal-dose literature). Your instinct that weekend-only lifting during the anti-growth phase is sufficient to *hold* what you built is physiologically sound — that is maintenance volume, not detraining. What it will not do is build, which is the point of the structure.

**The cell-level explanation for that finding does not hold in humans, and the structure does not need it.** The attractive version is myonuclear permanence — nuclei added during a hypertrophy block retained through the reduced-volume period, making re-expression cheap rather than a rebuild. It is true in rodents and it does not replicate in people: a systematic review and meta-analysis of human and animal studies found exercise-induced myonuclei were *not* retained across human detraining periods of 12 to 48 weeks, while remaining elevated in rodents, and concluded that epigenetic mechanisms are the more likely basis for muscle memory. Individual human trials since have found retention in type II fibres, so the question is live rather than settled, but the meta-analysis is the higher tier of evidence and it points the other way — and the detraining durations it covers include the length of an anti-growth block, so there is no version of this that survives on timescale.

What survives is the functional finding itself, which never depended on the mechanism: maintenance volume holds strength and lean mass for months whether or not the nuclei stay. Treating Bickel as the load-bearing evidence and the myonuclear story as an appealing explanation that failed its own replication test is the same discipline this document applies to astaxanthin and to MK-7.

**Protein cannot be banked, but it can be phased.** Muscle protein synthesis has a per-meal ceiling and a refractory period, which is why compressing a week's intake into a weekend fails. Compressing a *year's* anabolic emphasis into two six-week blocks does not have that problem, because you are not trying to make one meal do a week's work — you are running weeks of adequate intake back to back. The per-meal ceiling argument kills the weekend plan and does not touch the block plan.

**One constraint that does not relax:** you are on tirzepatide, and protein at 1.2–1.6 g/kg/day plus resistance training is the mitigation for drug-induced lean-mass loss. That mitigation holds in both phases. The anti-growth block is "reduced volume and reduced anabolic emphasis," not "restriction plus detraining," and a block built on sustained protein restriction while the drug is running has the lean-mass arithmetic going the wrong way regardless of how good the cycling structure is.

**The floor is an average across the window lean mass integrates over, not a daily minimum** — and that distinction is what lets the fasting cycles sit inside it rather than in violation of it. Lean mass is an accretion variable that moves over weeks; five FMD days are 6% of a 12-week block. This is the same argument the paragraph above already makes in the other direction: the per-meal ceiling governs distribution within a day at a given intake, and says nothing about amortising five days across eighty-four. So the floor is a trailing-window average with the FMD days named inside it, and the apparent conflict between the protein rule and the fasting cycles closes as arithmetic.

**What does not close is the refeed, and that is the real constraint.** The rebuilding half of a fasting cycle is the refeeding, and you are on a drug whose mechanism is making refeeding hard — appetite suppression meeting a vegan protein-density problem that the [protein row](therapeutics-by-mechanism.md#protein-1216-gkgday-distributed) already calls the most likely point of failure in the whole regimen. Run the fast and miss the refeed and you have executed the catabolic half of the cycle twice a year and none of the anabolic half, which is strictly worse than not fasting. The gardening structure can prune a plant that cannot grow back. So the gate belongs on the refeed rather than on the fast: **protein back to 1.6 g/kg/day within 48 hours of ending an FMD, tracked, or the next cycle does not run.** That is a hold rule in the same shape as the ones in Part 3, and it is the one this structure most needs.

### 4.4 The rhGH question

Scored separately at **1 × 2 = 2, MONITOR, high effort**.

**Why MONITOR rather than AVOID.** The strongest case for an AVOID would be "raises IGF-1, directly opposes rapamycin, methionine restriction and every CR mimetic on this list." That is a simultaneity argument, and a cycling structure answers it. Setting it aside leaves two objections, both real and both MONITOR-grade rather than AVOID-grade.

**What those two are, honestly.** First, the evidence base: TRIIM was n=9, single-arm, uncontrolled, with ~2.5 years of epigenetic age reversal measured by clocks that are not validated mortality surrogates, and seven years on there are no peer-reviewed TRIIM-X results — only a preliminary presentation at a Foresight talk in May 2026. The trial is participant-funded and sponsor-analyzed, which is a structurally weak evidence generator regardless of the underlying biology. Second, exogenous rhGH raises IGF-1 into a range that training and protein do not; elevated IGF-1 associates with increased prostate, colorectal and breast cancer risk, and reduced IGF-1/insulin signalling is the most conserved life-extension pathway across model organisms. The duty-cycle argument reduces that exposure substantially; it does not eliminate it, and it does not supply the missing efficacy data.

Third, a smaller point that the protocol makes about itself: metformin is in the cocktail specifically to offset GH-induced insulin resistance that the protocol creates. When a therapy needs a second drug to counteract its own primary side effect, that is information about the risk-benefit ratio.

**Eligibility.** NCT04375657 is ages 40–80. You are 38, so it is two years out of reach. If you want it, the honest reason to enroll at 40 is contributing data to a study that badly needs participants — not receiving a treatment whose effect size is unknown.

**The recommendation that follows.** Run the cycling structure. Build the pro-growth blocks out of training, protein, creatine and sleep, which is where the evidence is. Leave rhGH out of the first several cycles, because adding an unevidenced drug to an unevidenced schedule makes the result uninterpretable — if something improves, you will not know which change did it. If you still want the rhGH arm after two or three clean cycles, you will at least have a personal baseline to compare against, which is more than TRIIM-X itself has.

### 4.5 A concrete calendar, if you run it

Offered as a starting structure, not a protocol — nobody has tested this, and the parameters below are reasoned guesses.

| Weeks | Phase | Training | Diet | Pharmacology |
|---|---|---|---|---|
| 1–6 | **Pro-growth** | Resistance 3–4×/wk, progressive; cardio maintained at 2×/wk | Protein 1.6 g/kg/day distributed; adequate methionine; energy at or slightly above maintenance | Creatine 5 g/day. Nothing anti-growth. No antioxidant supplements near training, and no cold immersion after lifting — both suppress the signal the block exists to generate. |
| 7–8 | Transition down | Taper resistance volume to maintenance | Protein holds at 1.2–1.6 | IGF-1 normalizing; nothing new started |
| 9–20 | **Anti-growth** | Resistance 1–2×/wk at maintenance volume, **keeping the loaded and impact work rather than only the machines** — bone is the tissue this block is most likely to give away; cardio 3×/wk | Protein averages ≥1.2 g/kg across the block while on tirzepatide; **the load-bearing FMD cycle runs at weeks 19–20**, with an optional earlier one mid-block and each cycle conditional on the last refeed having been hit; methionine *sources* shifted at the margin (pulses and legumes over seitan, oats, nuts and seeds) with methionine kept sufficient, never by cutting protein | **An SGLT2 inhibitor displaces the FMD cycles rather than substituting for them** — taking it runs the block with no transition in it. Hold any ARB through the FMD days. Cold plunging, if it happens at all, happens here. |
| 21–22 | Transition up | Volume ramps | Protein to 1.6; the FMD refeed lands here | Nothing anti-growth still on board; anything with a washout cleared before resistance volume rises |
| 23–28 | **Pro-growth** | repeat | repeat | repeat |

That is roughly two pro-growth blocks per year at a ~23% duty cycle, with 12 weeks of anti-growth emphasis between them and clean two-week transitions at every boundary.

**Why the fasting cycle sits at the end of the block rather than in the middle of it.** Clear, then rebuild — the same sequence that puts senolytics at the end of an anti-growth block in §2.6 rather than scattered through it. At weeks 19–20 the refeed and the volume ramp of the transition-up become one event, so the rebuilding half of the cycle arrives on rising anabolic demand instead of landing into ten more weeks of maintenance volume. It also takes the protein trough out of the middle of the maintenance-lifting stretch, and it puts the ARB hold and the low-intake window on a boundary that is already a transition.

**And why an SGLT2 inhibitor is not a swap for it.** The ketoacidosis conflict makes the two an either/or, which is correct as a safety statement and misleading as a design one. An SGLT2 inhibitor is a *state* intervention — a continuous caloric-restriction mimetic that holds the anti-growth setting down for as long as it is taken. An FMD cycle is a *transition*. Choosing the drug does not exchange one anti-growth lever for another; it removes every transition from the year and leaves a block that is anti-growth continuously, which is the configuration this structure exists to avoid. Rapamycin has the same shape and carries the same trade: it deepens the state without adding a transition. That is a reason to leave it out of the block that stands alongside its score of 6 rather than depending on it.

### 4.6 How you would know if it's working

This is the part that separates a hypothesis from a belief, and it is worth more than the protocol design.

**Pre-specify these before starting:**

- **DEXA at every phase boundary** — not the Withings BIA, which will not resolve the 1–2 kg changes at stake. The pro-growth block should show lean mass up; the anti-growth block should show it flat, not falling. Lean mass falling during anti-growth blocks means the structure is failing at its main job.
- **Bone density from the same scan, annually.** Muscle is the tissue this structure is designed to protect and bone is the tissue most likely to be given away without anyone noticing, because it has no symptom and no weekly proxy — grip catches a muscle problem months before DEXA does, and nothing catches a bone problem early at all. An anti-growth block withdraws mechanical loading and anabolic signalling from a skeleton already carrying a vegan diet and a GLP-1, which is three withdrawals converging on one tissue. Z-score above −1.0 and stable across a cycle is the pass condition; a fall is a reason to keep impact and axial loading in the anti-growth block rather than letting it go with the hypertrophy volume. Bone is also the tissue the alternation reaches least, and the timescales are why: a remodeling unit runs roughly 120–200 days start to finish, with resorption taking about two weeks against about thirteen for formation, so the cycle outlasts a 12-week block and bone integrates the year rather than swinging with it. Muscle can be pruned and regrown on a 22-week schedule and bone cannot, which makes keeping the loading in both blocks a structural requirement rather than a hedge.
- **Grip strength weekly** — cheapest early warning, and it moves before DEXA does.
- **IGF-1 and fasting insulin at each phase midpoint** — this is the readout that tells you the phases are actually different. If IGF-1 doesn't separate between blocks, you are not running two phases, you are running one phase with a varying training schedule.
- **ApoB every 8 weeks through the first cycle** — rapamycin raises lipids and a pro-growth block changes intake; the item scoring 25 should not drift while you experiment with items scoring 6.
- **A stopping rule.** If lean mass falls >1 kg across a full anti-growth block despite maintained protein and maintenance-volume training, the anti-growth phase is too aggressive. Shorten it or lighten it.

**And the honest caveat about clocks:** if you evaluate this with an epigenetic age test, you will get a number, and it will not mean what you want it to mean. The clocks are not validated mortality surrogates, they drift with assay batch and cell composition, and the effect sizes you are looking for are inside their noise. The organ-specific proteomic clocks are the interesting successor — plasma proteomics resolving a brain age, a heart age and a kidney age separately, with organ-specific deviation predicting organ-specific disease better than a single composite does — and they inherit the same problem for this purpose. They are trained to predict, not validated to respond, so nobody has shown that an intervention moving one of them moves the outcome it predicts, and the within-person test-retest variability against a 22-week block is unestablished. Watch the field; do not buy the test to grade this experiment. DEXA, grip, IGF-1 and ApoB are boring and they will actually tell you something.

**Score for the structure: evidence 2 × benefit 3 = 6, safety OK, effort moderate.** B3 is covering two different things and they should not be collapsed into one another. The smaller is avoided cost: the structure recovers muscle, bone and repair capacity that a continuously anti-growth protocol gives away, and converts three phase conflicts from exclusions into calendar entries. The larger, if the transition thesis in §4.1 holds, is not reducible to the rows being scheduled at all — a transition is a state that neither arm produces while it is running, and the regenerative results motivating the whole idea are triggered by the change rather than by either setting.

E2 is what holds the product down, and it holds down the second claim specifically: that one is mechanism plus adjacent animal results, and no human trial has tested it. The distinction matters for what would move the row. Better evidence that alternation beats either arm continuously raises E and the score follows. Evidence that the benefit is only the avoided cost leaves the number where it is and makes it genuinely a scheduling structure — which is the version of this row that would be fully counted in the items it schedules.

---

## Part 5 — The methionine restriction plan

You proposed: **<1 g methionine/day, five days a week, plus methioninase, with high protein and intense strength training on weekends.**

The underlying instinct is right. The implementation is likely to cost you muscle without delivering the mechanism. Eight problems, roughly in order of severity — and note that **the scheduling half of problem 3, and problems 4 and 5 entire, are the ones your block-cycling hypothesis solves.** Those are real points in its favour, and the evidence backs them.

### 1. The newest data says to keep methionine adequate, not cut it

Fanti, Longo et al., *Cell Metabolism*, June 2026 — the most directly relevant result published on this question. In aged mice, a low-protein "longevity diet" modeling traditional Mediterranean and Okinawan patterns **but supplemented with methionine (LDMM)** reduced fat mass and frailty, improved cardiometabolic markers, raised GH, GLP-1 and FGF21, and lowered IGF-1 — **without lean mass loss and without calorie restriction.** FGF21 was mechanistically required for the fat loss and insulin sensitivity.

Longo's own summary of the dose-response: **too little methionine caused frailty; too much abolished the benefits.** Their conclusion was that overall protein intake may matter less than specific amino acid composition, with a small but *sufficient* methionine intake.

So the lever is **total amino acids down, methionine kept adequate.** Your protocol does close to the inverse: methionine specifically down, total protein potentially high. You'd be aiming at the frailty arm of their dose-response curve.

### 2. The cost lands on whole-body lean mass, not on your response to training

Methionine is the initiator amino acid — translation begins with Met-tRNAi at every start codon — which is the usual reason for expecting restriction to blunt the anabolic response to lifting. It does not appear to. Eight weeks of an 80% methionine cut in rats left resistance-exercise mTORC1 signalling fully intact, with muscle protein synthesis *higher* under restriction than in controls and catabolic markers lower; methionine restriction combined with mechanical overload improved muscle and metabolic outcomes in old mice on a high-fat diet. At the signalling level, restriction and training are not antagonists.

The debit shows up one level up, in body composition, which is where you are actually measuring. Intermittently restricted mice sat 11–22% below controls on lean body mass (Plummer, *Aging Cell*, 2022), and in the 8-week human trial the restricted arm lost 0.69 kg more fat-free mass than controls (p=0.013) — a difference that attenuated once total weight loss was accounted for, but pointed the wrong way throughout. The mechanism by which restriction costs muscle is not a blocked training response. It is a whole-body substrate deficit that lifting does not offset.

### 3. The cut you can reach is not the cut that does the work

Rodent MR runs 0.12–0.17% methionine against 0.86% controls — an 80%+ cut, and in the best-performing intermittent arm, methionine-free days. That is frank deficiency, and the phenotype is steeply dose-dependent on it. At an intake that respects the sulfur amino acid requirement, the human result is flat: 8 weeks, 59 adults, ~2 g/day sulfur amino acids against ~5.6, and IGF-1 rose in both arms with no separation, FGF-21 did not move, and fat mass did not differ.

**The schedule is not the problem, and this is where your instinct was right.** Four days replete against three days restricted cut IGF-1 40–56% and raised FGF21 42–87 fold during the restricted periods — indistinguishable from continuous restriction, and with more lean mass and more bone retained than the continuous arm. Intermittent restriction establishes the phenotype perfectly well. What it does not do is install a state: IGF-1 returned to control levels within four days of repletion. The benefit exists only while restricted, which makes this an exposure-duration effect and a legitimate argument for cycling rather than against it.

So the objection is depth and dietary context, not cycle length. You are already at the shallow end of the dose-response and cannot go deeper without aiming at problem 1.

### 4. You can't bank a week's anabolism into a weekend

Muscle protein synthesis has a per-meal ceiling and a refractory period. The distribution literature consistently shows even protein spread across the day beats bolus loading for net synthesis. Compressing five days of missed intake into two doesn't recover it.

Note that this objection is specific to the weekend design and does not transfer to block cycling, where you are running weeks of adequate intake consecutively rather than asking two days to do a week's work.

### 5. Your training and your restriction are scheduled out of phase — and block cycling fixes this

Hard weekend lifting is fine while methionine-replete. But adaptation, remodeling and repair continue for 48–72 hours afterward — which lands on Monday and Tuesday, your restricted days. You'd deliver the stimulus and then withdraw the substrate precisely during the window when it's being used.

The narrow version of this — that restriction blocks the acute anabolic response — is not supported, and problem 2 concedes it. What the rat work establishes is that mTORC1 signalling and muscle protein synthesis survive an 80% cut; the authors did not follow the animals long enough to measure hypertrophy, and said so. Accretion over weeks is a different question from signalling over hours, and it is the one a 5-on/2-off schedule puts at risk.

**This is still the objection your hypothesis answers most directly.** Multi-week blocks never interleave stimulus with withdrawal, so the question does not arise. If you are going to combine training with restriction at all, the block structure is the correct way to do it, and the weekly structure is not. Credit where it's due.

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

1. **Hold total protein at 1.2–1.6 g/kg/day, distributed across meals, in both phases** — as an average across the block, with the FMD days counted inside it rather than exempted from it. Non-negotiable while on tirzepatide.
2. **Shift protein *sources*, don't cut protein *amount* — and expect almost nothing from it.** Legumes, soy and dairy carry substantially less methionine per gram of protein than beef, eggs, poultry and especially fish, and the 25–40% drop that defines the LDMM pattern comes from moving in that direction while total protein stays flat. **A vegan diet has already banked that entire drop** — 0.88 g/day methionine against 1.67 for meat-eaters, and 2.3 g/day total sulfur amino acids against 6.8 on a high-protein Western pattern. The restricted arm of the one adequately powered human trial *was* a whole-food plant-based diet, and it moved neither IGF-1 nor FGF-21 over 8 weeks. What remains for you is the spread within plant proteins — pulses and legumes at the low end, seitan, oats, nuts and seeds at the high end — which is too small to carry a block. The weight of the anti-growth phase sits on item 3, and there is no version of this where it doesn't. It also inverts the direction of risk: with methionine, cysteine and taurine all low at baseline, the live failure mode is inadequacy rather than excess, so treat the ~15 mg/kg/day requirement in the section above as a floor never to go under rather than a number to aim at, and do not chase further restriction. Hitting the protein floor puts you close to twice that intake by arithmetic — EPIC-Oxford's vegan figure of 2.3 g/day sits about 1.8× the requirement for an 85 kg man — which is where you should be.
3. **Get the FGF21 signal from time-restricted feeding or periodic fasting-mimicking cycles** — a few 5-day cycles a year — which have human trial data behind them rather than a chronic deficiency state. These sit at the *end* of the anti-growth blocks in Part 4, where the refeed runs straight into the volume ramp, and they are gated on the refeed rather than on the fast: protein back to 1.6 g/kg within 48 hours, or the next cycle does not run.
4. **Drop methioninase.**
5. **Drop NAC/GlyNAC if you're pursuing methionine work at all** — pick one.
6. **Use block cycling rather than weekly cycling.** Resistance training 3×/week during pro-growth blocks, 1–2×/week at maintenance volume during anti-growth blocks. This is the change that resolves the phase problem, and it is your idea rather than mine.
7. **Measure properly.** DEXA at baseline and at every phase boundary — not the Withings BIA, which will not resolve the changes at stake. Grip strength weekly. IGF-1 is the readout that tells you whether the block did anything. **Not plasma methionine** — it is buffered too tightly to report dietary change: intake differences across diet groups of 50% show up as −13% to +16% in plasma, and eight weeks of an 80% dietary cut in rats produced no plasma difference at all. Homocysteine if you want the one-carbon readout.
8. **Pre-specify a stopping rule.** If DEXA shows >1 kg lean mass loss across a full anti-growth block, the block is too aggressive.

### The thing you're actually reaching for

Halofuginone — a prolyl-tRNA synthetase inhibitor that triggers the amino acid response pathway pharmacologically, mimicking amino acid restriction without the nutritional deficit — extended median lifespan **+9% in male mice** in the 2025 ITP report. That is the concept you're after: the signal without the substrate loss. It's not available or advisable now, but it's the right thing to watch, and it's a better bet than a bacterial enzyme sold as a supplement.

---

## Caveats

Rapamycin, statins, ezetimibe, PCSK9 inhibitors, SGLT2 inhibitors, metformin, rhGH, and GLP-1 agonists are all prescription drugs requiring a physician. The interaction analysis above is a prompt for that conversation, not a substitute for it — bring the specific items (especially the SGLT2i ketoacidosis hold rules, and any growth-cycling plan involving rhGH) to whoever manages your tirzepatide.

I'm not a physician and this isn't medical advice. The scoring model is a sorting heuristic, not a measurement — the numbers are there to make the ranking's assumptions legible and arguable, not to imply precision.

Part 4 in particular describes a structure that **no human trial has tested**. It is scored at evidence tier 2 for that reason, and it is written as a hypothesis with a measurement plan attached rather than as a recommendation. The measurement plan is the part worth keeping if you discard everything else.
