# Chemical Synthesizer Operations
### ARGUS Station Documentation — Pharmacopoeia & Reagent Catalogue

This document covers every compound achievable using the Chemical Synthesizer's built-in cartridge supply. Entries include clinical field notes, known effects, species considerations, and ready-to-paste import strings for standard production runs.

Import strings are formatted for **Production Mode**: enter the recipe name, then paste the string when prompted.

---

## Base Cartridge Supply (24 reagents)

The synthesizer ships stocked with the following:

| | | | |
|---|---|---|---|
| Hydrogen | Carbon | Nitrogen | Oxygen |
| Fluorine | Chlorine | Sodium | Potassium |
| Lithium | Aluminium | Silicon | Phosphorus |
| Sulfur | Iron | Copper | Mercury |
| Tungsten | Calcium | Radium | Water |
| Ethanol | Sugar | Sulfuric Acid | — |

Cartridges recharge automatically at 5u per cycle. High-volume queues may outpace recharge on heavily demanded reagents (Oxygen, Carbon, Sugar, Hydrogen). Plan accordingly.

---

## How to Read This Document

**Import string format:** `Chem1,vol1,Chem2,vol2,...`
Chemical names are case-sensitive and must match cartridge labels exactly.

**Batch math notation:** Each reaction entry includes a scaling ratio. For example, `1:1:1 → 3u` means one unit of each ingredient yields three units of product. Scale linearly.

**OD** = Overdose threshold. Standard threshold is 30u for most personnel. Species variation applies.

---

---

# SECTION I — DIRECT SYNTHESIS (Single Recipe, No Intermediates)

---

## INAPROVALINE
**Classification:** Synaptic Stimulant / Cardiostimulant
**Reaction:** `Oxygen,1 + Carbon,1 + Sugar,1 → 3u` · Scale 1:1:1
**Inhibitor:** Water — do not mix; reaction fails silently. Use a dry vessel.
**OD threshold:** 60u (unusually high — very safe margin)
**Dermal absorption:** Partial

### Field Notes
Inaprovaline is a front-line stabilization agent. Its primary function is to slow the physiological deterioration of critically injured patients — essentially buying time for proper treatment. It also suppresses pain signaling and clears the biochemical cascade triggered by allergic reactions. A patient on Inaprovaline will not die *faster*, even if untreated.

Diona patients do not respond. All other species process it normally.

Inaprovaline does not heal damage. It only holds the line.

### Import Strings

| Output | Steps | String |
|--------|-------|--------|
| 6u | 3 | `Oxygen,2,Carbon,2,Sugar,2` |
| 15u | 3 | `Oxygen,5,Carbon,5,Sugar,5` |
| 30u | 3 | `Oxygen,10,Carbon,10,Sugar,10` |
| 60u | 3 | `Oxygen,20,Carbon,20,Sugar,20` |
| 120u | 3 | `Oxygen,40,Carbon,40,Sugar,40` |

> Minimum clean batch: 3u (1+1+1). 5u requires fractional volumes — use 6u instead.

---

## ANTITOXIN (Dylovene)
**Classification:** Broad-Spectrum Antitoxin
**Reaction:** `Silicon,1 + Potassium,1 + Nitrogen,1 → 3u` · Scale 1:1:1
**OD threshold:** 30u
**Dermal absorption:** Partial

### Field Notes
Dylovene is the station's primary counter to Toxic damage. It clears accumulated toxins from the bloodstream, reduces drowsiness and hallucination effects caused by poisoning, and has a small chance per dose of fully purging an active poison modifier. Effective against most environmental and biological toxins.

Diona patients do not respond.

Promethean patients at doses above 15u will experience mild disorientation — dose carefully in conscious subjects.

### Import Strings

| Output | Steps | String |
|--------|-------|--------|
| 6u | 3 | `Silicon,2,Potassium,2,Nitrogen,2` |
| 15u | 3 | `Silicon,5,Potassium,5,Nitrogen,5` |
| 30u | 3 | `Silicon,10,Potassium,10,Nitrogen,10` |
| 60u | 3 | `Silicon,20,Potassium,20,Nitrogen,20` |
| 120u | 3 | `Silicon,40,Potassium,40,Nitrogen,40` |

---

## KELOTANE
**Classification:** Burn Damage Treatment
**Reaction:** `Silicon,1 + Carbon,1 → 2u` · Scale 1:1
**Inhibitor:** Water — fails silently. Dry vessel mandatory.
**OD threshold:** 30u
**Dermal absorption:** Partial

### Field Notes
Kelotane is the standard treatment for Burn damage. It accelerates tissue repair at a rate of 4u Burn healed per unit metabolised, scaled to species healing capacity.

**Promethean (Slime) warning:** Kelotane repairs burn tissue in Prometheans but damages their silicate skeletal structure at the same time, causing 2u Brute per metabolisation cycle. For Promethean burn patients, consult alternative burn treatments or monitor closely for compounding injury.

Diona patients do not respond.

### Import Strings

| Output | Steps | String |
|--------|-------|--------|
| 5u | 2 | `Silicon,2.5,Carbon,2.5` |
| 15u | 2 | `Silicon,7.5,Carbon,7.5` |
| 30u | 2 | `Silicon,15,Carbon,15` |
| 60u | 2 | `Silicon,30,Carbon,30` |
| 120u | 2 | `Silicon,60,Carbon,60` |

> Decimal volumes are valid in production mode. Minimum clean integer batch: 2u (1+1).

---

## SYNAPTIZINE
**Classification:** Neurostimulant / Anti-Stun Agent
**Reaction:** `Sugar,1 + Lithium,1 + Water,1 → 3u` · Scale 1:1:1
**OD threshold:** 30u
**Dermal absorption:** Partial
**Metabolism rate:** Very slow — single dose remains active for an extended period

### Field Notes
Synaptizine is used to treat neurological suppression. It clears drowsiness, counters paralysis, stun, and weakness effects, and actively purges Mindbreaker (hallucinogen) from the bloodstream with each metabolisation cycle. Its slow processing rate means a single dose provides extended coverage.

Promethean patients at dose ≥5u gain Brute and Burn healing from Synaptizine at the cost of accelerated nutrition consumption.

Diona patients do not respond.

**Note:** Water is a required ingredient here — this is not an inhibitor conflict. Ensure no excess Water is already present from prior reactions in the vessel; it will not block Synaptizine synthesis but will interfere with any co-queued Inaprovaline or Kelotane.

### Import Strings

| Output | Steps | String |
|--------|-------|--------|
| 6u | 3 | `Sugar,2,Lithium,2,Water,2` |
| 15u | 3 | `Sugar,5,Lithium,5,Water,5` |
| 30u | 3 | `Sugar,10,Lithium,10,Water,10` |
| 60u | 3 | `Sugar,20,Lithium,20,Water,20` |
| 120u | 3 | `Sugar,40,Lithium,40,Water,40` |

---

## HYPERZINE
**Classification:** Muscle Stimulant / Movement Enhancer
**Reaction:** `Sugar,1 + Phosphorus,1 + Sulfur,1 → 3u` · Scale 1:1:1
**OD threshold:** 15u — **overdoses at half the standard threshold. Handle carefully.**
**Dermal absorption:** Partial

### Field Notes
Hyperzine is a powerful long-acting muscle stimulant that increases movement speed significantly. Standard emergency-response issue for personnel who need rapid cross-station transit.

**Overdose hazard:** Threshold is half normal (≈15u in standard humans). Overdose causes intermittent cardiac stress — a small but non-zero chance of direct heart organ damage per metabolisation cycle. Do not administer casually.

Tajara metabolise Hyperzine at 1.25× potency — reduce dosing accordingly for Tajara patients.

Promethean patients experience skeletal instability rather than clean speed enhancement. At dose ≥5u, nutrition is burned at an accelerated rate.

Diona patients do not respond.

### Import Strings

| Output | Steps | String |
|--------|-------|--------|
| 6u | 3 | `Sugar,2,Phosphorus,2,Sulfur,2` |
| 15u | 3 | `Sugar,5,Phosphorus,5,Sulfur,5` |
| 30u | 3 | `Sugar,10,Phosphorus,10,Sulfur,10` |
| 60u | 3 | `Sugar,20,Phosphorus,20,Sulfur,20` |
| 120u | 3 | `Sugar,40,Phosphorus,40,Sulfur,40` |

> **Dispense in small batches for personal use.** A 30u bottle is more than enough for most standard deployments.

---

## IMPEDREZENE
**Classification:** Neurological Depressant / Incapacitant
**Reaction:** `Mercury,1 + Oxygen,1 + Sugar,1 → 2u` · Scale 1:1:1 at 66% yield
**OD threshold:** 30u
**Filtered by:** Spleen organ

### Field Notes
Impedrezene slows higher cognitive function, impairs coordination, and induces progressive drowsiness and Brain damage with sustained exposure. It is classified internally as a weapons-grade compound.

Practical medical use is limited. It sees occasional application in sedation protocols where Chloral Hydrate is unavailable, though with a significant side effect profile.

At low concentrations: reduces motor jitter, causes mild drowsiness, slowly accumulates Brain damage.
At prolonged exposure: drooling, incoherence, compounding Brain damage.

Diona patients do not respond.

**Yield note:** 3u of reagents yields only 2u of product. Scale accordingly.

### Import Strings

| Output | Steps | String |
|--------|-------|--------|
| 5u | 3 | `Mercury,2.5,Oxygen,2.5,Sugar,2.5` |
| 15u | 3 | `Mercury,7.5,Oxygen,7.5,Sugar,7.5` |
| 30u | 3 | `Mercury,15,Oxygen,15,Sugar,15` |
| 60u | 3 | `Mercury,30,Oxygen,30,Sugar,30` |
| 120u | 3 | `Mercury,60,Oxygen,60,Sugar,60` |

---

## MUTAGEN
**Classification:** Genetic Mutagen
**Reaction:** `Radium,1 + Phosphorus,1 + Chlorine,1 → 3u` · Scale 1:1:1

### Field Notes
Mutagen induces random genetic mutations in organic subjects. Effect delivery varies by administration route: blood injection is most reliable, ingestion has a 67% trigger chance, and topical application only 33%.

Synthetic units are immune. Dionaea are unaffected.

Mutation outcomes are entirely unpredictable and range from cosmetic to debilitating. This compound should not be administered therapeutically. Its primary function is as a precursor reagent in the synthesis of Left4Zed (see Section II).

### Import Strings

| Output | Steps | String |
|--------|-------|--------|
| 6u | 3 | `Radium,2,Phosphorus,2,Chlorine,2` |
| 15u | 3 | `Radium,5,Phosphorus,5,Chlorine,5` |
| 30u | 3 | `Radium,10,Phosphorus,10,Chlorine,10` |
| 60u | 3 | `Radium,20,Phosphorus,20,Chlorine,20` |
| 120u | 3 | `Radium,40,Phosphorus,40,Chlorine,40` |

---

## CLARIDYL
**Classification:** Analgesic / Stabilizer (Advanced)
**Reaction:** `Lithium,1 + Radium,1 + Sugar,1 → 1u` · Scale 1:1:1 at 33% yield
**OD threshold:** Effectively non-toxic at any practical dose
**Metabolism rate:** Slow — extended active duration
**Dermal absorption:** Full

### Field Notes
Claridyl is a high-potency analgesic and patient stabilizer. It provides the strongest stabilization and pain suppression available from this machine — roughly double Inaprovaline's stabilization strength and quadruple its analgesic effect. Extremely effective at keeping critical patients functional and alive under sustained injury.

At therapeutic doses it very slowly repairs minor Brute damage — however, each unit repaired costs proportional Hallucination damage. Not a clean healer; it trades one problem for another.

**Critical note for Tesshari (Tesh) personnel:** An extremely rare adverse reaction exists in which a single dose causes 50u of Toxic damage instantly. Document and flag any Tesh patients who have reported adverse reactions to Claridyl.

Minor behavioral side effects (irritability, cognitive lapses, dry mouth, mild dizziness) occur at low probability per cycle — patients may report feeling "off."

**Yield note:** This is an inefficient reaction. 3u of reagents produces only 1u of product. A 60u bottle consumes 180u of feedstock.

### Import Strings

| Output | Steps | String |
|--------|-------|--------|
| 5u | 3 | `Lithium,5,Radium,5,Sugar,5` |
| 15u | 3 | `Lithium,15,Radium,15,Sugar,15` |
| 30u | 3 | `Lithium,30,Radium,30,Sugar,30` |
| 60u | 3 | `Lithium,60,Radium,60,Sugar,60` |
| 120u | 3 | `Lithium,120,Radium,120,Sugar,120` |

> 120u batch consumes 360u total feedstock — within the machine's vessel limit, but allow time for Lithium, Radium, and Sugar cartridge recharge.

---

## BLISS
**Classification:** Psychoactive / Controlled Substance
**Reaction:** `Mercury,1 + Sugar,1 + Lithium,1 → 3u` · Scale 1:1:1
**OD threshold:** 30u

### Field Notes
Bliss is a psychoactive compound producing a pronounced euphoric high, disorientation, and periodic involuntary movement and emotional expression. Subjects experience elevated mood, perceptual distortion, and reduced inhibition.

**Overdose:** Causes hallucinations and accumulates Brain damage and Toxic damage per cycle. Extended overdose is harmful and potentially fatal.

Prometheans experience significantly reduced effect due to biochemical resistance to toxin-class compounds.

Diona patients do not respond.

No therapeutic application. Synthesis documented for completeness.

### Import Strings

| Output | Steps | String |
|--------|-------|--------|
| 6u | 3 | `Mercury,2,Sugar,2,Lithium,2` |
| 15u | 3 | `Mercury,5,Sugar,5,Lithium,5` |
| 30u | 3 | `Mercury,10,Sugar,10,Lithium,10` |
| 60u | 3 | `Mercury,20,Sugar,20,Lithium,20` |
| 120u | 3 | `Mercury,40,Sugar,40,Lithium,40` |

---

## APHRODISIAC
**Classification:** Pheromone Agent
**Reaction:** `Carbon,2 + Hydrogen,2 + Oxygen,2 + Water,1 → 6u` · Scale 2:2:2:1 at 86% yield

### Field Notes
Aphrodisiac produces mild behavioral and pheromone effects in subjects. Physical response is subtle — occasional involuntary expression. No therapeutic or emergency medical value. No damage profile. Synthesis documented for completeness.

**Yield note:** 7u of feedstock yields 6u of product.

### Import Strings

| Output | Steps | String |
|--------|-------|--------|
| 6u | 4 | `Carbon,2,Hydrogen,2,Oxygen,2,Water,1` |
| ~18u | 4 | `Carbon,6,Hydrogen,6,Oxygen,6,Water,3` |
| 30u | 4 | `Carbon,10,Hydrogen,10,Oxygen,10,Water,5` |
| 60u | 4 | `Carbon,20,Hydrogen,20,Oxygen,20,Water,10` |
| 120u | 4 | `Carbon,40,Hydrogen,40,Oxygen,40,Water,20` |

> 15u is not achievable in clean integers. Nearest batches: 12u (`Carbon,4,Hydrogen,4,Oxygen,4,Water,2`) or 18u (`Carbon,6,Hydrogen,6,Oxygen,6,Water,3`).

---

## CRYPTOBIOLIN
**Classification:** Vestibular Disruptor / Incapacitant
**Reaction:** `Potassium,1 + Oxygen,1 + Sugar,1 → 3u` · Scale 1:1:1
**OD threshold:** 30u
**Metabolism rate:** Fast — effects are short-lived

### Field Notes
Cryptobiolin is a vestibular disruption agent. It induces dizziness and cognitive confusion in affected subjects, with effect strength scaling to species toxin sensitivity.

Prometheans experience significantly reduced effect.
Diona patients do not respond.

No medical use. Its fast processing rate means effects are relatively brief compared to slow-metabolising sedatives.

### Import Strings

| Output | Steps | String |
|--------|-------|--------|
| 6u | 3 | `Potassium,2,Oxygen,2,Sugar,2` |
| 15u | 3 | `Potassium,5,Oxygen,5,Sugar,5` |
| 30u | 3 | `Potassium,10,Oxygen,10,Sugar,10` |
| 60u | 3 | `Potassium,20,Oxygen,20,Sugar,20` |
| 120u | 3 | `Potassium,40,Oxygen,40,Sugar,40` |

---

---

# SECTION II — CHAINED SYNTHESIS (Multi-Step, Single Recipe)

The reactions below require intermediates that can be generated *within the same recipe* by supplying all feedstock at once. The synthesizer vessel allows reactions to chain automatically. Do not attempt to manually separate steps — add all ingredients in a single recipe run.

> **Inhibitor reminder:** Ammonia synthesis is blocked by Phoron. If the catalyst slot contains Phoron, disable catalyst use before running these recipes.

---

## AMMONIA (Intermediate)
**Classification:** Industrial Precursor / Fertilizer Base
**Reaction:** `Hydrogen,3 + Nitrogen,1 → 3u` · Scale 3:1

Not directly useful for most personnel. Produced as an intermediate in Space Cleaner and Diethylamine synthesis. If needed standalone:

| Output | Steps | String |
|--------|-------|--------|
| 15u | 2 | `Hydrogen,15,Nitrogen,5` |
| 30u | 2 | `Hydrogen,30,Nitrogen,10` |
| 60u | 2 | `Hydrogen,60,Nitrogen,20` |

---

## SPACE CLEANER
**Classification:** Industrial Cleaning Agent
**Chain:** `3H + 1N → 3u Ammonia` → `Ammonia + Water → 2u Space Cleaner`
**Net ratio:** H×1 + N×(1/3) + Water×1 per unit of output

Space Cleaner decontaminates surfaces, objects, and personnel of most biological and chemical residue. It will extinguish lit smoking articles on contact with subjects. Effective against Macrophage viral entities (20 Toxic on contact).

**Single-recipe chaining works:** Add Hydrogen, Nitrogen, and Water together. Hydrogen and Nitrogen react first to form Ammonia, which immediately reacts with Water to form Space Cleaner.

| Output | Steps | String |
|--------|-------|--------|
| ~15u | 3 | `Hydrogen,7.5,Nitrogen,2.5,Water,7.5` |
| 30u | 3 | `Hydrogen,15,Nitrogen,5,Water,15` |
| 60u | 3 | `Hydrogen,30,Nitrogen,10,Water,30` |
| 120u | 3 | `Hydrogen,60,Nitrogen,20,Water,60` |

---

## DIETHYLAMINE
**Classification:** Chemistry Precursor
**Chain:** `3H + 1N → 3u Ammonia` → `Ammonia + Ethanol → 2u Diethylamine`
**Net ratio:** H×1 + N×(1/3) + Ethanol×1 per unit of output

Diethylamine is a secondary amine with mild corrosive properties and no direct therapeutic use. It is the primary intermediary required for Left4Zed synthesis and several advanced compounds not producible on this machine.

| Output | Steps | String |
|--------|-------|--------|
| ~15u | 3 | `Hydrogen,7.5,Nitrogen,2.5,Ethanol,7.5` |
| 30u | 3 | `Hydrogen,15,Nitrogen,5,Ethanol,15` |
| 60u | 3 | `Hydrogen,30,Nitrogen,10,Ethanol,30` |
| 120u | 3 | `Hydrogen,60,Nitrogen,20,Ethanol,60` |

---

## LEFT4ZED
**Classification:** Hydroponics Fertilizer
**Chain:** `3H + 1N → Ammonia` → `Ammonia + Ethanol → Diethylamine` → `2 Diethylamine + Mutagen → 3u Left4Zed`
**Parallel chain:** `Radium + Phosphorus + Chlorine → Mutagen` (runs simultaneously)
**Net ratio (per 9u output):** H×3, N×1, Ethanol×3, Radium×1, Phosphorus×1, Chlorine×1

Left4Zed is a hydroponics plant fertilizer. In the bloodstream it acts as a mild toxin. Personnel should not consume it intentionally. Its primary station use is accelerating plant growth cycles in the hydroponics bay.

**Batch sizing note:** Clean integer batches occur only at multiples of 9u due to the 3:1 Hydrogen:Nitrogen ratio and 2:1 Diethylamine:Mutagen ratio.

| Output | Steps | String |
|--------|-------|--------|
| 9u | 6 | `Hydrogen,3,Nitrogen,1,Ethanol,3,Radium,1,Phosphorus,1,Chlorine,1` |
| ~27u | 6 | `Hydrogen,9,Nitrogen,3,Ethanol,9,Radium,3,Phosphorus,3,Chlorine,3` |
| ~63u | 6 | `Hydrogen,21,Nitrogen,7,Ethanol,21,Radium,7,Phosphorus,7,Chlorine,7` |
| ~126u | 6 | `Hydrogen,42,Nitrogen,14,Ethanol,42,Radium,14,Phosphorus,14,Chlorine,14` |

> Nearest to 30u is 27u. Nearest to 60u is 63u. Nearest to 120u is 126u.

---

---

# SECTION III — ENGINEERING / INDUSTRIAL

---

## SILICATE
**Classification:** Glass Reinforcement Agent
**Reaction:** `Aluminium,1 + Silicon,1 + Oxygen,1 → 3u` · Scale 1:1:1

Silicate is applied topically to window structures to reinforce them against impact and damage. It has no effect when administered to personnel.

| Output | Steps | String |
|--------|-------|--------|
| 15u | 3 | `Aluminium,5,Silicon,5,Oxygen,5` |
| 30u | 3 | `Aluminium,10,Silicon,10,Oxygen,10` |
| 60u | 3 | `Aluminium,20,Silicon,20,Oxygen,20` |
| 120u | 3 | `Aluminium,40,Silicon,40,Oxygen,40` |

---

---

# SECTION IV — NOT ACHIEVABLE ON THIS MACHINE

| Compound | Reason |
|----------|--------|
| Leporazine | Requires Phoron as catalyst — not in base supply |
| Mead | Requires Enzyme catalyst — not in base supply |
| Hooch | Requires Fuel — not in base supply |
| Manlydorf | Requires Beer and Ale — not producible |
| Matcha Latte | Requires Matcha Powder and Milk — not producible |
| RobustHarvest | Requires Neurotoxic Protein — not producible |
| Most advanced compounds | Require Phoron catalyst, Plasticide, or brewed alcohol |

---

# APPENDIX A — Inhibitor Reference

Reactions that silently fail if these chemicals are present in the vessel. A failed reaction leaves all reagents unreacted — no output, no indication of failure. Rinse between batches if reusing the vessel.

| Compound | Blocked By |
|----------|------------|
| Inaprovaline | Water (any amount) |
| Kelotane | Water (any amount) |
| Ammonia | Phoron (any amount) |
| Lye | Carbon (any amount) |
| Water synthesis | Sodium or Carbon |
| Sodium Chloride | Copper |
| Chloral Hydrate | Fluorine (trace amounts) |
| Fringeweaver | Fuel |

---

# APPENDIX B — Catalyst Reference

Catalysts are loaded into the catalyst slot and returned to it after each recipe completes. They are not consumed in synthesis.

| Reaction | Catalyst | Available from base supply? |
|----------|----------|-----------------------------|
| Fire Foam | 10u Fluorine | Yes |
| Leporazine | Phoron | No |
| Mead | Enzyme | No |

> To run Fire Foam production: load 10u Fluorine into the catalyst bottle, seat it in the machine, enable catalyst use, then queue recipes using only Water as the synthesis ingredient. Fluorine is extracted and re-seated between each run automatically.

---

*All entries compiled from direct station system analysis. ARGUS.*
