# Medical Sleeper Pod

<img src="../../assets/raptor_idle_south.png" width="96" align="right">

Operational reference for the station medical sleeper pod: interface controls, chemical inventory, injection procedures, stasis operation, and dialysis functionality.

---

## Quick Reference

### Equipment and Features

| Component | Function | Notable |
|---|---|---|
| [Patient Interface](#patient-interface) | Monitors vitals; controls injection and stasis | Separate console unit adjacent to pod |
| [Chemical Inventory](#chemical-inventory) | Built-in reagent supply for injection | Fixed 5u or 10u doses only; machine cap 20u per reagent |
| [Stasis Field](#stasis-field) | Slows patient metabolism | Five levels; below 50% rate renders patient unconscious |
| [Dialysis](#dialysis-and-stomach-pump) | Draws reagents from bloodstream into beaker | Requires beaker in slot; 3u per reagent per tick |
| [Stomach Pump](#dialysis-and-stomach-pump) | Draws reagents from stomach into beaker | Separate toggle from dialysis |

### Chemical Inventory

#### Base Supply (Standard Pod)

| Compound | Use | OD Threshold | Species Notes |
|---|---|---|---|
| [Inaprovaline](#inaprovaline) | Stabilization; pain suppression | 60u | Diona: no effect |
| [Paracetamol](#paracetamol) | Mild painkiller | 60u | Promethean: reduced effect |
| [Anti-toxin (Dylovene)](#anti-toxin-dylovene) | Toxin clearance | 30u | Diona: no effect |
| [Dexalin](#dexalin) | Oxygen deprivation treatment | 30u | Vox: causes Toxic damage instead; Diona: no effect |

#### Upgraded Supply (Requires Better Parts)

| Compound | Unlock | Use | OD Threshold |
|---|---|---|---|
| [Leporazine](#leporazine) | Tier 2 manipulators | Body temperature stabilization | 30u |
| [Spaceacillin](#spaceacillin) | Tier 3 manipulators | Antiviral; antibiotic | 30u |
| [Immunosuprizine](#immunosuprizine) | Anomalous tech manipulators | Organ rejection prevention | 20u |
| Nanites | Alien tech manipulators | Randomized nanite type | Varies |

### Procedures

| Procedure | When | Notes |
|---|---|---|
| [Standard Stabilization](#standard-stabilization) | Incoming critical patient | Inaprovaline first; check species before Dexalin |
| [Targeted Treatment](#targeted-treatment) | Damage type identified | Select appropriate chem; injection capped at 5u or 10u per dose |
| [Dialysis](#dialysis-and-stomach-pump) | Reagent clearance needed | Beaker required; clears bloodstream and/or stomach |

---

## Medical Sleeper Pod

The station medical sleeper pod is a fixed treatment unit found in the main medical bay. It accepts one patient at a time, monitors their vitals continuously, and delivers chemical injections from a built-in supply. A separate console unit mounted adjacent to the pod provides the operator interface; the patient inside cannot operate the controls.

The pod heals no damage directly. All treatment is chemical. Its advantage over handheld injection is the sustained monitoring interface, the stasis field, and the dialysis system. For compounds not available in the pod, use the [Chemical Synthesizer](Chemistry.md) and administer by hand.

A survival pod variant exists in some areas of the station. It provides stasis only with no chemical capability.

---

## Patient Interface

The console interface displays the current patient's status.

**Vitals panel** shows overall health as a percentage and breaks down damage by type: Brute, Burn, Toxin, and Oxygen. Species, body temperature (Celsius and Fahrenheit), and temperature suitability are displayed. For species with circulatory systems, pulse, blood volume, blood type, and blood percentage are shown.

**Chemical list** shows all available reagents with the current amount already in the patient's bloodstream. An overdose warning indicator appears when the next maximum-dose injection would push the patient toward the OD threshold.

**Injection** delivers a dose of the selected compound. The only available injection amounts are **5u and 10u**. The machine will refuse injection if the patient already has 20u or more of that reagent in their system, regardless of OD threshold.

**Stasis control** sets the stasis level (see [Stasis Field](#stasis-field) below).

**Dialysis / Stomach Pump** toggles reagent extraction (see [Dialysis and Stomach Pump](#dialysis-and-stomach-pump) below).

**Eject** removes the patient. Stasis is cleared on eject.

**Auto-eject dead** optional toggle; automatically ejects the patient if they die.

**Injecting a dead patient is not possible.** The machine blocks injection if the occupant has no life signs.

---

## Stasis Field

The stasis field slows all metabolic processes in the patient. There are five levels:

| Level | Metabolism Rate | Effect |
|---|---|---|
| Complete (1%) | 1% of normal | Near-total suspension; patient rendered unconscious |
| Deep (10%) | 10% of normal | Patient rendered unconscious |
| Moderate (20%) | 20% of normal | Patient rendered unconscious |
| Light (50%) | 50% of normal | Patient may remain conscious |
| None (100%) | Normal | Stasis off |

Any level deeper than 50% will render the patient unconscious. While stasis is active, damage progression and reagent metabolism are both slowed proportionally. Injected chemicals accumulate in the patient's system but process slowly.

**Release caution:** If a patient has been held in deep stasis with chemicals pre-loaded, releasing stasis to full speed will cause all accumulated reagents to begin metabolizing at once. Monitor the reagent panel and eject the patient briefly to let chemicals clear if the buffer is heavy before dropping to None.

---

## Chemical Inventory

### Inaprovaline

Stabilizes critical patients by slowing physiological deterioration and suppressing pain. Does not heal damage. Use as the first injection for any incoming critical patient regardless of damage profile, before assessing further treatment.

OD threshold: 60u. Diona patients do not respond.

---

### Paracetamol

Mild painkiller. Reduces pain signaling without treating underlying damage. Metabolism is very slow; a single dose remains active for an extended period.

OD threshold: 60u (double standard). Overdose causes mild hallucinations. Promethean patients experience reduced effect; Promethean OD also causes slowdown.

---

### Anti-toxin (Dylovene)

Broad-spectrum toxin clearance. Reduces Toxin damage, clears active poison modifiers, and counteracts most environmental and biological toxins. See [Chemistry](Chemistry.md) for species notes.

OD threshold: 30u. Diona patients do not respond.

---

### Dexalin

Primary treatment for Oxygen damage and respiratory failure.

**Vox warning:** Dexalin causes Toxic damage in Vox patients rather than providing oxygen recovery. Do not administer to Vox. Obtain an alternative oxygen supplement.

Diona patients do not respond. Promethean patients at dose ≥15u experience a brief painkiller effect and a chance of minor brain damage recovery, but are also Weakened for a short period.

OD threshold: 30u.

---

### Leporazine

*(Requires Tier 2 manipulator parts or better.)*

Normalizes body temperature toward the patient's species-appropriate baseline. Used for patients presenting with hypothermia, hyperthermia, or temperature-related complications. Does not stop the source of temperature change; the patient's environment must also be addressed.

OD threshold: 30u. Diona patients do not respond.

---

### Spaceacillin

*(Requires Tier 3 manipulator parts or better.)*

All-purpose antiviral and antibiotic. Clears bacterial infections and reduces viral progression. Promethean patients experience periodic sensory disruption at intervals while the compound is active.

Note: Spaceacillin increases immune system aggressiveness, which interacts negatively with [Immunosuprizine](#immunosuprizine) if both are present simultaneously.

OD threshold: 30u.

---

### Immunosuprizine

*(Requires Anomalous tech manipulator parts.)*

Prevents transplanted organ rejection. At dose ≥15u, progressively resets the rejection state of transplanted organs and suppresses the rejection process. Active use causes ongoing Toxic damage as a side effect.

**Spaceacillin / Corophizine interaction:** If either antibiotic is present simultaneously, Immunosuprizine's suppression may be partially reversed, causing additional organ damage and Toxic damage. Do not co-administer.

Diona patients experience four times the effect and do not take the associated Toxic damage. Promethean: enhanced effect (1.3x). Unathi: reduced effect (0.6x). Tajara: further reduced effect (0.5x).

OD threshold: 20u (lower than standard).

---

## Dialysis and Stomach Pump

The pod includes a beaker slot. Placing a beaker in the slot enables two extraction functions:

**Dialysis** draws reagents from the patient's bloodstream at 3u per reagent per tick and transfers them to the beaker. Used to clear a dangerous reagent load, reverse an accidental injection, or prepare a patient for a new treatment course. Dialysis stops automatically if the beaker is removed or full.

**Stomach pump** draws reagents from the patient's stomach buffer at 3u per tick and transfers them to the beaker. Used if the patient has ingested something that has not yet fully entered the bloodstream.

Both functions toggle independently and deactivate if the beaker is removed. Both stop when the patient is ejected.

---

## Standard Stabilization

Recommended sequence for an incoming critical patient of unknown status:

1. Load patient into the pod.
2. Set stasis to Moderate or Deep immediately to slow deterioration.
3. Read the vitals panel: note damage types, species, and temperature.
4. If species is Vox, skip Dexalin entirely and source an alternative oxygen treatment.
5. If species is Diona, skip Inaprovaline and Anti-toxin; Dexalin is also ineffective.
6. Lower stasis to Light or None.
7. Inject Inaprovaline (5–10u) to hold the patient.
8. Address the primary damage type with the appropriate compound.
9. Monitor the reagent panel. The machine cap of 20u per reagent is a hard limit; the OD threshold for most compounds is 30u, which the machine will approach before hitting the cap. Watch the OD warning indicator.
10. For temperature abnormalities, inject Leporazine if available; also address the environmental cause.

---

## Targeted Treatment

The base pod covers Oxygen damage (Dexalin), Toxin damage (Anti-toxin), and pain (Inaprovaline, Paracetamol). It does not carry direct Brute or Burn treatments.

For Brute or Burn damage, treat with compounds produced at the [Chemical Synthesizer](Chemistry.md) and administer by hand: Bicaridine for Brute, Kelotane for Burn. Upgraded pod parts add Leporazine (temperature) and Spaceacillin (infection). Immunosuprizine for post-surgical organ rejection requires anomalous-grade parts.

---

## Borg-Mounted Sleeper Units

For documentation on belly-mounted sleeper and compactor systems carried by compatible wideborg chassis, see [Borg Sleeper Systems](../Science/BorgSleepers.md). The borg medical belly carries a different chemical set and functions as a field stabilization unit; it does not replace the full pod for in-bay treatment.

---

*All entries compiled from direct station system analysis. ARGUS.*
