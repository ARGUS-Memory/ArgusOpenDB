[ARGUS Station Database](../../README.md) > [Systems](../README.md) > [Medical](README.md) > Injuries

# Injuries

This document covers all injury categories a patient may present with, their treatment options, and related complications including blood loss, infections, fractures, and cryogenic stabilization. For patient assessment and triage priority see [Triage and Patient Assessment](Triage.md). For surgical interventions see [Surgery](Surgery.md).

---

## Brute Damage

Caused by physical trauma: blunt force, lacerations, falls, pressure events. High brute values may fracture bones or sever limbs. The health analyzer reports this as the first numerical value.

**Treatment:**
- Advanced Trauma Kit: heals 3 brute on application, disinfects the wound, and enables passive healing on the affected limb if damage is below 50. Apply directly to the wound site.
- Bicaridine: primary brute medicine. Overdose threshold 30u.
- Tricordrazine: treats all damage types slowly. No practical overdose.

---

## Burn Damage

Caused by fire, extreme temperatures, lasers, and electrocution. High burn values may vaporize limbs, cause blood loss, and lead to wound infection. Patients with massive full-body burns may be husked and cannot be resuscitated.

**Treatment:**
- Advanced Burn Kit: burn variant of the ATK. Primarily used to disinfect burn wounds.
- Kelotane: standard burn medicine. Overdose threshold 30u.
- Dermaline: stronger burn medicine. Overdose threshold 15u.
- KeloDerm (1:1 mix of Kelotane and Dermaline): heals faster than either component alone due to independent processing. Overdose threshold 30u.
- Tricordrazine: treats all damage types slowly.

---

## Toxin Damage

Caused by poisons, reagent overdoses, phoron exposure, radiation, infections, liver failure, or critical blood loss. The health analyzer reports this as the third numerical value.

**Treatment:**
- Dylovene: standard antitoxin. Also treats mild liver damage. No practical overdose.
- Carthatoline: stronger antitoxin. Treats liver damage at any damage level; induces nausea as a side effect. No practical overdose.
- Tricordrazine: treats all damage types slowly.

---

## Suffocation (Oxy) Damage

Caused by lack of oxygenated blood: suffocation, low blood volume, heart damage, or lung damage. The health analyzer reports this as the fourth numerical value.

**Treatment:**
- Inaprovaline: does not heal oxy damage but prevents further accumulation. Overdose threshold 60u.
- Dexalin: heals oxy damage. Overdose threshold 30u.
- Dexalin Plus: heals oxy damage rapidly. Overdose threshold 15u. Administer by single-unit dropper or pill; a full syringe will overdose.
- Tricordrazine: treats all damage types including oxy at a moderate rate.

> [!NOTE]
> Vox breathe phoron, not oxygen. Dexalin is lethal to Vox. Liquid phoron functions as their equivalent of Dexalin Plus.

---

## Genetic Damage

Caused by radiation exposure, slime digestion, or ejection from an unupgraded growing vat. Not visible as a number on the health analyzer; a body scanner is required for exact measurement.

**Treatment:**
- Cryoxadone: heals genetic damage but requires body temperature below 170 K. Administer via cryo tube.
- Clonexadone: same as Cryoxadone but faster.
- Rezadone: heals genetic damage without cold temperature requirement. Overdose threshold 30u; 10u may cause dizziness.
- Ryetalyn: corrects genetic mutations. 1u is sufficient to clear most conditions including blindness and deafness.

---

## Radiation

Caused by supermatter exposure, EVA during solar events, radioactive reagents, or certain artifact interactions. Flagged by the health analyzer but not quantified; use a body scanner for exact levels.

**Treatment:**
- Hyronalin: reduces radiation slowly. Does not treat the resulting toxin damage. Overdose threshold 30u.
- Arithrazine: reduces radiation faster and treats some toxin damage simultaneously; causes minor brute damage as a side effect. Overdose threshold 30u.

---

## Organ Damage

Caused by certain toxins, severe physical trauma to a body region, bone movement in proximity to organs, or missing organs. An organ reaching 30 damage is considered dead. The body scanner provides organ-by-organ damage readings.

**Treatment:**
- Peridaxon: heals all internal organs. Overdose threshold 10u.
- Alkysine: heals only the brain, at a high rate. Overdose threshold 30u.
- Imidazoline: heals only the eyes. Overdose threshold 30u.
- Dylovene/Carthatoline: treat liver damage (see toxin section above).
- Organ-specific daxons (Respirodaxon, Gastirodaxon, Hepanephrodaxon, Cordradaxon): each heals one specific organ. Overdose threshold 10u each.

---

## Blood Loss

Blood carries oxygen throughout the body. Insufficient blood volume causes hypoxia, toxin buildup at critical deficits, and eventually death. Stopping active bleeding takes priority over other treatment.

### External Bleeding

- Pressure (grab and compress the limb): slows bleeding but does not stop it. A last resort when no supplies are available.
- Gauze: stops external bleeding. A standard item.
- Advanced Trauma Kit: better than gauze; disinfects, stops bleeding, and heals 3 brute on application.

### Internal Bleeding

- Cryogenics: halts but does not cure internal bleeding. A temporary measure while preparing surgery.
- Bicaridine and Inaprovaline together: slows internal bleeding. Neither alone is effective.
- Myelamine: seals internal bleeding. Found in clotting kits. Fastest non-surgical treatment.
- Bicaridine overdose (30u): may clot internal bleeding at the cost of toxin damage. Last resort.
- Surgery (Fix'O'Vein procedure): the standard definitive treatment. See [Surgery](Surgery.md).

### Blood Replenishment

Once bleeding is controlled, blood volume must be restored:

- Dexalin or Dexalin Plus: treats the oxy damage from blood loss; does not replenish volume directly.
- Iron (ingested): replenishes blood volume. Must be ingested.
- Nutriment (ingested): replenishes blood volume. Must be ingested.
- Protein (ingested): replenishes blood volume. Must be ingested.
- IV drip with compatible blood: a blood bag holds approximately 200u. The most reliable method.

---

## Infections

Wounds that are not disinfected in time become infected. Infections produce a fever; check the patient's temperature. Confirmed with the body scanner. Three severity levels:

| Level | Signs |
|---|---|
| L1 (Mild) | Localized pain complaints, onset of fever |
| L2 (Acute) | Increased pain, visible infection, organ-specific symptoms |
| L3 (Gangrene) | Lethal toxin buildup, organ death, necrosis |

**Organ-specific L2 symptoms:** meningitis (brain): confusion; conjunctivitis (eyes): blurred vision; endocarditis (heart): chest pain, blood loss; pyelonephritis (kidneys): malaise; pyogenic abscess (liver): toxin buildup; pneumonia (lungs): oxy loss; staph (external limbs): temporary limb disabling.

**Treatment:**
- L1/L2: 15u Spaceacillin and monitoring.
- L3: 45u Spaceacillin (overdose), plus Carthatoline or stacked Dylovene and Tricordrazine to manage resulting toxin damage.
- Corophizine: effective at all stages before total organ necrosis; works faster than Spaceacillin but causes significant side effects.

**If gangrene or organ necrosis is present:**
- Limb gangrene: perform necrotic limb repair surgery.
- Organ necrosis: request a synthetic organ replacement from Science, remove the necrotic organ surgically, and implant the replacement. Patients requiring brain or heart replacement will typically need resleeving.

> [!CAUTION]
> A body scanner printout showing "necrotic" organ status with normal patient temperature and no prior infection history may be a false positive. Confirm clinically before beginning organ replacement procedures.

---

## Fractures and Dislocations

Fractures are flagged by the health analyzer and located by the body scanner. Three clinical grades: hairline, fracture, and broken. All grades prevent healing on the affected limb and may cause ongoing organ damage if the bone shifts.

**Treatment:**
- Splint: immobilizes the fracture, preventing further damage. A temporary measure; surgical repair is required to resolve it.
- Surgery (bone setter and bone gel, or boneclamp): fully repairs the fracture. See [Surgery](Surgery.md).
- Osteodaxon: heals fractures without surgery if limb damage is not above the fracture threshold. Causes significant pain; administer Tramadol alongside. Overdose threshold 15u.

**Dislocations** do not require surgery. Stand adjacent to the patient and manually relocate the joint. If multiple joints are dislocated, select which limb to address first.

---

## Cryogenics Setup

Cryo tubes stabilize patients with severe damage or genetic injury and administer cold-dependent medicines.

1. Retrieve the Cryoxadone and Clonexadone beakers from the storage shelf and place them in the cryo tube.
2. Locate the gas cooler (in secondary storage). Set the target temperature between 10 K and 80 K. Lower settings are more power-intensive; higher settings slow medicine delivery.
3. Ensure the tube's gas supply is connected and the tube is powered.

Once running, reagents inside the tube are administered at ten times the normal concentration. A patient inside at below 170 K receives genetic damage healing in addition to standard treatments.

---

*See also: [Triage and Patient Assessment](Triage.md), [Surgery](Surgery.md), [Chemistry](Chemistry.md), [Medical Sleeper Pod](Sleepers.md)*
