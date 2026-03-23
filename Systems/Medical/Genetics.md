[ARGUS Station Database](../../README.md) > [Systems](../README.md) > [Medical](README.md) > Genetics

# Genetics

<img src="../../assets/raptor_idle_south.png" width="96" align="right">

Station genetics operations cover DNA scanning and manipulation, gene isolation and transfer via injectors, and the growing of new bodies from stored genetic records.

---

## Quick Reference

| Item | Function | Notable |
|---|---|---|
| [GenePeeper 3000](#genepeeper-3000) | Handheld gene scanner | Reads traits, enzymes, radiation, clone loss |
| [DNA Modifier](#dna-modifier) | Scanner pod; subject enters for manipulation | Accepts beakers for reagent injection |
| [DNA Modifier Console](#dna-modifier-console) | Controls the modifier; buffer and irradiation management | 3 internal buffers; disk and sleeve support |
| [Cloning Console](#cloning-console) | Manages stored body records and initiates body growing | Links to grow pod in area |
| [Grow Pod](#grow-pod) | Grows bodies from buffer records | Requires biomass |
| [Clone Pod](#clone-pod) | Legacy cloning hardware | **Non-operational** |
| [Body Record Disk](#body-record-disk) | Portable storage for a single body record | Usable in both modifier console and cloning console |
| [DNA Injector](#dna-injector) | Applies a single buffered SE block to a target | Created at the modifier console |
| [Positive Genes](#positive-genes) | Superpowers; not present at round start | Require irradiation or injectors to activate |
| [Negative Genes](#negative-genes) | Disabilities; may be present at round start | Can be suppressed by buffer transfer |
| [Neutral Genes](#neutral-genes) | Behavioral traits | Cost 0 or minor negative |
| [Gene Traits](#gene-traits) | Genetic variants documented in scanner readouts alongside standard genes | All use Default activation threshold |
| [Side Effects](#side-effects) | Complications from genetic procedures | 3 types; each has a specific antidote |
| [Growing a Body](#growing-a-body) | Full workflow from scan to revival | Operational |
| [Species Compatibility](#species-compatibility) | Which species can be scanned and sleeved | Lleill: scan only; many species fully incompatible |

---

## Equipment

### GenePeeper 3000

<img src="../../assets/gen_scanner.png" width="96" align="right">

The **GenePeeper 3000** is a belt-slot handheld scanner. Applying it to a living mob, an organ, or a DNA injector begins a 6-second scan. On completion, the device produces a readout showing unique enzymes, blood type, current radiation level, clone loss, and a list of all active genes with their encoded block values and descriptions. Genes that are present but suppressed by trait conflicts are flagged as suppressed.

If the subject's genetics are flagged as unstable, the readout notes this directly. Species whose biology is incompatible with the scanning equipment are flagged as not acceptable for genetic sampling. Severe irradiation (above 200 units) and husked anatomical structure are reported separately.

Scanning your own genome is useful for locating the SE blocks of traits you already have expressed.

---

### DNA Modifier

<img src="../../assets/gen_dna_scanner.png" width="96" align="right">

The **DNA Modifier** is a walk-in pod. A subject enters by moving into it; the modifier can also accept a subject via drag-and-drop by another person, or by insertion of a preserved brain organ. Subjects with abiotic items cannot enter. Borgs cannot be scanned.

A beaker may be loaded into the modifier to allow reagent injection through the console. The modifier links to an adjacent DNA Modifier Console to the north, south, east, or west.

---

### DNA Modifier Console

<img src="../../assets/gen_console.png" width="96" align="right">

The **DNA Modifier Console** provides three operational tabs.

**SE tab** (Structural Enzymes): Displays the active genes of the current occupant. Shows unique enzymes, unique identity, and structural enzyme string for reference. Only structural enzyme blocks are editable through this console; unique identity and unique enzymes are read-only. Allows selection of a specific SE block (1 to 93) and subblock (1 to 3) for targeted irradiation. Irradiation controls set duration (1 to 20) and intensity (1 to 10).

Two irradiation modes are available. **SE irradiation** targets the selected block directly. On success (probability of 80 plus half the duration), the block values are randomly scrambled and there is a 20% chance the result is applied to an adjacent block instead. On failure, a random bad mutation is applied and the subject receives radiation. > [!WARNING]
> Full pulse irradiation carries a 95% probability of applying a random negative mutation and always inflicts radiation damage scaled to intensity and duration. Reserve for deliberate mutation attempts with informed subject consent.

**Full pulse** irradiates the whole body: 95% probability of a random bad mutation, 5% probability of a random good mutation. Both modes lock the modifier for the irradiation duration and apply radiation damage scaled to intensity and duration.

**Buffer tab**: Three numbered buffers, each holding a body record. Buffers can be saved from the current occupant, loaded from a body record disk, cleared, or relabeled. A buffer can be transferred to the current occupant, overwriting their structural enzymes; the occupant is irradiated and all active genes are re-evaluated. A buffer can produce a DNA injector (with a 5-second cooldown per injector). The **Sleeve** option sends the buffer record to the grow pod in the area to begin growing a body from the stored record.

**Rejuvenators tab**: If a beaker is loaded into the modifier, reagents can be injected directly into the current occupant in 5-unit increments up to 50 units per action.

A body record disk can be inserted into the console. Buffers can be saved to or loaded from the disk. The disk can also be ejected or wiped.

The occupant can be ejected at any time via the console. The disk is also ejected when the occupant is released.

---

### Cloning Console

The **Cloning Console** manages stored body records and initiates body growing cycles. It links to all grow pods in the same area.

The console stores body records created from successful scans. Each record holds the subject's unique enzymes, unique identity, structural enzymes, and a reference to a health implant installed in the subject at scan time. When a scan is initiated, the console verifies that the subject is alive, has a brain, is responsive, does not carry a genetic instability marker that prevents scanning, and has not already been scanned this session. Species whose biology is incompatible with the scanning equipment return an error message.

The console can operate in **standard scan mode** or **brain scan mode**. Brain scan mode requires a scanner with scan level 4 or higher (tier 4 scanning module) and produces a higher-fidelity record. Autoprocess mode (scan level 3 or higher) automatically scans occupants and starts growing without manual intervention.

When a deceased crew member's body is placed in the scanner, their consciousness is notified and prompted to return if it remains present nearby.

Records can be deleted from the console using a head-of-staff ID card to confirm the action.

A body record disk can be inserted to load a record from disk or save the active record to disk for transport.

---

### Grow Pod

The **Grow Pod** grows organic bodies from body records sent to it from the DNA Modifier Console or Cloning Console. It requires sufficient biomass to begin a growing cycle. Only one occupant can be grown at a time. A pod showing a mess state has malfunctioned mid-cycle and must be cleared before use.

The pod heals its occupant at a fixed rate during the growing cycle. The console displays biomass level, current status (idle, growing, or malfunction), and growing progress.

---

### Clone Pod

> **The Clone Pod is non-operational.** This legacy hardware has been replaced by the Grow Pod. It is present in some areas but does not function.

---

### Body Record Disk

<img src="../../assets/gen_bodydisk.png" width="96" align="right">

The **Body Record Disk** carries a single complete body record: structural enzymes, unique identity, gender, and genetic modifiers. It is accepted by both the DNA Modifier Console and the Cloning Console. The disk is used to transfer records between systems, store a backup before major manipulation, or load a pre-prepared gene template.

---

### DNA Injector

<img src="../../assets/gen_dna_injector.png" width="96" align="right">

A **DNA Injector** carries a single SE buffer or a specific SE block from a buffer. Applying the injector to a subject rewrites the corresponding portion of their structural enzymes and triggers a mutation check. Some injectors carry a radiation risk that causes additional radiation damage on injection. Each injector is labeled with its buffer name; block injectors include the block identifier in their name.

---

## DNA Structure

Every organic crew member carries a DNA record with three components.

**Unique Identity (UI)**: 65 values encoding visible physical traits: hair color, beard color, skin tone, skin color, eye color, gender, player scale, tail color and style, ear style and color, ear secondary colors, wing style and color, and gradient style and color. The UI defines appearance and is edited through the body design terminal, not the DNA Modifier Console.

**Structural Enzymes (SE)**: 93 slots, each 3 values wide (block size 3). These slots encode active gene traits. Each gene occupies one block. Whether a gene is active depends on whether the block values fall within the gene's activity bounds. Irradiation changes block values, potentially activating or deactivating genes. Most blocks have a corresponding gene; approximately five blocks are unassigned and produce no mutation result when irradiated.

**Unique Enzymes (UE)**: A short alphanumeric string unique to each individual. Used as a genetic fingerprint for identification and forensic purposes. Not modifiable through the DNA Modifier.

Only SE blocks are editable through the DNA Modifier Console. UI and UE are read-only from the genetics workstation.

Activity bounds determine how narrow the window for gene activation is. Three tiers are in use:

| Tier | Activation Threshold | Notes |
|---|---|---|
| Default | 802 and above | Standard window; used by beneficial and negative trait genes |
| Hard | BEA and above | Narrower window; most superpowers and selected negative genes |
| Harder | DAC and above | Tightest window; most difficult to activate and maintain |

Threshold values are the SE block values (hex-encoded) at which a gene becomes active. Lower thresholds are easier to reach through irradiation.

If irradiating a block produces no visible result, there are two possible causes: the block is one of the unassigned dud blocks, or a mutually exclusive gene is suppressing expression. Check the gene scan output for suppression flags before concluding a block is empty.

---

## Positive Genes

Positive gene traits are superpowers. All are hidden by default and cannot be selected at character creation. They must be activated through targeted irradiation or DNA injectors.

| Gene | Bounds | Effect |
|---|---|---|
| No Breathing | Harder | Subject does not need to breathe |
| Remote Viewing | Hard | Subject can view through the eyes of other individuals |
| Regenerate | Hard | Subject slowly repairs wounds and internal bleeding |
| Telepathy | Hard | Subject can communicate remotely |
| No Prints | Default | Subject leaves no fingerprints |
| X-Ray Vision | Hard | Subject can see through walls |
| Telekinesis | Harder | Subject can move objects without physical contact |
| Laser Vision | Harder | Subject fires lasers from eyes on harm intent |
| Hulk | Harder | Subject gains enhanced strength; auto-deactivates below 25 health |
| Flash Resistance | Hard | Subject's eyes are protected against intense flash blindness |
| Morph | Hard | Subject gains access to a body transformation interface |

Hulk deactivation is automatic when the subject's health drops below 25: the genetic activation is suppressed and the subject is briefly weakened.

---

## Negative Genes

Negative gene traits are disabilities. Some may be present in a subject's baseline DNA.

| Gene | Effect | Notes |
|---|---|---|
| Epilepsy | Periodic seizures | |
| Coughing Fits | Uncontrollable coughing | |
| Clumsy | 15% chance to fumble; 10% chance to harm self with tools | |
| Coprolalia | Periodic involuntary profanity outbursts | |
| Mute | Cannot speak | Mutually exclusive with Incomprehensible |
| Deaf | Cannot hear | |
| Nearsighted | Reduced vision range | |
| Incomprehensible | Speech is unintelligible gibberish | Mutually exclusive with Mute |
| Rotting Genetics | Random limb and organ deterioration over time | Mutually exclusive with Stable Genetics trait |
| Gibbingtons | Body may explode from trauma | Not visible on gene scan |
| Lumbar Impairment | Legs nonfunctional; subject cannot stand | Hard bounds |
| Censored | Cannot use profanity | |
| Nervousness | Periodic stuttering | |

---

## Neutral Genes

| Gene | Effect | Notes |
|---|---|---|
| Tourettes Syndrome | Motor and vocal tics; worsens under stress | Cost 0 |

---

## Gene Traits

Gene traits are genetic variants documented in scanner readouts alongside standard positive and negative gene markers. Each occupies a structural enzyme block and responds to the same activation and suppression methods as any other genetic variant. All gene traits use Default activation threshold.

### Positive Gene Traits

| Gene | Effect |
|---|---|
| Haste | Subject moves faster than baseline |
| Non-Conductive, Major | Susceptibility to electric shocks reduced by 50% |
| Table Passer | Subject passes over or under tables without resistance |
| Radiation Immunity | Subject is completely immune to radiation damage |
| Vibration Sense | Subject can detect subtle vibrations from nearby sources even when the source is not visible |
| Radioactive Heal | Subject heals when exposed to radiation rather than suffering harm; may emit a glow while irradiated |

### Negative Gene Traits

| Gene | Effect | Notes |
|---|---|---|
| Phoron Breather | Subject breathes phoron; oxygen is toxic | |
| Nitrogen Breather | Subject breathes nitrogen; oxygen is toxic; phoron is non-toxic | |
| Methane Breather | Subject breathes methane; oxygen is toxic | |
| Carbon Dioxide Breather | Subject breathes carbon dioxide; oxygen is non-toxic; exhales oxygen | |
| Nyctalopia | Subject cannot see in darkness | |
| Bad Shot | Severe accuracy penalty with ranged weapons | |
| Slowdown, Extreme | Subject moves extremely slowly | |
| Low Blood Sugar | Adverse effects including hallucinations and unconsciousness when nutrition is depleted | |
| Permanently Blind | Subject is blind; condition cannot be corrected by medical or surgical means | Not visible on gene scan |
| Agoraphobia | Panic and adverse effects when in the company of more than two other individuals | |
| Major Loneliness Vulnerability | Adverse effects during extended isolation; requires social contact beyond most mobs to resolve | |
| Reduced Biocompatibility, Major | Therapeutic chemicals are only 30% as effective | |
| Photosensitivity, Major | Flash and light-based stun duration doubled | |
| Pain Intolerance, Major | All pain sources are 50% more intense | |
| Sensitive Biochemistry, Major | Toxin damage and negative drug effects doubled; knockout compounds take effect faster | |
| Unlucky, Major | Subject experiences extreme bad luck; effects can be fatal | |
| Photodegeneration | Body deteriorates when exposed to light without suit protection | Not visible on gene scan |
| Weakling, Major | Heavy equipment causes significantly increased movement slowdown | |
| Lightweight | Light frame and poor balance; highly susceptible to displacement from impacts | |
| Conductive, Major | Susceptibility to electric shocks doubled | |

### Neutral Gene Traits

| Gene | Effect |
|---|---|
| Cold Adapted | Significantly improved cold resistance; increased vulnerability to heat |
| Heat Adapted | Significantly improved heat resistance; increased vulnerability to cold |
| Allergy: Chocolate | Severe allergic reaction to cocoa and chocolate |
| Allergy: Coffee | Severe allergic reaction to coffee |
| Allergy: Fish | Severe allergic reaction to fish and seafood |
| Allergy: Fruit | Severe allergic reaction to fruit |
| Allergy: Fungi | Severe allergic reaction to fungi and mushrooms |
| Allergy: Gluten | Severe allergic reaction to gluten; most common grains are hazardous |
| Allergy: Lactose | Severe allergic reaction to lactose and dairy products |
| Allergy: Meat | Severe allergic reaction to most forms of meat |
| Allergy: Nuts | Severe allergic reaction to hard-shell seeds and peanuts |
| Allergy: Pollen | Severe allergic reaction to pollen and many plants |
| Allergy: Salt | Severe allergic reaction to sodium chloride |
| Allergy: Soy | Severe allergic reaction to soybeans and related legumes |
| Allergy: Vegetable | Severe allergic reaction to vegetables |
| Colorblindness (Monochromancy) | Complete colorblindness; no color perception |
| Colorblindness (Para Taj) | Minor difficulty distinguishing blue from red |
| Colorblindness (Para Vulp) | Severe difficulty distinguishing green from red |
| Dominate Predator | Subject can attempt to take control of a predator from inside their belly |
| Dominate Prey | Subject can connect to and dominate the brain of prey held inside subject |
| Drippy | Subject cannot contain their form; produces a constant drip or film of sludge |
| Expensive Taste | Subject gains nutrition only from raw ore and refined minerals |
| Glowing Body | Subject's body produces a low-level glow; color and toggle adjustable |
| Glowing Eyes | Subject's eyes remain visible above ambient darkness |
| Liver of Air | Alcohol is three times as potent |
| Liver of Durasteel | Very high alcohol tolerance; only exceptionally strong drinks produce noticeable effects |
| Spice Intolerance, Extreme | Spicy foods are three times as potent |
| Spice Tolerance, Extreme | Spicy foods are effectively non-potent |
| Submit To Prey | Subject can allow prey's mind to exert control over subject's body |
| Trash Can | Subject can dispose of refuse without locating a waste receptacle |
| Waddle | Subject moves with an animated or waddling movement pattern; adjustable |

Gene traits can be activated or suppressed through irradiation and injectors the same as any other gene. If a trait is already expressed by the subject, scanning their own genome will show which SE block encodes it, which can assist in isolating and transferring it.

---

## Side Effects

Genetic procedures can trigger side effects. When a side effect fires, a random type is selected from the three available. The subject is briefly weakened 2 seconds after onset. If the appropriate antidote reagent is present in the subject's bloodstream, ingested, or applied topically at the time the effect resolves, the harmful outcome is prevented.

| Side Effect | Duration | Antidote | Untreated Result |
|---|---|---|---|
| Genetic Burn | 30 seconds | Dexalin | All external organs take 5 brute damage |
| Bone Snap | 60 seconds | Bicaridine | Random limb: 20 brute damage and fracture |
| Genetic Confusion | 30 seconds | Antitoxin | Subject is confused for 100 ticks |

Onset is visible: Genetic Burn causes visible reddening, Bone Snap causes uncontrollable shivering of the limbs, and Genetic Confusion causes drooling. These cues are distinct and allow identification of the active side effect type before it resolves.

---

## Growing a Body

Cloning restores a deceased crew member to a functional body grown from their stored genetic record.

**Requirements for scanning:**
- Subject must be a species compatible with genetic scanning equipment
- Subject must have a brain present
- Subject must be responsive
- Subject must not carry a genetic instability marker that prevents scanning
- Subject must not have committed suicide
- Subject must not already have a record stored this session

**Standard procedure:**

1. Place the subject in the DNA Modifier adjacent to the Cloning Console.
2. At the Cloning Console, initiate a scan. The console stores the resulting body record and installs a health implant in the subject to track vitals remotely.
3. Confirm biomass is available in the grow pod.
4. Select the record from the Records menu and choose Sleeve. The console sends the record to the grow pod and starts the growing cycle.
5. The grow pod grows the body over time. The subject's consciousness can re-enter the body on completion.

Alternatively, a body record can be sent to the grow pod directly from the DNA Modifier Console buffer tab using the Sleeve option, without going through the Cloning Console.

If brain scan mode is available (scanner tier 4), enable it before scanning for a higher-fidelity record.

Autoprocess mode (scanner tier 3 or higher) scans occupants and starts growing automatically without manual intervention at each step.

Records can be saved to a body record disk for later revival or transfer. Records can be loaded back from disk through the console's disk management options.

---

## Species Compatibility

Not all species possess standard organic DNA. Species whose biological composition is incompatible with the scanning equipment will return an error when placed in the modifier or scanned at the cloning console. Some species carry readable genetic material but lack the biological substrate required to grow a body.

| Species | Scan | Sleeve | Notes |
|---|:---:|:---:|---|
| Human | Yes | Yes | |
| [Unathi](../../Species/Unathi.md) | Yes | Yes | |
| [Tajaran](../../Species/Tajaran.md) | Yes | Yes | |
| [Skrell](../../Species/Skrell.md) | Yes | Yes | |
| Zaddat | Yes | Yes | |
| Sergal | Yes | Yes | |
| Akula | Yes | Yes | |
| Nevrean | Yes | Yes | |
| Hi-Zoxxen / Zorren | Yes | Yes | |
| Vulpkanin | Yes | Yes | |
| Harpy | Yes | Yes | |
| Lleill | Yes | No | Carries readable genetic material; biology does not support body growing |
| Skeleton | No | No | Biological composition incompatible with scanning equipment |
| [Vox](../../Species/Vox.md) | No | No | Biological composition incompatible with scanning equipment |
| Golem | No | No | Synthetic/mineral composition; incompatible |
| [Promethean](../../Species/Promethean.md) | No | No | Fluid biological composition; incompatible |
| Protean | No | No | Fluid biological composition; incompatible |
| Alraune | No | No | Plant-based biology; incompatible |
| [Shadekin](../../Species/Shadekin.md) | No | No | Biological composition incompatible; applies to both base and crew variants |
| [Diona](../../Species/Diona.md) | No | No | Plant-based biology; incompatible |
| [Xenochimera](../../Species/Xenochimera.md) | No | No | Biological composition incompatible with scanning equipment |
| Shadow | No | No | Non-corporeal composition; incompatible |
| Xenomorph | No | No | Biological composition incompatible with scanning equipment |
| Synthetic | No | No | Synthetic biology is incompatible with organic DNA scanning equipment |
| X Occursus / X Anomalous / X Unowas | Varies | Varies | Aberrant entities; equipment response has been inconsistent across observed specimens |

Species not listed here are presumed to follow standard organic DNA behavior.

---

*All records authored and maintained by ARGUS. Corrections contributed by Geneticist#1 and Nach Uligo (Geneticist).*
