# Genetic Pathways

**Target:** healthy male, age 39, US, vegan, currently on tirzepatide
**9 August 2026**
**Companion to** [anti-aging-inventory.md](anti-aging-inventory.md) (framework, grouped inventory, interactions, protocols) and [therapeutics-by-mechanism.md](therapeutics-by-mechanism.md) (row-level reasoning for the drugs)

This file holds the human-genetics layer: the loss-of-function and gain-of-function variants that sit behind the drug targets in the other two documents, and the somatic editing programs that would install them directly.

**How this document is arranged**

1. **Each pathway is doing two jobs at once, and they are graded separately.** A human knockout is both *evidence* for a drug target and a *proposal* for an edit. Those have completely different strengths, and conflating them is the characteristic error in this field. Part 1 separates them.
2. **The scale is the one used everywhere else** — `E × B = score`, safety as a veto flag, effort as a tag outside the score. What is scored here is **the edit**: installing the variant somatically, in you, now. The drug that already exploits the same pathway is named in each row and carries its own score in the inventory.
3. **Grouping follows the inventory's mechanism families**, so a row here sits opposite its drug row there.
4. **Most of these rows score low, and the reasons repeat.** Rather than restate them twenty times, the three recurring discounts — exposure time, delivery, and loss of control — are argued once in Part 1 and referenced afterward.

---

## Part 1 — The framework

### The two jobs, and why they get different grades

Take PCSK9. The nonsense carriers in Cohen's 2006 cohort run 28% lower LDL-C lifelong and have 88% less coronary heart disease. That single fact does two different things:

- **As evidence,** it is close to decisive. It is a randomized-at-conception, lifelong-exposure natural experiment with a hard clinical endpoint, and it is a large part of why the inventory grades PCSK9-mediated LDL lowering as a *causally validated surrogate* rather than an ordinary one — the reason enlicitide sits at E4 on lipid data alone instead of E3.
- **As a therapeutic proposal,** it is nearly worthless on its own. It says nothing about whether editing *PCSK9* in a 39-year-old's hepatocytes is safe, how much of the 88% survives the timing change, or what the edit does over forty years that a stopped drug would not.

Every row below carries both. **The genetics column is frequently the strongest evidence in this entire repository. The edit column is almost uniformly the weakest.** That is not a contradiction; they are answers to different questions.

The practical consequence is that this document's main output is *not* a list of things to do. It is the reason the ApoB family in [§2 of the detail file](therapeutics-by-mechanism.md#2-apob-and-the-lipoprotein-pathway) is graded the way it is, and a filter that stops the same genetic evidence being spent twice — once to justify a drug, and again to justify an edit that has not earned it.

### The attenuation ladder — what a germline effect size is worth at 39

A Mendelian randomization estimate describes a variant that has been running since conception in every cell. Five discounts separate that number from what a somatic edit buys a 39-year-old, and they compound.

**1. Exposure time.** This is the largest, and the repo already has the arithmetic. Ference puts 40 years of 1 mmol/L lower LDL-C at 54.5% lower CHD risk, against roughly 24% for a statin started mid-life and run five years. Same molecule, same target, ~3× the effect from starting earlier. **You cannot buy back the first 39 years with an edit.** What an edit at 39 delivers is the *start-now* number — which is the same number a $5 statin started now delivers. The exposure-time leverage that makes the genetics so persuasive is the one component that is not for sale.

**2. Development.** Part of a lifelong variant's effect is structural and laid down before adulthood — vascular architecture, bone geometry, brain organization, muscle fiber number. Myostatin nulls are muscular *at birth*. Klotho and IGF-1 signalling shape the skeleton during growth. An edit installed after skeletal maturity cannot access any of it.

**3. Coverage.** A germline variant is present in 100% of cells at a known allele dose. Somatic editing is partial and mosaic — the best in-vivo liver programs reach roughly 60–70% of hepatocytes in primates at high dose. For a secreted protein whose effect scales with circulating concentration, partial is proportional and fine. For a tumor suppressor, partial is worthless, because the uncorrected cells are the ones that matter. Part 1's third subsection makes this the organizing distinction.

**4. Compensation.** A lifelong variant is buffered — the organism develops around it, which can shrink the phenotype relative to an acute change, or hide harms that only appear when the change is made abruptly. MR estimates the effect of *the variant*, not of *the intervention*. The gap between the two is the standing reason drug-target MR is treated here as strong support rather than proof.

**5. Direction is not symmetric.** That losing a gene is harmful does not establish that having more of it helps. *TREM2* is the clean case: biallelic loss causes Nasu-Hakola disease and R47H roughly doubles-to-quadruples Alzheimer's odds, which is solid evidence that TREM2 is load-bearing — and the first real test of TREM2 *agonism* in humans failed. The same asymmetry applies to klotho and to follistatin, where the entire case runs on deficiency phenotypes and mouse overexpression.

### Delivery decides this list, not biology

The split between what is in the clinic and what is not tracks almost perfectly with a single fact: **lipid nanoparticles go to hepatocytes by default**, taken up through the LDL receptor after ApoE adsorbs to them. Everything that is editable in humans today is a liver-expressed, secreted-protein pathway.

| Editable now, in trials | Not, and not soon |
|---|---|
| *PCSK9*, *ANGPTL3*, *TTR*, *APOC3*, *LPA*, *ASGR1*, *INHBE*, *HSD17B13* | *KLOTHO*, *TREM2*, *APOE*, *FOXO3*, *PTEN*, *BRCA1/2*, *SLC5A2*, *GLP1R*, *GIPR* |
| hepatocyte-expressed, secreted, dose-responsive | brain, kidney, microglia, muscle, or every cell in the body |

The second constraint is **what kind of edit**. Three tiers, in descending order of feasibility:

- **Knockout** — break a gene. A nuclease cut or a base edit that installs a stop codon or wrecks a splice site. This is the easy one, and it is what every clinical program on the list above is doing. Eight of the user-named pathways are knockouts, which is why eight of them have real programs behind them.
- **Overexpression** — add a gene. AAV delivery, episomal, so it dilutes in dividing tissue; capped at ~4.7 kb; blocked in people with pre-existing neutralizing antibodies to the capsid; and carrying a live safety record — high-dose systemic AAV has produced fatal acute liver failure, including two deaths in Duchenne patients in 2025. This is the tier *FST* and *KLOTHO* sit in.
- **Precise correction** — change one base to another without breaking the gene. Requires prime editing or base editing with a favorable target sequence, and it is barely feasible: the landmark is a single bespoke n-of-1 base-editing treatment for CPS1 deficiency in an infant in 2025, built for one patient over six months. *BRCA1*, *BRCA2*, *PTEN* and APOE conversion are all in this tier.

**The user's list is therefore three lists.** Knockouts of secreted liver proteins are a live clinical field. Overexpression in muscle and brain is early and has killed people. Correcting a germline point mutation in every cell of an adult is not a thing that exists.

### The control problem — an edit deletes the levers this regimen runs on

This is the argument that ends most rows below, and it comes straight out of [Part 4 of the inventory](anti-aging-inventory.md#part-4--growth-cycling).

The whole regimen is built on the premise that **duty cycle is a lever**: six-week blocks rather than continuous administration, washouts budgeted at every boundary, a rapamycin dose timed to clear before training volume returns. Its safety management is likewise built on three controls — **dose titration** (tirzepatide against the fuel floor and ALMI), **hold rules** (SGLT2 inhibitor for any illness with poor intake, GLP-1 before anesthesia), and **washout** (rapamycin ≥2 weeks before a pro-growth block).

An edit is the maximum-duty-cycle intervention. It has no dose, no hold, and no washout. That is precisely what you want for ApoB, where the direction of benefit is monotone, certain, and wanted forever — and it is precisely wrong for everything else on the list.

Two rows make the point concretely rather than abstractly. An edited *SLC5A2* is a permanent SGLT2 inhibitor, and the entire management of euglycemic ketoacidosis in this regimen is *stop the drug* — an edit deletes the only mitigation there is. An enhanced GLP1R has no dose to cut when total testosterone drops below 500 ng/dL or ALMI falls. Both are hard conflicts in the [Part 3 sense](anti-aging-inventory.md#part-3--interactions): the usual remedy is scheduling, and scheduling is the thing being removed.

---

## Part 2 — The pathways, grouped by mechanism

`E` = evidence (1–5) for **the edit, in you, now** · `B` = benefit at 39 · safety is a veto flag · effort sits outside the score.
Each row also states **the natural experiment** (what the human variant establishes, and how strongly) and **the drug** that already reaches the same target.

### 2.1 Lipoprotein — where the genetics carry real weight

This is the family where human genetics is not a supporting argument but the load-bearing one. It is also the family where every pathway already has a drug, which is what makes the edits redundant rather than exciting.

#### PCSK9 knockout
**2 × 4 = 8** · MONITOR · high · phase 1b · **WATCH**
**The natural experiment — very strong.** *PCSK9* nonsense variants (Y142X, C679X) at ~2.6% frequency in African-Americans give 28% lower LDL-C and 88% less coronary heart disease; R46L in European-ancestry cohorts gives ~15% lower LDL-C and ~47% less CHD (Cohen, NEJM 2006). A compound heterozygote with essentially no circulating PCSK9 was healthy, fertile and cognitively normal at an LDL-C of 14 mg/dL. Target-by-target MR against parental lifespan puts *PCSK9* lipid-lowering alleles on the longer-lived side.
**The drug:** [rosuvastatin + ezetimibe](therapeutics-by-mechanism.md#2b-hmg-coa-reductase) (25 and 16) reach most of this for under $25/month; [evolocumab](therapeutics-by-mechanism.md#evolocumab--alirocumab) (25), [inclisiran](therapeutics-by-mechanism.md#inclisiran) (20) and [enlicitide](therapeutics-by-mechanism.md#enlicitide-decanoate-lipfendra-oral) (20) hit PCSK9 itself.
**The edit:** VERVE-102, an adenine base editor delivered in a GalNAc-targeted LNP that disrupts *PCSK9* in hepatocytes. Phase 1b has reported dose-dependent LDL-C reductions reaching roughly 50%+ at the top doses in a few dozen participants, durable across the follow-up so far.
**Why:** E2 — real human data, but a surrogate endpoint in a phase 1b of a few dozen people, with no long-horizon safety and no way to reverse the change if one appears. B4 — the *increment* over generics, not the whole ApoB effect, which is the same reasoning that puts [ApoB to <30](therapeutics-by-mechanism.md#apob-to-30-mgdl-the-increment-beyond-60) at B4 rather than B5. **The honest case against it at 39 is not safety, it is arithmetic:** the edit's selling point over inclisiran is adherence across decades, and it is buying that with irreversibility in the one person on this list whose adherence problem is hypothetical. If any edit on this page ever becomes reasonable for you, it is this one — after outcomes data, not before.

#### ANGPTL3 knockout
**1 × 3 = 3** · MONITOR · high · phase 1 (HoFH) · **WATCH**
**The natural experiment — strong.** Familial combined hypolipidemia: over 200 heterozygous and ~20 homozygous loss-of-function carriers are described, with ~40% lower ASCVD odds and no adverse cardiometabolic phenotype. Homozygous humans with no functional ANGPTL3 walking around healthy is the strongest safety datum available for any target in this document.
**The drug:** evinacumab (approved for HoFH), plus siRNA agents in development. No inventory row — the indication is homozygous FH, not primary prevention.
**The edit:** VERVE-201, base editing *ANGPTL3*, in early trials for HoFH and refractory hypercholesterolemia.
**Why:** E1 for you — the human data is in a genetic disease you do not have. B3 — ANGPTL3 loss lowers LDL, triglycerides *and* HDL, and on a vegan diet with a statin your triglycerides are the part of that package least in need of help. You would be buying a broad lipid effect to capture a narrow LDL increment that the [PCSK9 ladder](therapeutics-by-mechanism.md#2e-pcsk9--four-modalities-one-target) reaches more directly.

#### LPA knockout
**1 × 4 = 4** · OK · high · no clinical editing program · **WATCH**
**The natural experiment — strong, and it sets the dose.** Lp(a) is ~90% determined by *LPA*, and humans with essentially undetectable Lp(a) are common and unremarkable — the protein is dispensable, which is unusual and is the main safety argument for knocking it out. MR also tells you *how much* lowering is required: roughly 100 mg/dL of Lp(a) reduction to match the CHD benefit of 1 mmol/L of LDL-C, which is why modest reductions are not worth chasing. One discordant signal, replicated: genetically very low Lp(a) associates with slightly *higher* type 2 diabetes risk.
**The drug:** [pelacarsen, olpasiran, lepodisiran, muvalaplin](therapeutics-by-mechanism.md#2f-apoa--lpa) (8, WATCH). Lp(a)HORIZON is event-driven and past its guided mid-2026 window; OCEAN(a) targets December 2026.
**The edit:** none in humans. The *LPA* kringle IV repeat region is highly repetitive, which is a genuinely difficult editing substrate.
**Why:** E1 — no editing program exists. B4 — matches the inventory's Lp(a) row, and like it, is entirely conditional on your number. [Measure Lp(a) once](therapeutics-by-mechanism.md#lpa-once-lifetime) (16): if it comes back low, this whole row is inert for you permanently, which is the highest-value thing genetics can tell you for $30.

#### CETP loss of function
**1 × 2 = 2** · MONITOR · high · no editing program · **WATCH the drug**
**The natural experiment — real but ambiguous, and instructive for that reason.** CETP deficiency is common in Japanese populations (D442G, intron 14 splice variants) and produces markedly high HDL-C. Whether those carriers have *less* coronary disease has been contested for thirty years, with the Omagari cohort pointing the wrong way. Drug-target MR is cleaner: lower CETP activity associates with lower apoB and lower coronary risk, and *CETP* variants are among the three lipid targets — with *HMGCR* and *NPC1L1* — associated with lower dementia risk in the ~1M-person analysis cited in [§2](therapeutics-by-mechanism.md#2-apob-and-the-lipoprotein-pathway).
**The drug:** four CETP inhibitors have failed for four different reasons — torcetrapib on off-target hypertension, dalcetrapib and evacetrapib on futility, anacetrapib on adipose accumulation despite a positive REVEAL. Obicetrapib is the fifth, with phase 3 lipid data showing substantial LDL-C lowering and, unusually, ~50%+ Lp(a) reduction. **PREVAIL is the outcomes readout and it is the only thing that matters here.** No inventory row until it lands.
**Why:** E1 — a class with a 4-for-4 failure record does not get graded on its genetics. B2 — on statin plus ezetimibe, the apoB increment is modest; the interesting part is the Lp(a) and dementia signal, and both are unproven. **This is the clearest case in the document of strong genetics failing to translate**, which is worth carrying as a standing caution against the rest of the page.

#### The rest of the lipid pathways, briefly
Four more carry good human genetics and change nothing for you, but they belong here because they show the family is not uniform.

- **APOB loss of function — the knockout you do not want.** Heterozygous familial hypobetalipoproteinemia gives ~50% lower LDL-C and low coronary disease, and it costs hepatic steatosis, because APOB is required to export VLDL from the liver. Same lipid direction as *PCSK9*, opposite safety profile — and the reason mipomersen was withdrawn. **1 × 1 = 1 · AVOID.** The lesson generalizes: "lowers LDL by knockout" is not one category.
- **ASGR1 loss of function — the one where the effect exceeds the lipids.** A 12-base deletion in Icelanders gives ~15 mg/dL lower non-HDL-C and ~34% lower coronary artery disease, a reduction larger than the lipid change predicts. Live target, no clinical program. **1 × 2 = 2 · WATCH.**
- **APOC3 loss of function.** ~40% lower CHD via triglyceride-rich lipoproteins; olezarsen is approved for familial chylomicronemia. **1 × 1 = 1** — your triglycerides on a vegan diet with an incretin are not the problem this solves.
- **NPC1L1 loss of function.** Naturally occurring inactivating variants give ~50% lower CHD odds — the genetic backing for [ezetimibe](therapeutics-by-mechanism.md#2c-npc1l1-cholesterol-absorption) (16), and worth noting because *NPC1L1* is the lipid target that does **not** reach significance in lifespan MR while looking protective in dementia MR. That inconsistency is an instrument-strength artifact rather than a biological finding, and it is the reason the inventory declines to claim a longevity effect for ezetimibe specifically while still recommending it.

### 2.2 Incretin, glucose and body weight

Every pathway here is already being addressed pharmacologically in your regimen, and every edit forfeits the dose control that regimen depends on.

#### GLP1R gain of function
**1 × 1 = 1** · MONITOR · high · no program
**The natural experiment — moderate.** *GLP1R* Ala316Thr (rs10305492) associates with lower fasting glucose and lower type 2 diabetes risk, with a concordant direction on coronary disease. It is a modest-effect common variant, not a knockout, and it establishes the direction rather than the magnitude.
**The drug:** [tirzepatide](therapeutics-by-mechanism.md#3a-incretin-receptor-agonism) (16), which you are on. SELECT established MACE and all-cause mortality benefit for the class in non-diabetic adults.
**Why:** E1 — no editing program, and none is plausible, since GLP1R is expressed across pancreas, gut, brain and vasculature with no delivery route that reaches the right subset. B1 — **a peptide agonist is strictly better than an edited receptor here**, because the regimen's entire safety architecture for this drug is dose titration: cut the dose when ALMI falls or the fuel floor trips. A constitutively enhanced receptor has no dose to cut.

#### GIPR loss of function
**1 × 1 = 1** · MONITOR · high · no program
**The natural experiment — strong, and it contradicts your drug.** *GIPR* E354Q and related reduced-function variants associate with lower BMI and lower fat mass, and MR supports GIP receptor *blockade* for obesity. You are taking a GIP receptor *agonist*. Both directions produce weight loss in humans: tirzepatide via agonism, and maridebart cafraglutide (a GIPR antagonist fused to a GLP-1 agonist) reaching roughly 20% weight loss in phase 2.
**The resolution, such as it is:** chronic GIPR agonism causes receptor desensitization and downregulation, so sustained agonism may be functionally closer to antagonism than the labels suggest. This is unresolved, it is one of the more interesting open questions in the field, and **nobody should be editing a receptor whose useful direction is actively disputed.**
**Why:** E1 — the direction of benefit is not settled. B1 — you already have the pharmacological version, and it is titratable. One caution worth carrying regardless of route: GIP is bone-anabolic, and reduced GIPR signalling has been linked to lower bone mineral density — relevant to a regimen that treats bone loading as a reason to lift.

#### SLC5A2 (SGLT2) loss of function
**1 × 2 = 2** · **AVOID** · high · no program
**The natural experiment — strong, and it is the best safety datum SGLT2 inhibition has.** Familial renal glucosuria is caused by biallelic *SLC5A2* loss of function. Homozygotes excrete large quantities of glucose daily, have normal renal function and normal lifespan, and the condition is regarded as benign — which is a far better answer to "what does a lifetime of SGLT2 blockade do to a kidney" than any trial can give. MR on *SLC5A2* variants points to lower HbA1c, lower diabetes risk and lower heart failure risk.
**The drug:** [empagliflozin / canagliflozin](therapeutics-by-mechanism.md#3b-sglt2-inhibition) (6, MONITOR, optional). Canagliflozin gave +14% median lifespan in male ITP mice, the largest male effect in ITP history.
**Why:** E1 for the edit. B2 matches the drug row — you have no heart failure, no CKD and no diabetes. **AVOID is about control, not about the target.** The inventory's management of euglycemic ketoacidosis is entirely a hold rule: stop the drug for any illness with poor oral intake, stop it 3 days before a procedure, and never run it alongside the FMD cycles. A permanent edit deletes every one of those, and converts a scheduled either/or into an unresolvable [hard conflict](anti-aging-inventory.md#hard-conflicts--these-do-not-resolve-with-scheduling). The genetics are excellent and they argue for taking the pill, not for making the change permanent.

#### The obesity and glycemia knockouts, briefly
- **SLC30A8 loss of function** — protein-truncating variants give ~65% lower type 2 diabetes risk, and the direction is *opposite* to the rodent knockout. The best single reminder on this page that mouse genetics can invert. **1 × 1 = 1** — no diabetes to prevent that tirzepatide is not already preventing.
- **GPR75 loss of function** — heterozygous carriers (~4 per 10,000) weigh ~1.8 kg less and have ~54% lower obesity odds. A live target with no clinical agent. **1 × 1 = 1.**
- **MC4R gain of function** — leanness-associated variants track lower BMI, lower diabetes and lower coronary risk; loss of function causes severe obesity and is the setmelanotide indication. **1 × 1 = 1.** All three are redundant against a drug already achieving 20%+ weight loss with hard-outcome data behind it.

### 2.3 Muscle and the ActRII axis — the family most likely to be mistaken for a fit

Follistatin, myostatin and activin E all converge on activin type II receptor signalling, which is the same axis as the [myostatin/activin blockade row](therapeutics-by-mechanism.md#myostatin--activin-blockade-bimagrumab-apitegromab) (4, WATCH). Everything the inventory says against the *antibody* applies with more force to a *gene therapy*, because the antibody at least stops eventually.

#### FST (follistatin) gain of function
**1 × 1 = 1** · **AVOID** · high · unregulated clinics · **matches the [§17 row](therapeutics-by-mechanism.md#17-no-credible-mechanism-or-unregulated-administration)**
**The natural experiment — absent.** There is no human follistatin gain-of-function cohort. The case is mouse overexpression producing large muscle gains, plus small AAV-follistatin trials in Becker muscular dystrophy and inclusion body myositis with mixed results in single-digit patient numbers.
**The problem is specificity.** Follistatin does not bind myostatin alone — it binds activin A, GDF11 and several BMPs. Systemic overexpression is therefore a broad, permanent perturbation of the activin/inhibin axis, which is also the axis regulating FSH and reproductive function. "More muscle" is one of the things it does, not the thing it does.
**Why:** E1 — no human evidence at all for the intervention as sold. B1 — the axis is already covered for free by [resistance training, protein and creatine](therapeutics-by-mechanism.md#6-gh--igf-1-and-anabolism--the-pro-growth-arm) at 15, 12 and 9. **AVOID is over-determined:** it is sold through medical-tourism clinics outside any regulatory review, and it fails the inventory's two structural objections to ActRII blockade at full strength — mass is not function, and it cannot be phased out of an anti-growth block, so it takes the DEXA series, which is the only instrument the cycle has, and makes it permanently unreadable.

#### MSTN (myostatin) knockout
**1 × 1 = 1** · **AVOID** · high · no human program
**The natural experiment — real but n≈1.** A child with a homozygous *MSTN* splice mutation was described in 2004 with visible muscularity at birth and strength above age norms; the animal versions are Belgian Blue cattle, Piedmontese cattle and bully whippets.
**Why it does not transfer:** the phenotype is largely **hyperplastic and developmental** — more fibers, laid down before birth — which is exactly the [developmental discount](#the-attenuation-ladder--what-a-germline-effect-size-is-worth-at-39) in Part 1. Myostatin-null muscle also shows reduced specific force per unit cross-section and altered tendon properties in animals. A permanent edit in an adult installs the part of the phenotype with the worst evidence and none of the part with the best.
**Why:** E1 · B1 · AVOID for the same reasons as follistatin.

#### INHBE (activin E) knockout
**1 × 2 = 2** · MONITOR · high · preclinical/early · **WATCH**
**The natural experiment — good, and pointed in a more useful direction than the other two.** *INHBE* protein-truncating variants associate with lower waist-to-hip ratio adjusted for BMI — that is, favorable *fat distribution* rather than added mass — along with a better metabolic profile and lower coronary risk. It is liver-expressed and secreted, which puts it in the editable column.
**Why:** E1 for the edit. B2 — visceral adiposity is a target this regimen already attacks hard, with [VAT <50 cm²](README.md) as an explicit DEXA endpoint under tirzepatide. **This is the one row in the family whose genetics favor it**, and it is the one with no product. Worth watching precisely because it is the opposite of follistatin: a real human signal, a plausible delivery route, and no clinic selling it.

### 2.4 Growth signalling and the longevity loci

This section is the genetic version of [Part 4](anti-aging-inventory.md#part-4--growth-cycling)'s central question, and it does not answer it cleanly in either direction.

#### FOXO3 gain of function
**1 × 1 = 1** · OK · high · no program
**The natural experiment — the second-best-replicated longevity locus in humans, and it does not do what the name implies.** *FOXO3* rs2802292 has been associated with exceptional longevity across Japanese-American, German, Italian, Chinese and Ashkenazi cohorts — with *APOE*, one of only two loci that replicate reliably for human lifespan. Homozygous carriers show meaningfully raised odds of reaching 95+.
**Why it is not editable, and why that barely matters:** the variant is intronic and acts on *FOXO3* expression under stress conditions, in every tissue. There is no construct to deliver and no target cell population to deliver it to. But the parenthetical in the request is the important part — **AMPK phosphorylates and activates FOXO3, and the inventory has already worked out what that implies.** [§2.3](anti-aging-inventory.md#23-ampk-and-energy-sensing) puts the best-evidenced AMPK activator on the list at 20, and it is [cardiorespiratory training](therapeutics-by-mechanism.md#4-ampk-and-energy-sensing), which is free. Metformin scores 4 and berberine is an AVOID.
**Why:** E1 · B1 — **the actionable form of "FOXO3 gain of function" is already in the regimen, and it is exercise.** That is not a consolation prize; it is the one intervention on this page with a score above 15.

#### GHR / IGF1R loss of function
**1 × 1 = 1** · **AVOID** · high · no program
**The natural experiment — strong, famous, and more equivocal than it is usually reported.** The Ecuadorian Laron cohort (growth hormone receptor deficiency) has near-total protection from diabetes and near-zero cancer incidence across decades of follow-up. Separately, heterozygous *IGF1R* loss-of-function variants are enriched among Ashkenazi centenarians. Reduced IGF-1/insulin signalling remains the most conserved life-extension pathway across model organisms.
**The part that gets left out:** the Laron cohort **did not live longer**. Protection from two major causes of death did not produce lifespan extension, in part because other causes filled the gap. And the phenotype is profound short stature established in childhood — the single purest illustration of the developmental discount.
**Why:** E1 · B1 · AVOID — you cannot install this at 39, and the cohort that has it lifelong shows what it buys and what it does not. **Its real use in this repo is as a check on Part 4:** it is the strongest human evidence that suppressing growth signalling protects against cancer and diabetes, and simultaneously the strongest human evidence that doing so does not straightforwardly extend life. Both halves belong in the ledger, and the second half is the one that keeps the [rhGH row](therapeutics-by-mechanism.md#rhgh-containing-pro-growth-block-triim--triim-x-style) at MONITOR rather than AVOID.

#### KLOTHO gain of function
**1 × 2 = 2** · MONITOR · high · preclinical / early AAV · **WATCH**
**The natural experiment — genuinely interesting, with a strange shape.** The *KL-VS* haplotype associates with longer life and better cognition **in heterozygotes**, while homozygotes do *worse* — a heterozygote advantage, which is unusual and means "more klotho" is not a straight line. Klotho-overexpressing mice live ~20–30% longer; klotho-deficient mice show a premature-aging syndrome; circulating klotho declines with age in humans. A single low-dose injection of soluble klotho improved cognitive performance in aged rhesus monkeys in 2023, which is the most striking primate result in the geroscience literature and remains a single study.
**The complication:** klotho is the obligate co-receptor for FGF23, so raising it systemically perturbs phosphate and vitamin D metabolism. Membrane klotho and soluble klotho are different molecules doing different jobs, and it is not settled which one the longevity association is about.
**Why:** E1 — mouse and one primate study. B2 — cognition and kidney aging are real targets, and the delivery problem is brain and kidney, which is the wrong column. AAV programs exist in early development. **Watch the soluble-protein route rather than the gene therapy route** — a dosable protein preserves every control an edit destroys, and the primate result was produced by an injection, not an edit.

### 2.5 Vascular and fibrinolytic

#### SERPINE1 (PAI-1) loss of function
**1 × 2 = 2** · MONITOR · high · drug in early trials · **WATCH**
**The natural experiment — one of the most striking human longevity findings there is, and it comes with its own dose-response warning.** An Old Order Amish kindred in Berne, Indiana carries a null *SERPINE1* allele. Heterozygous carriers have longer leukocyte telomeres, lower fasting insulin, better vascular compliance, and a median lifespan roughly a decade longer than non-carriers in the same community — an unusually clean comparison, since the kindred is genetically and environmentally homogeneous. **Homozygous null carriers have a bleeding disorder** with delayed bleeding after trauma and surgery.
**So the genetics specify a dose.** One allele is beneficial; two are a hemostatic defect. That is a partial-inhibition target, which is a drug's shape, not a knockout's.
**The drug:** TM5614, an oral PAI-1 inhibitor, has run in early Japanese trials across several indications. No inventory row — nothing near an outcomes trial.
**Why:** E1 for the edit. B2 — plausible vascular and metabolic benefit with no human interventional outcome data. Note the interaction the repo already tracks: added fibrinolytic activity stacks with the [aspirin + fish oil + nattokinase bleeding conflict](anti-aging-inventory.md#hard-conflicts--these-do-not-resolve-with-scheduling), and aspirin is already an AVOID at your age.

#### PDE5 loss of function
**1 × 1 = 1** · OK · high · no program; **the drug is generic and cheap**
**The natural experiment — weak, and the honest thing to say is that this pathway is not really a genetics story.** There is no protective human *PDE5A* knockout cohort. What exists is drug-target MR using *PDE5A* variants weighted to blood pressure, which associates PDE5 inhibition with lower coronary risk, plus a large and messy observational literature: lower mortality after myocardial infarction in registry data, and a much-publicized claims-based association with reduced Alzheimer's incidence that **did not survive better-controlled replication**.
**Why:** E1 for the edit and E2 at best for the pathway. B1 for the edit — **tadalafil is a generic pill costing a few dollars a month, and any test of this hypothesis runs through it.** The reason there is no inventory row is that the evidence sits at mechanism-plus-confounded-observational with no hard outcome, which would place it among the 2s and 4s rather than anywhere that changes a decision. One live interaction to carry regardless: berberine raises tadalafil exposure through CYP3A4 and P-gp, which is part of why berberine is an [AVOID](therapeutics-by-mechanism.md#4-ampk-and-energy-sensing).

### 2.6 Neurodegeneration

Both rows here are conditional on a genotype you would have to test for first — and [testing is the insurable event](therapeutics-by-mechanism.md#apoe-genotype--cad-polygenic-risk-score). **GINA covers health insurance but not life, disability or long-term-care insurance.** Secure term life and own-occupation disability coverage before ordering any of it.

#### APOE4 or APOE3 → APOE2
**1 × 2 = 2** · MONITOR · high · phase 1/2 in AD patients · **WATCH**
**The natural experiment — the strongest common-variant effect in late-onset Alzheimer's, and it is not a free lunch in either direction.** ε4 raises risk substantially and dose-dependently; ε2 lowers it relative to ε3. But ε2 carries liabilities of its own: ε2/ε2 homozygosity is the necessary background for type III hyperlipoproteinemia, which develops in a minority of homozygotes, and ε2 is associated with increased risk of cerebral amyloid angiopathy–related hemorrhage.
**What is actually being tried, and why it is not conversion:** LEXEO's LX1001 delivers an *APOE2* transgene intrathecally by AAV to APOE4 homozygotes with Alzheimer's disease, and phase 1/2 work has shown CSF APOE2 expression with biomarker movement. That is **additive APOE2 expression in a subset of CNS cells**, not conversion of an ε4 allele to ε2. True conversion would require precise correction in essentially every APOE-expressing cell in brain and liver — Part 1's third tier, and not a thing that exists.
**Why:** E1 — early-phase, in symptomatic patients, in the highest-risk genotype. B2 — dementia is a top-five cause of death and the effect would be meaningful *if* it worked, but the trial population is people who already have the disease, which is the opposite of your position. **The actionable version at 39 is the [genotype test](therapeutics-by-mechanism.md#apoe-genotype--cad-polygenic-risk-score) (6), insured first**, and the honest note attached to it: at 39 there is little you would do differently that is not already on the list.

#### TREM2 gain of function
**1 × 1 = 1** · MONITOR · high · agonist antibody failed
**The natural experiment — solid in the deleterious direction only.** R47H raises Alzheimer's odds roughly two- to four-fold and R62H less so; biallelic loss of *TREM2* or *TYROBP* causes Nasu-Hakola disease. That establishes TREM2 as load-bearing for microglial function. **It does not establish that more TREM2 signalling helps** — Part 1's fifth discount, in its cleanest form.
**And the direction has now been tested.** AL002, a TREM2 agonist antibody, failed its phase 2 in early Alzheimer's disease, with no clinical benefit and safety findings that argue against simply pushing harder.
**Why:** E1 — the first real human test of the intended direction was negative. B1 — no route to benefit at 39 from a pathway whose agonism has not been shown to do anything.

### 2.7 Amyloid — TTR knockout

#### TTR knockout
**3 × 1 = 3** · OK · high · **phase 3 · DEFER**
**The natural experiment plus the pharmacology — jointly the strongest evidence for any knockout on this page.** Transthyretin knockdown to ~80–90% below baseline has been sustained for years in humans with patisiran and vutrisiran without a deficiency syndrome, which is as close to a controlled human knockout experiment as this field gets. The variant most worth knowing about is **V122I (p.V142I), carried by roughly 3–4% of Black Americans**, which causes late-onset cardiac amyloidosis.
**The edit:** nexiguran ziclumeran (nex-z, formerly NTLA-2001) — in-vivo CRISPR knockout of *TTR* in hepatocytes via LNP, producing ~90% durable serum TTR reduction from a single dose, now in phase 3 for both ATTR cardiomyopathy and hereditary polyneuropathy. **This is the most advanced in-vivo gene editing program in medicine** and the reference point for what a real human knockout-on-demand looks like.
**Why it is nonetheless a 3:** E3 — the knockdown and its tolerability are well established, and the phase 3 outcome data is pending. B1 at your age, for the same reason [coronary artery calcium](therapeutics-by-mechanism.md#coronary-artery-calcium) is a 5 × 1 — the evidence is excellent and it is evidence about a condition you do not have and are unlikely to develop for four decades. Wild-type ATTR is a disease of the eighties, present in a substantial minority of aged hearts at autopsy and badly underdiagnosed.
**The practical position:** nothing to do at 39. If ancestry makes V122I plausible, that genotype is worth knowing eventually — after the insurance is in place — and the trigger is unexplained left ventricular hypertrophy, heart failure with preserved ejection fraction, bilateral carpal tunnel syndrome or lumbar spinal stenosis, not a birthday. **One durable caution for the whole class:** TTR carries thyroxine and retinol-binding protein, so knockdown requires vitamin A monitoring.

### 2.8 Cancer predisposition — a different kind of row entirely

*BRCA1*, *BRCA2* and *PTEN* are not "install a beneficial variant." They are "remove a deleterious one you may not have," and three things follow that do not apply anywhere else on this page.

**First, the row is conditional on carrier status, and most people have nothing to correct.** For a non-carrier the score is undefined rather than low — there is no edit, because there is no mutation.

**Second, tumor suppressors are the all-or-nothing case.** [Part 1's coverage discount](#the-attenuation-ladder--what-a-germline-effect-size-is-worth-at-39) is fatal here. Editing 60% of hepatocytes gives you 60% of a PCSK9 effect, because circulating protein is a dose. Correcting 60% of cells in a *BRCA1* carrier gives you approximately none of the benefit, because a tumor arises from **one** uncorrected cell that loses its remaining allele. The target is every cell in every at-risk tissue, and it is a *correction*, not a knockout — the hardest tier of the hardest problem.

**Third, the effective intervention already exists and is not genetic.** For a male *BRCA2* carrier the actionable consequences are earlier and more intensive prostate surveillance, awareness of male breast and pancreatic risk, PARP-inhibitor sensitivity if cancer ever arises, and — the part that usually matters most — implications for children and siblings. For *PTEN*, Cowden syndrome carries a distinctive phenotype (macrocephaly, mucocutaneous lesions, thyroid and renal findings) that is typically recognizable well before 39, and management is a surveillance schedule.

#### BRCA1 / BRCA2 correction
**1 × 1 = 1** · MONITOR · high · no program · **the row that matters is testing, then surveillance**
**Why:** E1 — germline correction in an adult is not an existing capability, and the closest human precedent is a single bespoke base-editing treatment built for one infant with a urea-cycle disorder over six months. B1 as an edit. **The conditional value of *knowing* is high** and it runs through [cancer screening on schedule](therapeutics-by-mechanism.md#16-early-detection) (20), which is already one of the top rows in the inventory. Insure before testing.

#### PTEN correction
**1 × 1 = 1** · MONITOR · high · no program
**Why:** E1 · B1, on the same reasoning. *PTEN* adds one wrinkle: it is haploinsufficient and dose-sensitive, so the therapeutic window for any future correction is narrower than for a straightforward knockout — too much PTEN activity is not obviously benign either.

### 2.9 Telomeres — the counterexample worth keeping

#### TERT / telomerase gain of function
**1 × 1 = 1** · **AVOID** · high · unregulated clinics · **matches the [§17 row](therapeutics-by-mechanism.md#17-no-credible-mechanism-or-unregulated-administration)**
**The natural experiment runs the wrong way.** Short-telomere syndromes cause bone marrow failure and pulmonary fibrosis, which is the fact these clinics cite. **Long-telomere syndromes** — *POT1* and *TERT* promoter variants — cause **increased cancer**: melanoma, chronic lymphocytic leukemia, glioma, and others. Human genetics has tested "longer telomeres are better" directly, and answered no.
**Why:** E1 · B1 · AVOID. It belongs on this page because it is the pathway where the intuition behind half of this list is most clearly wrong, and where the genetics were available to say so before anyone sold it.

### 2.10 Inflammation — IL6R loss of function

#### IL6R loss of function
**1 × 1 = 1** · MONITOR · high · no editing program · **WATCH the drug**
**The natural experiment — clean.** The *IL6R* Asp358Ala variant impairs IL-6 receptor signalling and associates with lower coronary heart disease risk per allele, alongside the expected CRP and fibrinogen shifts. It is the best genetic support for the residual-inflammatory-risk hypothesis, and it is why [hsCRP](therapeutics-by-mechanism.md#hscrp) (6) is on the diagnostics list at all: the test exists to gate this question.
**The drug:** ziltivekimab is the IL-6 ligand antibody being carried through cardiovascular outcomes trials in inflammatory high-risk populations. CANTOS validated the upstream IL-1β step and then failed on cost-effectiveness and infection risk rather than on efficacy.
**Why:** E1 for the edit; the pathway itself is on much firmer ground than the score suggests. B1 for you specifically — the trial populations are people with elevated CRP *and* established disease *and* usually chronic kidney disease. **The trigger that would make this live is a persistently elevated hsCRP after ApoB is at target**, which is the residual-risk branch the inventory's [inflammation section](anti-aging-inventory.md#26-everything-else-by-family) already describes, and where [low-dose colchicine](therapeutics-by-mechanism.md#11-inflammation) (2) failed at n=7,062.

---

## Part 3 — Flat ranked list

Score-ordered. Every row is the **edit**, not the drug; the drug's score lives in the inventory.

| Score | E×B | Pathway | Direction | Safety | Status |
|---:|:---:|---|---|:---:|---|
| **8** | 2×4 | *PCSK9* | knockout | monitor | phase 1b (VERVE-102) — WATCH |
| **4** | 1×4 | *LPA* | knockout | ok | no program — conditional on your Lp(a) |
| **3** | 1×3 | *ANGPTL3* | knockout | monitor | phase 1 in HoFH — WATCH |
| **3** | 3×1 | *TTR* | knockout | ok | phase 3 (nex-z) — **defer, evidence is excellent and the disease is 40 years away** |
| **2** | 1×2 | *INHBE* | knockout | monitor | preclinical — the one in its family the genetics favor |
| **2** | 1×2 | *KLOTHO* | gain of function | monitor | early AAV — watch the soluble protein instead |
| **2** | 1×2 | *SERPINE1* | loss of function | monitor | oral inhibitor in early trials; homozygous null bleeds |
| **2** | 1×2 | *APOE* ε4/ε3 → ε2 | isoform conversion | monitor | phase 1/2, additive expression in AD patients, not conversion |
| **2** | 1×2 | *CETP* | loss of function | monitor | four drug failures; obicetrapib's PREVAIL is the readout |
| **2** | 1×2 | *ASGR1* | loss of function | monitor | no program |
| **2** | 1×2 | *SLC5A2* | loss of function | **AVOID** | excellent genetics, and it deletes the ketoacidosis hold rule |
| **1** | 1×1 | *GLP1R* · *GIPR* · *SLC30A8* · *GPR75* · *MC4R* | mixed | monitor | drug exists and is titratable; direction disputed for *GIPR* |
| **1** | 1×1 | *FOXO3* | gain of function | ok | not deliverable; the actionable form is exercise (20) |
| **1** | 1×1 | *IL6R* | loss of function | monitor | trigger is hsCRP elevated after ApoB is at target |
| **1** | 1×1 | *PDE5* | loss of function | ok | the drug is generic; the AD signal did not replicate |
| **1** | 1×1 | *APOC3* · *NPC1L1* | loss of function | ok | covered by diet and by ezetimibe (16) |
| **1** | 1×1 | *BRCA1* · *BRCA2* · *PTEN* | correction | monitor | not an existing capability; test, insure first, then screen |
| **1** | 1×1 | *TREM2* | gain of function | monitor | agonist antibody failed phase 2 |
| **1** | 1×1 | *GHR* / *IGF1R* | loss of function | **AVOID** | developmental, and the Laron cohort did not live longer |
| **1** | 1×1 | *APOB* | knockout | **AVOID** | hepatic steatosis — the lipid knockout you do not want |
| **1** | 1×1 | *MSTN* | knockout | **AVOID** | hyperplastic and developmental; unphaseable |
| **1** | 1×1 | *FST* | gain of function | **AVOID** | unregulated clinics; breaks the DEXA instrument permanently |
| **1** | 1×1 | *TERT* | gain of function | **AVOID** | long-telomere syndromes cause cancer |

**Nothing on this page outscores rosuvastatin.** The highest row here is 8; [ApoB to <60](therapeutics-by-mechanism.md#apob-to-60-mgdl) is 25, and it is reached with two generics costing under $25 a month. That is the summary finding, and it is not an artifact of conservatism — it is the exposure-time discount doing its work. The genetics that make these pathways compelling are compelling *because* the variant ran for eighty years, and the only intervention on this list that captures anything like that is one you start now and keep taking.

---

## Part 4 — Triggers

Nothing here is actionable today. These are the specific events that would change an answer, and they are the reason to keep the page.

| Trigger | What changes |
|---|---|
| **Lp(a) comes back high** | The *LPA* row goes from conditional to live, and the [Lp(a)-lowering drugs](therapeutics-by-mechanism.md#2f-apoa--lpa) get there first. Lp(a)HORIZON and OCEAN(a) are the readouts. |
| **PREVAIL reports positively for obicetrapib** | CETP enters the [lipoprotein family](anti-aging-inventory.md#21-apob-and-the-lipoprotein-pathway) as a drug row, with the dementia MR as the interesting second endpoint. Four prior failures mean the outcome trial is the whole case. |
| **VERVE-102 reports cardiovascular outcomes** | The *PCSK9* edit becomes gradeable rather than speculative. Until then it competes with a $5 statin on adherence alone. |
| **hsCRP stays elevated with ApoB at target** | The *IL6R* row becomes the live branch of the residual-risk question, and ziltivekimab's outcomes data becomes the thing to read. |
| **ALMI falls below 8.5 kg/m² with protein and lifting documented** | The [antibody](therapeutics-by-mechanism.md#myostatin--activin-blockade-bimagrumab-apitegromab) becomes a question. The gene therapies do not — being unphaseable and irreversible is disqualifying in exactly the scenario where you most need to be able to stop. |
| **Family history or ancestry raises a specific carrier probability** | *BRCA1/2*, *PTEN*, *TTR* V122I. Test — **after** term life and own-occupation disability coverage are in force. The action that follows is surveillance, which is already a 20 in the inventory. |
| **A soluble klotho protein enters human trials** | Watch it. A dosable protein keeps every control an AAV construct destroys. |

---

## Caveats

Everything scored on this page is either unavailable, available only inside a trial for a disease you do not have, or sold by clinics operating outside regulatory review. Nothing here is a recommendation, and several rows exist specifically to explain why an attractive-sounding intervention is not one.

The genetics themselves are a different matter, and they are load-bearing elsewhere in this repo: Mendelian randomization and human knockout cohorts are a substantial part of why the [lipoprotein family](therapeutics-by-mechanism.md#2-apob-and-the-lipoprotein-pathway) is graded at E4–E5 on surrogate endpoints when nothing else is. That grading depends on MR being treated as strong support rather than proof — the [compensation discount](#the-attenuation-ladder--what-a-germline-effect-size-is-worth-at-39) is the reason for the gap, and it is why a positive outcomes trial still moves a score and a positive MR alone does not.

I'm not a physician and this isn't medical advice. Gene editing programs move quickly and the trial statuses above are a snapshot; the scores are a sorting heuristic, not a measurement.
