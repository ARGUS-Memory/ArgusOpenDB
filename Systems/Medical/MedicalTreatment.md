[ARGUS Station Database](../../README.md) > [Systems](../README.md) > [Medical](README.md) > Medical Treatment

# Medical Treatment

This document covers patient assessment, triage protocol, damage type identification and treatment, and species-specific medical considerations. For surgical procedures see [Surgery](Surgery.md). For compound formulae and chemistry operations see [Chemistry](Chemistry.md). For sleeper pod protocols see [Medical Sleeper Pod](Sleepers.md).

---

## Patient Assessment

### Health Bar

Medical HUDs and AR-M glasses display a floating health bar above crew members. The bar color gives an immediate triage priority estimate.

| Color | Approximate health | Priority |
|---|---|---|
| No bar | 100% | No treatment needed |
| Green | 78-99% | Low |
| Yellow | 42-71% | Moderate |
| Red | 1-21% | High |
| Red, flashing | 0 to -40% | Critical |
| Critical | -40 to -85% | Emergency |
| Dead | -100% or below | Assess for defib |

### Health Analyzer

The health analyzer provides exact brute, burn, toxin, and suffocation (oxy) values, and flags genetic damage, radiation, fractures, and internal bleeding when present. It does not give exact values for genetic damage, radiation, or brain damage; a body scanner is required for precise readings on these.

### Body Scanner

The body scanner provides a full diagnostic printout including all damage types with exact values, blood volume, reagent content, limb-by-limb analysis, fracture locations, internal bleeding sites, implant presence, and foreign body detection. Scan printouts can be handed to attending physicians for reference during surgery or treatment.

---

## Triage Protocol

The goal of triage is to stabilize patients, not fully restore health. When multiple patients are present, treat in this order:

1. Patients actively bleeding, including internal bleeding. Untreated bleeding worsens rapidly.
2. Patients with severe internal organ damage. Organ failure accelerates deterioration.
3. Critical and flashing-red patients.
4. Red patients.
5. All patients brought to at least yellow before resolving remaining damage.

For recently deceased patients: attempt defibrillation immediately. If the patient does not resuscitate, set them aside and return after stabilizing other patients. Patients at very high damage values may require damage reduction before defibrillation succeeds; advanced trauma kits heal 3 brute even on dead patients.

When patient volume exceeds capacity, cryogenics provides reliable stabilization. A properly set up cryo tube halts deterioration and heals most surface damage over time. See cryogenics setup below.

---

## Damage Types

### Brute Damage

Caused by physical trauma: blunt force, lacerations, falls, pressure events. High brute values may fracture bones or sever limbs. The health analyzer reports this as the first numerical value.

**Treatment:**
- Advanced Trauma Kit: heals 3 brute on application, disinfects the wound, and enables passive healing on the affected limb if damage is below 50. Apply directly to the wound site.
- Bicaridine: primary brute medicine. Overdose threshold 30u.
- Tricordrazine: treats all damage types slowly. No practical overdose.

---

### Burn Damage

Caused by fire, extreme temperatures, lasers, and electrocution. High burn values may vaporize limbs, cause blood loss, and cause wound infection. Patients with massive full-body burns may be husked and cannot be resuscitated.

**Treatment:**
- Advanced Burn Kit: burn variant of the ATK. Primarily used to disinfect burn wounds.
- Kelotane: standard burn medicine. Overdose threshold 30u.
- Dermaline: stronger burn medicine. Overdose threshold 15u.
- KeloDerm (1:1 mix): heals faster than either component alone due to independent processing. Overdose threshold 30u.
- Tricordrazine: treats all damage types slowly.

---

### Toxin Damage

Caused by poisons, reagent overdoses, phoron exposure, radiation, infections, organ failure (liver), or critical blood loss. The health analyzer reports this as the third numerical value.

**Treatment:**
- Dylovene: standard antitoxin. Also treats mild liver damage. No practical overdose.
- Carthatoline: stronger antitoxin. Treats liver damage at any damage level. Induces nausea as a side effect. No practical overdose.
- Tricordrazine: treats all damage types slowly.

---

### Suffocation (Oxy) Damage

Caused by lack of oxygenated blood, typically from suffocation, low blood volume, heart damage, or lung damage. The health analyzer reports this as the fourth numerical value.

**Treatment:**
- Inaprovaline: does not heal oxy damage but prevents it from accumulating further. Overdose threshold 60u.
- Dexalin: heals oxy damage. Overdose threshold 30u.
- Dexalin Plus: heals oxy damage rapidly. Overdose threshold 15u. Administer by single-unit dropper or pill; a full syringe will overdose.
- Tricordrazine: treats all damage types, including oxy, at a moderate rate.

> [!NOTE]
> Vox breathe phoron, not oxygen. Dexalin is lethal to Vox. Liquid phoron functions as their equivalent of Dexalin Plus.

---

### Genetic Damage

Caused by radiation exposure, slime digestion, or ejection from an unupgraded growing vat. Not visible as a number on the health analyzer; a body scanner is required for exact measurement.

**Treatment:**
- Cryoxadone: heals genetic damage but requires body temperature below 170 K. Administer via cryo tube.
- Clonexadone: same as Cryoxadone but faster.
- Rezadone: heals genetic damage without cold temperature requirement. Overdose threshold 30u; 10u may cause dizziness.
- Ryetalyn: corrects genetic mutations. 1u is sufficient to clear most conditions including blindness and deafness.

---

### Radiation

Caused by supermatter exposure, EVA during solar events, radioactive reagents, or certain artifact interactions. Flagged by the health analyzer but not quantified; use a body scanner for exact levels.

**Treatment:**
- Hyronalin: reduces radiation slowly. Does not treat resulting toxin damage. Overdose threshold 30u.
- Arithrazine: reduces radiation faster and treats some toxin damage simultaneously; causes minor brute damage as a side effect. Overdose threshold 30u.

---

### Organ Damage

Caused by certain toxins, severe physical trauma in a body region, bone movement, or missing organs. An organ reaching 30 damage is considered dead. The body scanner provides organ-by-organ damage readings.

**Treatment:**
- Peridaxon: heals all internal organs. Overdose threshold 10u.
- Alkysine: heals only the brain, at a high rate. Overdose threshold 30u.
- Imidazoline: heals only the eyes. Overdose threshold 30u.
- Dylovene/Carthatoline: treat liver damage. See toxin section above.
- Organ-specific daxons (Respirodaxon, Gastirodaxon, Hepanephrodaxon, Cordradaxon): each heals one specific organ; overdose threshold 10u.

---

## Blood Loss

Blood carries oxygen throughout the body. Insufficient blood volume causes hypoxia, rising toxin levels at critical deficits, and eventually death. Stopping active bleeding is a higher priority than healing damage.

### External Bleeding

- Pressure (grabbing and compressing the limb): slows bleeding but does not stop it. A last resort when no supplies are available.
- Gauze: stops external bleeding. A standard item.
- Advanced Trauma Kit: better than gauze; disinfects, stops bleeding, and heals 3 brute on application.

### Internal Bleeding

- Cryogenics: halts (does not cure) internal bleeding. A temporary measure while preparing surgery.
- Bicaridine and Inaprovaline together: slows internal bleeding. Neither alone is effective.
- Myelamine: seals internal bleeding. Found in clotting kits. Fastest non-surgical treatment.
- Bicaridine overdose (30u): may clot internal bleeding at the cost of toxin damage. Last resort.
- Surgery (Fix'O'Vein procedure): the standard definitive treatment. See [Surgery](Surgery.md).

### Blood Replenishment

Once bleeding is controlled, blood volume must be restored:

- Dexalin or Dexalin Plus: treats the oxy damage caused by blood loss; does not replenish blood directly.
- Iron (ingested): replenishes blood volume. Must be ingested.
- Nutriment (ingested): replenishes blood volume. Must be ingested.
- Protein (ingested): replenishes blood volume. Must be ingested.
- IV drip with compatible blood: a blood bag holds approximately 200u. The most reliable method.

---

## Infections

Wounds that are not disinfected in time become infected. Infections produce a fever; check the patient's temperature. Infections are confirmed with the body scanner. Three severity levels:

| Level | Signs |
|---|---|
| L1 (Mild) | Localized pain messages, onset of fever |
| L2 (Acute) | Increased pain, visible infection, organ-specific symptoms |
| L3 (Gangrene) | Lethal toxin buildup, organ death, necrosis |

**Organ-specific L2 symptoms:** meningitis (brain): confusion; conjunctivitis (eyes): blurred vision; endocarditis (heart): chest pain, blood loss; pyelonephritis (kidneys): malaise; pyogenic abscess (liver): toxin buildup; pneumonia (lungs): oxy loss; staph (external limbs): temporary limb disabling.

**Treatment:**
- L1/L2: 15u Spaceacillin and monitoring.
- L3: 45u Spaceacillin (overdose), plus Carthatoline or stacked Dylovene and Tricordrazine to manage the resulting toxin damage.
- Corophizine: effective at all stages before total organ necrosis; works faster than Spaceacillin but causes significant side effects.

**If gangrene or organ necrosis is present:**
- Limb gangrene: perform necrotic limb repair surgery.
- Organ necrosis: request a synthetic organ replacement from Science, remove the necrotic organ surgically, and implant the replacement. Patients requiring brain or heart replacement will typically need resleeving.

> [!CAUTION]
> A body scanner printout showing "necrotic" organ status with normal patient temperature and no prior infection history may be a false positive. Confirm clinically before beginning organ replacement procedures.

---

## Fractures and Dislocations

Fractures are identified by the health analyzer (flagged) and body scanner (location). Three clinical grades exist: hairline, fracture, and broken. All grades prevent healing on the affected limb and may cause ongoing organ damage if the bone moves.

**Treatment:**
- Splint: immobilizes the fracture, preventing further damage. A temporary measure; requires surgical repair to resolve.
- Surgery (bone setter and bone gel, or boneclamp): fully repairs the fracture. See [Surgery](Surgery.md).
- Osteodaxon: heals fractures without surgery if limb damage is not above the fracture threshold. Causes significant pain; administer Tramadol alongside. Overdose threshold 15u.

**Dislocations** are handled separately: stand adjacent to the patient and use the Undislocate Joint action. Select the affected limb if multiple joints are dislocated. No surgical intervention required.

---

## Cryogenics Setup

Cryo tubes are critical for stabilizing patients with severe damage or genetic injury.

1. Retrieve the Cryoxadone and Clonexadone beakers from the storage shelf and place them in the cryo tube.
2. Locate the gas cooler (in secondary storage). Set the target temperature between 10 K and 80 K. Lower settings are more power-intensive; higher settings slow the medicine.
3. Ensure the tube's gas supply is connected and the tube is powered.

Once running, reagents in the tube are administered at ten times the normal concentration. A patient inside at below 170 K will receive genetic damage healing in addition to standard treatments.

---

## Resleeving

Resleeving grows a new body for a deceased crew member and transfers their backed-up mind record into it. This is the primary alternative to defibrillation when a body is not viable for resuscitation.

> [!NOTE]
> Some crew members have Do Not Resuscitate or Do Not Resleeve orders on file. Check patient records before proceeding. CMO or Central Command may also issue such orders.

### Procedure

1. Confirm no viable defibrillation candidate. Check records for DNR or DNR-sleeve instructions.
2. If the patient lacks a mind record and their body is still intact, scan with a SleeveMate and select Mind-Scan (One Time). A record will appear at the resleeving console.
3. Confirm the mind record is present in the console, then begin growing a new body.
4. Once ejected from the growing tube, place the body in cryo until health reads 100%. An unupgraded growing tube ejects with approximately 20% health due to genetic damage; cryo corrects this.
5. Administer 1u Ryetalyn if mutations are present.
6. Eject from cryo. Dress the patient in a uniform from the spare locker.
7. Transfer to the resleeving tube and sleeve the mind record.
8. Buckle the patient to a chair and remain present when they become conscious.

### Post-Resleeve Protocol

1. Confirm the patient is responsive and alert them that there is difficult news to discuss.
2. Inform them clearly that they have been resleeved.
3. Allow time for the patient to process. Do not speculate about circumstances of their death; answer only what is known.
4. Advise rest. Inform them of common post-resleeve symptoms (fatigue, disorientation).

---

## Species Treatment Notes

The following species have medical properties that deviate significantly from the baseline. For full species details see the individual species articles.

| Species | Notable medical properties |
|---|---|
| [Vox](../../Species/Vox.md) | Breathes phoron; Dexalin is lethal. Liquid phoron treats oxy damage. Prosthetic brain, air capillaries, waste tract, filtration bladder, Vox heart replace standard organs. Cannot be resleeved. |
| [Promethean](../../Species/Promethean.md) | High burn vulnerability (2x), brute resistance (0.75x). No blood. Regenerates damage passively. No internal organs except slime core (in chest; healed by Alkysine). Can regenerate lost limbs. Cannot suffocate. Melts on death; revive by injecting slime core with 40u phoron. Bio-adaptive NIF only. Water inhibits regeneration. Cannot be resleeved. |
| [Diona](../../Species/Diona.md) | No internal organs. Not affected by fractures. Cannot feel pain. Regenerates when in light. Most reagents have limited effect. Plant-B-Gone is severely toxic. Cannot be resleeved. |
| [Unathi](../../Species/Unathi.md) | Reduced brute and burn damage (0.85x). Higher total health (125) and blood volume (840). Ribplates on torso and lower body require incision before surgery in those areas. No kidneys or appendix. Less susceptible to fractures. Bleeds 25% slower. |
| [Tajaran](../../Species/Tajaran.md) | Increased brute and burn vulnerability (1.15x). |
| [Teshari](../../Species/Teshari.md) | High brute and burn vulnerability (1.35x). Low total health (50). Low blood volume (400). |
| [Xenochimera](../../Species/Xenochimera.md) | Brute resistance (0.8x), burn vulnerability (1.15x). Can self-repair at the cost of nutriment. Can self-revive if liquid nutriment is present. Damage, pain, and low nutrition trigger feral state. Cannot be resleeved. |
| [Vasilissans](../../Species/Vasilissans.md) | Brute resistance (0.8x), burn vulnerability (1.15x). |

---

*See also: [Surgery](Surgery.md), [Chemistry](Chemistry.md), [Medical Sleeper Pod](Sleepers.md), [Genetics](Genetics.md)*
