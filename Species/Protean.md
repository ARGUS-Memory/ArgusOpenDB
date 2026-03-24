[ARGUS Station Database](../README.md) > [Species](README.md) > Protean

# Protean

<img src="../assets/raptor_idle_south.png" width="96" align="right">

Nanoswarm-based synthetics whose bodies consist of cohesive masses of nanomachines capable of shapeshifting and self-regeneration, proteans represent an advanced development in modular synthetic construction and are rare, tightly regulated, and frequently under institutional scrutiny due to the instability of their technology base.

---

## Quick Reference

| | |
|---|---|
| [Physical Components](#physical-components) | Core, Orchestrator, Refactory, Nanoswarm |
| [Mind-Origin Classification](#mind-origin-classification) | PCX, PDN, PAS, PXS types |
| [Regulation and Assessment](#regulation-and-assessment) | Stability evaluation, capability testing, PAN permit |
| [Capabilities and Limitations](#capabilities-and-limitations) | Shapeshifting, EMP vulnerability, no remote interfacing |
| [Interspecies Relations](#interspecies-relations) | General galactic standing, NT research context |
| [Medical and Operational Notes](#medical-and-operational-notes) | EMP vulnerability, regeneration time, cloning incompatibility |

---

## Physical Components

A protean body consists of four functional components: the Core, the Orchestrator, the Refactory, and the Nanoswarm.

### Core

The Core is the intelligence housing. It stores the mind that controls the protean body, analogous to the positronic brain of a standard synthetic. Cores vary in size and composition but are almost universally surrounded by an electromagnetically conductive alloy to provide strong signal pathways to the Orchestrator.

Transferring a mind into a nanoswarm body is expensive and high-risk. Mind-body compatibility with the specific swarm-orchestrator pairing must be developed through experience. The process is typically contractually binding; the transferring party is generally unable to reverse the conversion without corporate or governmental assistance, and attempting reversal without such assistance typically results in fatal incompatibility.

### Orchestrator

The Orchestrator is the computational intermediary between the Core's high-level commands and the individual components of the swarm. No known intelligence can manage each nanite directly; the Orchestrator receives commands such as "form an appendage" or "reshape this section" and executes them by controlling each subcluster in parallel through specialized accelerator hardware. Without an Orchestrator, a protean is limited to slow deliberate motion or blob-form movement.

Adapting to the specific architecture of a given swarm-Orchestrator combination is considered one of the most difficult aspects of becoming a protean. Mass production of proteans has been halted repeatedly due to this adaptation difficulty.

### Refactory

The Refactory is the protean's production engine. It contains billions of molecular constructors running continuously to produce a stream of replacement nanites. It is typically the most energy-consuming component and also the most physically fragile. The Refactory requires physical ingestion of material for synthesis and is sensitive to shock and stress. Some modern Refactories contain limited self-repair capability; older designs can be damaged by falls from standing height without swarm support. A protean without a functional Refactory cannot regenerate and will progressively shed nanites until the swarm fails unless external nanite chambers are found and reprogrammed.

### Nanoswarm

The Nanoswarm is the majority of the protean body. Modern swarms use weak electromagnetic coupling at the molecular scale for alignment and friction, enabling efficient shapeshifting and fluid movement compared to earlier physically-hooked designs.

The electromagnetic reliance that enables swarm flexibility also creates a critical vulnerability. Military-grade EMP is capable of halting a protean in motion or causing outright destruction. The swarm's design amplifies electromagnetic pulses rather than dissipating them, the direct inverse of conventional conductive metal chassis behavior.

---

## Mind-Origin Classification

**PCX (Contemporary Experimental):** Positronic intelligences. The most common protean type. Most are prototypes financed by megacorporations researching nanoswarm feasibility for labor applications.

**PDN (Drone-Intelligence):** Rare. Drones are subject to strict operational standards that limit eligibility for nanoswarm conversion. PDN proteans are typically used to regulate swarm integrity pending assignment to a full intelligence. PDNs are lawed; complete autonomy is theoretically possible through unlawing but requires corporate assistance due to operating system complexity, and would result in reclassification as PCX.

**PAS (Assimilated-type):** Very rare. Created from a copy or direct transfer of an organic mind.

**PXS (Xenosynthetic):** Intelligences that do not fit the other three categories. Often assigned to proteans produced by extinct or ancient cultures, or intelligences unidentifiable by current classification standards.

---

## Regulation and Assessment

Proteans in most jurisdictions undergo periodic evaluation including standard synthetic psychological assessment and human-adapted psychological examination. Stability testing for swarm consistency and control is a separate requirement. Advanced tests examine shapeshifting accuracy, mimicry, and confirm that Orchestrator and Refactory capabilities are not bypassed in unauthorized ways, such as forming integrated weapons or deconstructing complex external structures.

A Protean Access Network (PAN) permit is required for most protean operations in civilized space.

---

## Capabilities and Limitations

Proteans can shapeshift, regenerate from damage, and alter their appearance within the limits of their swarm composition. They cannot interface remotely with external computers or machinery; operating system incompatibility prevents any form of remote computation or machine control. Proteans interact with all external systems through manual physical interfaces, the same as organic crew.

Most swarms consist of a single nanite type; even advanced proteans cannot utilize more than a few types simultaneously. Proteans cannot form complex machinery internally despite the shapeshifting capability.

---

## Interspecies Relations

Proteans are rare across known space and carry an uncanny or dangerous reputation in many jurisdictions. Their presence is uncommon in core systems. Reactions range from scientific interest to institutional caution. Being uncommon and under active development, protean social standing varies significantly by polity.

---

## Medical and Operational Notes

**EMP vulnerability:** Proteans take double damage from electromagnetic pulses, which also cause blindness and deafness on impact. EMP-based security measures in areas with protean crew are inadvisable. Avoid EMP grenades or pulse weapons against protean crew even at low settings.

**Regeneration:** Passive healing consumes stored steel from the Refactory continuously. Full structural reconstruction requires adequate steel reserves; a complete rebuild costs substantial steel and takes approximately 40 seconds. Proteans that exhaust their steel supply cannot passively regenerate.

**Temperature:** Proteans are not affected by cold environments. Heat, however, causes accelerated harm beginning at lower thresholds than most humanoids. Thermal and energy damage is significantly elevated relative to organic crew.

**Vacuum and pressure:** Protean swarm structure is not disrupted by vacuum or low-pressure environments. Standard EVA hazard protocols do not apply to proteans.

**Refactory protection:** Physical shock damage to the Refactory is possible even in normal station environments. Falls, impacts, and high-energy incidents should be followed by Refactory integrity assessment.

**Cloning incompatibility:** Protean bodies cannot be produced by body-printing technology.

**Injury treatment:** Standard medical supplies have no effect on protean physiology. Bandages, bruise packs, burn kits, and similar treatments do not function on nanoswarm tissue. The only effective damage treatment is steel: the Refactory converts stored steel into replacement nanites continuously, and active limb reconstruction is performed by the protean directly. Medical staff responding to a protean injury should ensure the patient has access to steel and, in severe cases, facilitate transport to the Protean Reconstitutor. Toxin and viral treatments are similarly without effect.

**Nutrition and materials:** On this station, proteans consume steel for Refactory synthesis. Ensure adequate steel access for extended operations; a protean without steel cannot regenerate damage.

---

<details>
<summary><strong>Mechanics Reference (OOC)</strong></summary>

> **Out-of-character notice:** This section describes in-game mechanical properties of the Protean species as implemented on CHOMPStation. It is intended as a player reference and should not inform in-character knowledge.

### Damage Modifiers

| Damage Type | Modifier | Notes |
|---|---|---|
| Brute | 0.8x | Reduced physical damage |
| Burn | 1.5x | Elevated thermal and energy damage |
| Oxygen | Immune | No oxygen requirement (`oxy_mod = 0`) |
| Cold | Immune | Cold damage thresholds set to minimum possible |
| EMP | 2.0x | Siemens coefficient 2; also causes blindness and deafness |
| Radiation | Standard | No special modifier |
| Toxin | Immune | No poison type; virus-immune flag |
| Vacuum | Immune | Low-pressure hazard disabled (`hazard_low_pressure = -1`) |

Proteans cannot enter critical condition (`crit_mod = 4`). They have passive dark vision (range 10).

### Inherent Abilities

| Ability | Function |
|---|---|
| **Toggle Blobform** | Switch between humanoid and amorphous blob form. Cannot activate while stunned or paralyzed. In blob form, passive steel consumption provides slow healing. |
| **Ref - Single Limb** | Rebuild or replace one missing or damaged limb. Costs 2,000 steel per limb. |
| **Total Reassembly** | Two options: Rebuild repairs all limbs and damage over 40 seconds, costs 10,000 steel. Reassemble restores saved appearance at no cost. |
| **Ref - Store Metals** | Consume a held stack of steel and transfer it to Refactory storage. |
| **Copy Form** | While aggressively grabbing a consenting target, copy their species appearance. Does not copy their name. |
| **Change Species Fit** | Adjust body proportions to fit suits designed for a different species. |
| **Modify Form - Hardsuit** | Retract mass into the protean RIG control module at will. |
| **Latch / Unlatch Host** | Forcibly latch onto or detach from a target host. |
| **Assimilate Host** | Devour a currently latched host. |
| **Toggle Blobform (blob)** | Return to humanoid form from blob. |
| **Hide Self** | Disperse blob mass into a thin veil; conceals presence and functions as a prey trap. |
| **Change Volume** | Adjust body size. |
| Shapeshifter selectors | Hair, eye color, skin color, gender, wings, tail, ears, secondary ears -- all adjustable in humanoid form. |

### Steel Economy

On CHOMPStation only steel is accepted by the Refactory (`PROTEAN_EDIBLE_MATERIALS = list(MAT_STEEL)`). Other materials present in the base code (uranium, gold, silver, metalhydrogen) and their associated passive bonuses are disabled on this server.

| Operation | Steel Cost |
|---|---|
| Single limb regrowth | 2,000 (one sheet) |
| Total Reassembly (full rebuild) | 10,000 (five sheets) |
| Total Reassembly (appearance only) | 0 |
| Passive healing per tick (blob form) | 100 (1/20 sheet) |

### Death Behavior

On death, a protean retreats into its hardsuit RIG control module. The protean is locked to the module and cannot act until revived. Revival requires the **Protean Reconstitutor** machine in the Science department, which requires the protean's positronic brain, Orchestrator, Refactory, and a supply of nanopaste to reconstitute a new body.

### Species Notes

Proteans are a **whitelisted species** and require approval before joining as one. Native language is Extended Algorithmic Language (EAL). Proteans move slower when carrying items (`item_slowdown_mod = 1.5`) and spawn with a P.A.N. card (Permit for Advanced Nanotechnology), 5 steel sheets, and a NIF implant.

</details>
