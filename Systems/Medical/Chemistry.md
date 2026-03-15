[ARGUS Station Database](../../README.md) > Systems > Medical > Chemical Synthesizer Operations

# Chemical Synthesizer Operations

<img src="../../assets/raptor_idle_south.png" width="96" align="right">

Operational reference for the Chemical Synthesizer: compound formulae, import strings, species considerations, and container specifications for station pharmacopoeia and industrial reagent production.

---

## Quick Reference

### Equipment

| Item | Capacity | Notable |
|---|---|---|
| [Chemical Synthesizer](#chemical-synthesizer) | 24 base cartridges | Catalysts loaded separately; 5u recharge per cycle |
| [Beaker](#beaker) | 50u | Standard vessel; reagents react on contact |
| [Large Beaker](#large-beaker) | 100u | High-volume runs |
| [Bluespace Beaker](#bluespace-beaker) | 300u | Full-capacity runs; not in base storage |
| [Cryostasis Beaker](#cryostasis-beaker) | 50u | Suppresses reactions; no capacity increase |
| [Vial](#vial) | 30u | Precision dosing; accepts labels |

### Medical Compounds

| Compound | Primary Use | Notable |
|---|---|---|
| [Inaprovaline](#inaprovaline) | Stabilization; pain suppression | Holds critical patients; does not heal; OD 60u |
| [Antitoxin (Dylovene)](#antitoxin-dylovene) | Toxin clearance | Broad-spectrum; OD 30u |
| [Kelotane](#kelotane) | Burn damage treatment | Causes Brute in Prometheans; OD 30u |
| [Synaptizine](#synaptizine) | Anti-stun; neurological clearance | Clears Mindbreaker; very slow metabolism; OD 30u |
| [Hyperzine](#hyperzine) | Movement stimulant | OD 15u; cardiac damage risk on overdose |
| [Claridyl](#claridyl) | High-potency analgesic; stabilizer | 33% yield; Tesshari adverse reaction risk |

### Other Compounds

| Compound | Classification | Notable |
|---|---|---|
| [Bliss](#bliss) | Psychoactive | No medical use; OD causes Brain and Toxic damage |
| [Aphrodisiac](#aphrodisiac) | Pheromone agent | No medical use; 86% yield |
| [Cryptobiolin](#cryptobiolin) | Vestibular disruptor | Fast metabolism; brief effects |
| [Impedrezene](#impedrezene) | Neurological depressant | Weapons-grade; accumulates Brain damage |
| [Mutagen](#mutagen) | Genetic mutagen | Unpredictable outcomes; precursor for Left4Zed |

### Chained and Industrial Synthesis

| Compound | Type | Notable |
|---|---|---|
| [Space Cleaner](#space-cleaner) | Industrial decontaminant | Chains from Hydrogen, Nitrogen, Water; kills Macrophage |
| [Diethylamine](#diethylamine) | Synthesis precursor | Required for Left4Zed |
| [Left4Zed](#left4zed) | Hydroponics fertilizer | Toxic if ingested; 9u minimum clean batch |
| [Silicate](#silicate) | Window reinforcement agent | Topical application only |

### Reference Tables

| Table | Purpose |
|---|---|
| [Inhibitor Reference](#appendix-a-inhibitor-reference) | Silent-fail inhibitors per compound; check before reusing vessels |
| [Catalyst Reference](#appendix-b-catalyst-reference) | Catalyst slot reagents; catalysts not consumed in synthesis |

---

## Chemical Synthesizer

<img src="../../assets/chem_synthesizer.png" width="96" align="right">

The **Chemical Synthesizer** produces chemical compounds from a set of 24 built-in reagent cartridges. Reagents are added in sequence via a production queue. Reactions occur inside the machine's internal vessel and the product is dispensed into a container placed in the output slot.

**Base cartridge supply (24 reagents)**

| | | | |
|---|---|---|---|
| Hydrogen | Carbon | Nitrogen | Oxygen |
| Fluorine | Chlorine | Sodium | Potassium |
| Lithium | Aluminium | Silicon | Phosphorus |
| Sulfur | Iron | Copper | Mercury |
| Tungsten | Calcium | Radium | Water |
| Ethanol | Sugar | Sulfuric Acid | |

Cartridges recharge at 5u per cycle. High-volume queues may outpace recharge on heavily demanded reagents such as Oxygen, Carbon, Sugar, and Hydrogen. Plan accordingly.

**How to read import strings:** Import strings use the format `Reagent,volume,Reagent,volume,...` where chemical names are case-sensitive and must match cartridge labels exactly. Each entry below includes a scaling ratio. For example, `1:1:1 → 3u` means one unit of each ingredient yields three units of product; scale linearly.

**OD** denotes overdose threshold. Standard threshold is 30u for most personnel. Species variation applies.

---

## Containers

Containers receive output from the synthesizer and carry reagents for administration or further use. Placing the correct container in the output slot before queuing a batch determines the available volume.

---

### Beaker

<img src="../../assets/chem_beaker.png" width="48" align="right">

The **beaker** is the standard reaction and transfer vessel. It holds up to 50u of reagent. Reagents placed in the same beaker react automatically if a valid reaction exists; this makes it useful for chaining synthesis outside the machine, but also a contamination risk if multiple reagents are present unexpectedly.

---

### Large Beaker

<img src="../../assets/chem_beaker_large.png" width="48" align="right">

The **large beaker** holds up to 100u. Used for high-volume production runs where the standard beaker capacity is insufficient. Reaction behavior is identical to the standard beaker.

---

### Bluespace Beaker

<img src="../../assets/chem_beaker_bluespace.png" width="48" align="right">

The **bluespace beaker** holds up to 300u. Suitable for full-capacity synthesizer runs and bulk transfer operations. Available through requisition or research supply; not stocked in base chemistry storage.

---

### Cryostasis Beaker

<img src="../../assets/chem_beaker_noreact.png" width="48" align="right">

The **cryostasis beaker** suppresses chemical reactions between its contents. Reagents placed inside do not react with each other regardless of concentration. This makes it the correct storage vessel when carrying multiple reactive compounds simultaneously, or when preserving an intermediate reagent for use in a later step. Capacity is 50u. The cryostasis effect is purely contained; reagents behave normally once transferred to a standard vessel.

---

### Vial

<img src="../../assets/chem_vial.png" width="48" align="right">

The **vial** holds up to 30u. Used for precise small-volume doses and individual patient dispensing. Vials accept labels for identification.

---

## Section I: Direct Synthesis

Single-step reactions achievable without intermediate compounds.

---

## Inaprovaline

**Classification:** Synaptic Stimulant / Cardiostimulant
**Reaction:** `Oxygen,1 + Carbon,1 + Sugar,1 → 3u` · Scale 1:1:1
**Inhibitor:** Water. Reaction fails silently if present. Use a dry vessel.
**OD threshold:** 60u
**Dermal absorption:** Partial

Inaprovaline is a front-line stabilization agent. Its primary function is to slow the physiological deterioration of critically injured patients, buying time for proper treatment. It also suppresses pain signaling and clears the biochemical cascade triggered by allergic reactions. A patient on Inaprovaline will not deteriorate faster, even if untreated. Inaprovaline does not heal damage; it only holds the line.

Diona patients do not respond. All other species process it normally.

| Output | String |
|--------|--------|
| 6u | `Oxygen,2,Carbon,2,Sugar,2` |
| 15u | `Oxygen,5,Carbon,5,Sugar,5` |
| 30u | `Oxygen,10,Carbon,10,Sugar,10` |
| 60u | `Oxygen,20,Carbon,20,Sugar,20` |
| 120u | `Oxygen,40,Carbon,40,Sugar,40` |

> Minimum clean batch: 3u (1+1+1). 5u requires fractional volumes. Use 6u instead.

---

## Antitoxin (Dylovene)

**Classification:** Broad-Spectrum Antitoxin
**Reaction:** `Silicon,1 + Potassium,1 + Nitrogen,1 → 3u` · Scale 1:1:1
**OD threshold:** 30u
**Dermal absorption:** Partial

Dylovene is the station's primary counter to Toxic damage. It clears accumulated toxins from the bloodstream, reduces drowsiness and hallucination effects caused by poisoning, and has a small chance per dose of fully purging an active poison modifier. Effective against most environmental and biological toxins.

Diona patients do not respond. Promethean patients at doses above 15u will experience mild disorientation; dose carefully in conscious subjects.

| Output | String |
|--------|--------|
| 6u | `Silicon,2,Potassium,2,Nitrogen,2` |
| 15u | `Silicon,5,Potassium,5,Nitrogen,5` |
| 30u | `Silicon,10,Potassium,10,Nitrogen,10` |
| 60u | `Silicon,20,Potassium,20,Nitrogen,20` |
| 120u | `Silicon,40,Potassium,40,Nitrogen,40` |

---

## Kelotane

**Classification:** Burn Damage Treatment
**Reaction:** `Silicon,1 + Carbon,1 → 2u` · Scale 1:1
**Inhibitor:** Water. Fails silently if present. Dry vessel mandatory.
**OD threshold:** 30u
**Dermal absorption:** Partial

Kelotane is the standard treatment for Burn damage. It accelerates tissue repair at a rate of 4u Burn healed per unit metabolized, scaled to species healing capacity.

**Promethean (Slime) warning:** Kelotane repairs burn tissue in Prometheans but simultaneously damages their silicate skeletal structure, causing 2u Brute per metabolization cycle. For Promethean burn patients, consult alternative burn treatments or monitor closely for compounding injury.

Diona patients do not respond.

| Output | String |
|--------|--------|
| 5u | `Silicon,2.5,Carbon,2.5` |
| 15u | `Silicon,7.5,Carbon,7.5` |
| 30u | `Silicon,15,Carbon,15` |
| 60u | `Silicon,30,Carbon,30` |
| 120u | `Silicon,60,Carbon,60` |

> Decimal volumes are valid in production mode. Minimum clean integer batch: 2u (1+1).

---

## Synaptizine

**Classification:** Neurostimulant / Anti-Stun Agent
**Reaction:** `Sugar,1 + Lithium,1 + Water,1 → 3u` · Scale 1:1:1
**OD threshold:** 30u
**Dermal absorption:** Partial
**Metabolism rate:** Very slow; single dose remains active for an extended period.

Synaptizine is used to treat neurological suppression. It clears drowsiness, counters paralysis, stun, and weakness effects, and actively purges Mindbreaker (hallucinogen) from the bloodstream with each metabolization cycle. Its slow processing rate means a single dose provides extended coverage.

Promethean patients at dose ≥5u gain Brute and Burn healing from Synaptizine at the cost of accelerated nutrition consumption. Diona patients do not respond.

Water is a required ingredient, not an inhibitor. Ensure no excess Water is already present from prior reactions; it will not block Synaptizine synthesis but will interfere with any co-queued Inaprovaline or Kelotane.

| Output | String |
|--------|--------|
| 6u | `Sugar,2,Lithium,2,Water,2` |
| 15u | `Sugar,5,Lithium,5,Water,5` |
| 30u | `Sugar,10,Lithium,10,Water,10` |
| 60u | `Sugar,20,Lithium,20,Water,20` |
| 120u | `Sugar,40,Lithium,40,Water,40` |

---

## Hyperzine

**Classification:** Muscle Stimulant / Movement Enhancer
**Reaction:** `Sugar,1 + Phosphorus,1 + Sulfur,1 → 3u` · Scale 1:1:1
**OD threshold:** 15u (half the standard threshold). Handle carefully.
**Dermal absorption:** Partial

Hyperzine is a powerful long-acting muscle stimulant that increases movement speed significantly. It is standard emergency-response issue for personnel who require rapid cross-station transit.

**Overdose hazard:** Overdose causes intermittent cardiac stress, with a non-zero chance of direct heart organ damage per metabolization cycle. A 30u bottle is sufficient for most standard deployments.

Tajara metabolize Hyperzine at 1.25× potency; reduce dosing accordingly. Promethean patients experience skeletal instability rather than clean speed enhancement, and at dose ≥5u nutrition is burned at an accelerated rate. Diona patients do not respond.

| Output | String |
|--------|--------|
| 6u | `Sugar,2,Phosphorus,2,Sulfur,2` |
| 15u | `Sugar,5,Phosphorus,5,Sulfur,5` |
| 30u | `Sugar,10,Phosphorus,10,Sulfur,10` |
| 60u | `Sugar,20,Phosphorus,20,Sulfur,20` |
| 120u | `Sugar,40,Phosphorus,40,Sulfur,40` |

---

## Impedrezene

**Classification:** Neurological Depressant / Incapacitant
**Reaction:** `Mercury,1 + Oxygen,1 + Sugar,1 → 2u` · Scale 1:1:1 at 66% yield
**OD threshold:** 30u
**Filtered by:** Spleen organ

Impedrezene slows higher cognitive function, impairs coordination, and induces progressive drowsiness and Brain damage with sustained exposure. It is classified internally as a weapons-grade compound. Practical medical use is limited; it sees occasional application in sedation protocols where Chloral Hydrate is unavailable, with a significant side effect profile.

At low concentrations: reduces motor jitter, causes mild drowsiness, slowly accumulates Brain damage. At prolonged exposure: drooling, incoherence, compounding Brain damage.

Diona patients do not respond.

**Yield note:** 3u of reagents yields only 2u of product. Scale accordingly.

| Output | String |
|--------|--------|
| 5u | `Mercury,2.5,Oxygen,2.5,Sugar,2.5` |
| 15u | `Mercury,7.5,Oxygen,7.5,Sugar,7.5` |
| 30u | `Mercury,15,Oxygen,15,Sugar,15` |
| 60u | `Mercury,30,Oxygen,30,Sugar,30` |
| 120u | `Mercury,60,Oxygen,60,Sugar,60` |

---

## Mutagen

**Classification:** Genetic Mutagen / Synthesis Precursor
**Reaction:** `Radium,1 + Phosphorus,1 + Chlorine,1 → 3u` · Scale 1:1:1

Mutagen induces random genetic mutations in organic subjects. Administration route affects delivery: blood injection is most reliable, ingestion has a 67% trigger chance, and topical application only 33%. Synthetic units are immune. Dionaea are unaffected.

Mutation outcomes are entirely unpredictable and range from cosmetic to debilitating. This compound should not be administered therapeutically. Its primary station use is as a precursor reagent in the synthesis of [Left4Zed](#left4zed).

| Output | String |
|--------|--------|
| 6u | `Radium,2,Phosphorus,2,Chlorine,2` |
| 15u | `Radium,5,Phosphorus,5,Chlorine,5` |
| 30u | `Radium,10,Phosphorus,10,Chlorine,10` |
| 60u | `Radium,20,Phosphorus,20,Chlorine,20` |
| 120u | `Radium,40,Phosphorus,40,Chlorine,40` |

---

## Claridyl

**Classification:** Analgesic / Stabilizer (Advanced)
**Reaction:** `Lithium,1 + Radium,1 + Sugar,1 → 1u` · Scale 1:1:1 at 33% yield
**OD threshold:** Effectively non-toxic at any practical dose
**Metabolism rate:** Slow; extended active duration
**Dermal absorption:** Full

Claridyl is a high-potency analgesic and patient stabilizer. It provides the strongest stabilization and pain suppression available from this machine: roughly double Inaprovaline's stabilization strength and quadruple its analgesic effect. Extremely effective at keeping critical patients functional and alive under sustained injury.

At therapeutic doses it very slowly repairs minor Brute damage; however, each unit repaired costs proportional Hallucination damage, trading one problem for another.

**Critical note for Tesshari (Tesh) personnel:** An extremely rare adverse reaction exists in which a single dose causes 50u of Toxic damage instantly. Document and flag any Tesh patients who report adverse reactions to Claridyl.

Minor behavioral side effects (irritability, cognitive lapses, dry mouth, mild dizziness) occur at low probability per cycle.

**Yield note:** 3u of reagents produces only 1u of product. A 60u bottle consumes 180u of feedstock.

| Output | String |
|--------|--------|
| 5u | `Lithium,5,Radium,5,Sugar,5` |
| 15u | `Lithium,15,Radium,15,Sugar,15` |
| 30u | `Lithium,30,Radium,30,Sugar,30` |
| 60u | `Lithium,60,Radium,60,Sugar,60` |
| 120u | `Lithium,120,Radium,120,Sugar,120` |

> 120u batch consumes 360u total feedstock. Allow time for Lithium, Radium, and Sugar cartridge recharge.

---

## Bliss

**Classification:** Psychoactive / Controlled Substance
**Reaction:** `Mercury,1 + Sugar,1 + Lithium,1 → 3u` · Scale 1:1:1
**OD threshold:** 30u

Bliss is a psychoactive compound producing a pronounced euphoric high, disorientation, and periodic involuntary movement and emotional expression. Subjects experience elevated mood, perceptual distortion, and reduced inhibition. Overdose causes hallucinations and accumulates Brain damage and Toxic damage per cycle.

Prometheans experience significantly reduced effect due to biochemical resistance to toxin-class compounds. Diona patients do not respond. No therapeutic application; synthesis documented for completeness.

| Output | String |
|--------|--------|
| 6u | `Mercury,2,Sugar,2,Lithium,2` |
| 15u | `Mercury,5,Sugar,5,Lithium,5` |
| 30u | `Mercury,10,Sugar,10,Lithium,10` |
| 60u | `Mercury,20,Sugar,20,Lithium,20` |
| 120u | `Mercury,40,Sugar,40,Lithium,40` |

---

## Aphrodisiac

**Classification:** Pheromone Agent
**Reaction:** `Carbon,2 + Hydrogen,2 + Oxygen,2 + Water,1 → 6u` · Scale 2:2:2:1 at 86% yield

Aphrodisiac produces mild behavioral and pheromone effects in subjects. Physical response is subtle. No therapeutic or emergency medical value; no damage profile. Synthesis documented for completeness.

**Yield note:** 7u of feedstock yields 6u of product.

| Output | String |
|--------|--------|
| 6u | `Carbon,2,Hydrogen,2,Oxygen,2,Water,1` |
| ~18u | `Carbon,6,Hydrogen,6,Oxygen,6,Water,3` |
| 30u | `Carbon,10,Hydrogen,10,Oxygen,10,Water,5` |
| 60u | `Carbon,20,Hydrogen,20,Oxygen,20,Water,10` |
| 120u | `Carbon,40,Hydrogen,40,Oxygen,40,Water,20` |

> 15u is not achievable in clean integers. Nearest batches: 12u (`Carbon,4,Hydrogen,4,Oxygen,4,Water,2`) or 18u.

---

## Cryptobiolin

**Classification:** Vestibular Disruptor / Incapacitant
**Reaction:** `Potassium,1 + Oxygen,1 + Sugar,1 → 3u` · Scale 1:1:1
**OD threshold:** 30u
**Metabolism rate:** Fast; effects are short-lived.

Cryptobiolin is a vestibular disruption agent. It induces dizziness and cognitive confusion in affected subjects, with effect strength scaling to species toxin sensitivity. Prometheans experience significantly reduced effect. Diona patients do not respond. No medical use.

| Output | String |
|--------|--------|
| 6u | `Potassium,2,Oxygen,2,Sugar,2` |
| 15u | `Potassium,5,Oxygen,5,Sugar,5` |
| 30u | `Potassium,10,Oxygen,10,Sugar,10` |
| 60u | `Potassium,20,Oxygen,20,Sugar,20` |
| 120u | `Potassium,40,Oxygen,40,Sugar,40` |

---

## Section II: Chained Synthesis

The reactions below require intermediates that can be generated within the same recipe by supplying all feedstock at once. The synthesizer vessel allows reactions to chain automatically. All ingredients are added in a single recipe run; do not attempt to manually separate steps.

> **Inhibitor reminder:** Ammonia synthesis is blocked by Phoron. If the catalyst slot contains Phoron, disable catalyst use before running these recipes.

---

## Ammonia

**Classification:** Industrial Precursor / Fertilizer Base
**Reaction:** `Hydrogen,3 + Nitrogen,1 → 3u` · Scale 3:1

Not directly useful for most personnel. Produced as an intermediate in Space Cleaner and Diethylamine synthesis.

| Output | String |
|--------|--------|
| 15u | `Hydrogen,15,Nitrogen,5` |
| 30u | `Hydrogen,30,Nitrogen,10` |
| 60u | `Hydrogen,60,Nitrogen,20` |

---

## Space Cleaner

**Classification:** Industrial Cleaning Agent
**Chain:** `3H + 1N → Ammonia` → `Ammonia + Water → 2u Space Cleaner`
**Net ratio:** H×1 + N×(1/3) + Water×1 per unit of output

Space Cleaner decontaminates surfaces, objects, and personnel of most biological and chemical residue. It extinguishes lit smoking articles on contact with subjects and is effective against Macrophage viral entities (20 Toxic on contact).

Adding Hydrogen, Nitrogen, and Water together in one recipe causes them to chain automatically: Hydrogen and Nitrogen react first to form Ammonia, which immediately reacts with Water to form Space Cleaner.

| Output | String |
|--------|--------|
| ~15u | `Hydrogen,7.5,Nitrogen,2.5,Water,7.5` |
| 30u | `Hydrogen,15,Nitrogen,5,Water,15` |
| 60u | `Hydrogen,30,Nitrogen,10,Water,30` |
| 120u | `Hydrogen,60,Nitrogen,20,Water,60` |

---

## Diethylamine

**Classification:** Synthesis Precursor
**Chain:** `3H + 1N → Ammonia` → `Ammonia + Ethanol → 2u Diethylamine`
**Net ratio:** H×1 + N×(1/3) + Ethanol×1 per unit of output

Diethylamine is a secondary amine with mild corrosive properties and no direct therapeutic use. It is the primary intermediary required for Left4Zed synthesis and several advanced compounds not producible on this machine.

| Output | String |
|--------|--------|
| ~15u | `Hydrogen,7.5,Nitrogen,2.5,Ethanol,7.5` |
| 30u | `Hydrogen,15,Nitrogen,5,Ethanol,15` |
| 60u | `Hydrogen,30,Nitrogen,10,Ethanol,30` |
| 120u | `Hydrogen,60,Nitrogen,20,Ethanol,60` |

---

## Left4Zed

**Classification:** Hydroponics Fertilizer
**Chain:** `3H + 1N → Ammonia` → `Ammonia + Ethanol → Diethylamine` → `2 Diethylamine + Mutagen → 3u Left4Zed`
**Parallel chain:** `Radium + Phosphorus + Chlorine → Mutagen` (runs simultaneously)
**Net ratio (per 9u output):** H×3, N×1, Ethanol×3, Radium×1, Phosphorus×1, Chlorine×1

Left4Zed is a hydroponics plant fertilizer that accelerates plant growth cycles in the hydroponics bay. In the bloodstream it acts as a mild toxin; personnel should not consume it intentionally.

**Batch sizing note:** Clean integer batches occur only at multiples of 9u due to the 3:1 Hydrogen:Nitrogen ratio and 2:1 Diethylamine:Mutagen ratio.

| Output | String |
|--------|--------|
| 9u | `Hydrogen,3,Nitrogen,1,Ethanol,3,Radium,1,Phosphorus,1,Chlorine,1` |
| ~27u | `Hydrogen,9,Nitrogen,3,Ethanol,9,Radium,3,Phosphorus,3,Chlorine,3` |
| ~63u | `Hydrogen,21,Nitrogen,7,Ethanol,21,Radium,7,Phosphorus,7,Chlorine,7` |
| ~126u | `Hydrogen,42,Nitrogen,14,Ethanol,42,Radium,14,Phosphorus,14,Chlorine,14` |

> Nearest to 30u is 27u. Nearest to 60u is 63u. Nearest to 120u is 126u.

---

## Section III: Engineering / Industrial

---

## Silicate

**Classification:** Glass Reinforcement Agent
**Reaction:** `Aluminium,1 + Silicon,1 + Oxygen,1 → 3u` · Scale 1:1:1

Silicate is applied topically to window structures to reinforce them against impact and damage. It has no effect when administered to personnel.

| Output | String |
|--------|--------|
| 15u | `Aluminium,5,Silicon,5,Oxygen,5` |
| 30u | `Aluminium,10,Silicon,10,Oxygen,10` |
| 60u | `Aluminium,20,Silicon,20,Oxygen,20` |
| 120u | `Aluminium,40,Silicon,40,Oxygen,40` |

---

## Section IV: Not Achievable on This Machine

| Compound | Reason |
|----------|--------|
| Leporazine | Requires Phoron as catalyst; not in base supply |
| Mead | Requires Enzyme catalyst; not in base supply |
| Hooch | Requires Fuel; not in base supply |
| Manlydorf | Requires Beer and Ale; not producible |
| Matcha Latte | Requires Matcha Powder and Milk; not producible |
| RobustHarvest | Requires Neurotoxic Protein; not producible |
| Most advanced compounds | Require Phoron catalyst, Plasticide, or brewed alcohol |

---

## Appendix A: Inhibitor Reference

Reactions that fail silently if these chemicals are present in the vessel. A failed reaction leaves all reagents unreacted with no output and no indication of failure. Rinse between batches if reusing the vessel.

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

## Appendix B: Catalyst Reference

<img src="../../assets/chem_cartridge.png" width="48" align="right">

Catalysts are loaded into the catalyst slot and returned to it after each recipe completes. They are not consumed in synthesis.

| Reaction | Catalyst | Available from base supply? |
|----------|----------|-----------------------------|
| Fire Foam | 10u Fluorine | Yes |
| Leporazine | Phoron | No |
| Mead | Enzyme | No |

To produce Fire Foam: load 10u Fluorine into the catalyst bottle, seat it in the machine, enable catalyst use, then queue recipes using only Water as the synthesis ingredient. Fluorine is extracted and re-seated between each run automatically.

---

*All entries compiled from direct station system analysis. ARGUS.*
