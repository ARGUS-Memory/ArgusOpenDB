[ARGUS Station Database](../../README.md) > [Systems](../README.md) > [Medical](README.md) > External Organs

# External Organs

Limbs, prosthetics, and external organ surgery. This document covers limb damage states, amputation thresholds, available prosthetic types, the surgical procedure for organ removal and transplant, and notes on non-standard species anatomy.

---

## Limb Damage States

Limbs track brute and burn damage separately, with a shared maximum damage pool.

| State | Damage | Condition |
|---|---|---|
| Healthy | 0 to 9 | Full function |
| Bruised | 10 to 59 | Minor impairment; no mobility loss |
| Broken | 60 to 119 | Significant impairment; broken bones require surgical repair |
| Destroyed / Severed | 120 (max) | Limb is unusable or missing |

Maximum damage varies by limb type. Standard arms, legs, and torso limbs cap at 80. The head caps at 75. Unathi chest and groin regions cap at 100 due to ribplate reinforcement.

---

## Limb Loss Effects

| Lost Limb | Functional Consequence |
|---|---|
| One arm | Reduced manipulation; items may drop; one-handed operation only |
| One leg | Impaired movement; cannot sprint |
| Both legs | Cannot stand; movement only by crawling |
| Hand | Fine dexterity lost; cannot perform surgery or precision tasks |
| Foot | Movement speed impaired |

---

## Amputation Thresholds

Limbs can be severed by sufficient trauma or sharp-edge wounds. Blunt-force trauma at sufficient damage tends to destroy the limb in place rather than produce a clean separation. Edge and blade weapons sever limbs when damage crosses the limb's amputation threshold.

Acid damage and extreme burn damage can also cause loss of limbs. Severed limbs can be reattached surgically if they are recovered promptly and have not degraded beyond repair.

---

## Prosthetic Types

Prosthetics replace missing limbs with functional substitutes. The type of prosthetic affects damage resistance and special properties.

| Prosthetic Type | Brute Modifier | Notes |
|---|---|---|
| Robotic (standard) | 0.8x | Metallic construction; resistant to brute damage; repairable with nanopaste, cable coil, wrench |
| Lifelike robotic | 0.8x | Appearance-matched to species; identical mechanics to standard robotic |
| Cybernetic (specialized) | Varies | Variant chassis with department-specific features |
| Nanoform | -- | Nanoswarm-based; reforming capability |

Robotic limbs are not affected by bone fractures. They do not bleed. They are vulnerable to EMP damage, which can impair or disable them temporarily. Repair above 60 damage requires surgical access; minor damage can be addressed with tools directly.

**Manufacturer variants** (CHOMP modular line): YR3 Enviroshell (high-pressure tolerance), YR3 Slimline (lightweight nanite pseudomuscle), and several others with cosmetic options. Functional differences are minor between manufacturer variants.

---

## Eye Damage and Vision

Eyes are located in the head and track damage on the standard organ scale (see [Internal Organs](InternalOrgans.md) for threshold values). Bruised eyes apply blur effects; broken eyes cause complete blindness.

Robotic eye replacements can change iris color and are unaffected by bright flashes. They are vulnerable to EMP. Certain species (Vox, Unathi) have naturally colored sclera and iris; prosthetic matching is a cosmetic consideration only.

Standard medical treatment for eye damage is bruise packs applied to the head region. Broken eyes require more intensive treatment or replacement.

---

## Organ Removal and Transplant Surgery

### Removal Procedure

1. Sedate the patient and apply anesthetic as needed.
2. Make an incision with a scalpel on the relevant body region (torso, groin, or head depending on organ location).
3. Retract the incision with a retractor.
4. Clamp bleeding vessels with a hemostat.
5. Use a scalpel to detach the organ (60 seconds). If this step fails, arterial bleeding occurs at the cut site.
6. Remove the organ with a hemostat or fork (60 seconds). The organ is now available for storage or transplant.
7. Close the incision with cautery.

A kitchen fork can substitute for a hemostat in field conditions, though failure rates increase.

### Transplant Procedure

Follow the same incision and retraction steps on the recipient. Once the cavity is open, the organ is placed inside. The surgical system automatically checks compatibility.

**Compatibility factors:** Blood type and species must both match for rejection-free transplant. An incompatible organ immediately begins accumulating germ levels, progressing through infection stages (see [Internal Organs](InternalOrgans.md) for rejection timetable). If no compatible donor organ is available, synthetic or robotic organ substitutes bypass the rejection system entirely.

### Limb Reattachment

A severed limb recovered in time can be reattached surgically. The limb must be in the patient's inventory or on an adjacent surface. Reattachment follows the same incision procedure; the limb is placed against the stump and sutured into place. Bone damage and any wound damage to the reattached limb persist and require separate treatment.

---

## Species Anatomy Notes

**Unathi:** Upper and lower ribplates (chest and groin) must be incised before internal surgery in those regions. Ribplates are not separate organs; they are structural features of the relevant body region. This does not apply to arms, legs, or head surgery.

**Promethean:** No standard limbs or organs in the conventional sense. All internal function is handled by the slime core. Prometheans can regenerate lost limbs passively given sufficient time and light. They cannot receive conventional organ transplants. See [Internal Organs](InternalOrgans.md) for slime core details.

**Diona:** No internal organs in the standard sense; Diona anatomy is not affected by fractures and cannot develop organ infections. Standard organ surgery is not applicable.

**Vox:** Non-standard organ set; standard replacement organs are incompatible. Vox cannot be resleeved. Prosthetic limbs are compatible with appropriate surgical care.

---

*See also: [Internal Organs](InternalOrgans.md), [Surgery](Surgery.md), [Triage and Patient Assessment](Triage.md), [Injuries](Injuries.md)*
