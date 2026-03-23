[ARGUS Station Database](../../README.md) > [Systems](../README.md) > [Medical](README.md) > Internal Organs

# Internal Organs

Station medical staff treat internal organ damage as a distinct category from general brute and burn damage. Each organ has its own damage pool, failure symptoms, and treatment requirements. This document covers all standard internal organs, their failure thresholds, infection behavior, and species-specific variants.

---

## Damage Thresholds

All standard organs share the same numerical thresholds:

| State | Damage |
|---|---|
| Healthy | 0 to 9 |
| Bruised | 10 to 59 |
| Broken | 60 to 119 |
| Dead | 120 (maximum) |

Bruised organs produce mild symptoms. Broken organs produce severe symptoms and may directly threaten the patient. Dead organs cease all function and require surgical intervention to restore.

Organ damage is not automatically healed by standard brute or burn treatments. Bruise packs and advanced bruise packs applied to the relevant body region heal organ damage; peridaxon injections (5 units) restore dead organs to minimal function.

---

## Vital Organs

### Brain

Located in the head. The brain governs consciousness and controls neural function including respiration. At 80% control efficiency or lower (damage 24+), the lungs begin to malfunction independently, compounding respiratory failure.

Death occurs immediately on removal from a living patient. A recently deceased patient can be resuscitated with a defibrillator within a limited window; this window narrows each second the patient remains dead. The brain retains identity and mind data; it can be transplanted into a compatible body or mechanized housing.

Broken brain symptoms include severe cognitive impairment. Infection at level 2 causes neck stiffness, dizziness, and confusion.

### Heart

Located in the torso. Maintains circulation and pulse. Robotic hearts produce no detectable pulse. Broken heart symptoms include severe stabbing chest pain and periodic halloss damage.

Infection at level 2 causes endocarditis with stabbing chest pain. Death occurs on removal from a living patient.

### Lungs

Located in the torso. Govern gas exchange and respiration. Bruised lungs cause occasional blood coughing and gradual breath loss. Broken lungs cause frequent blood coughing, severe gasping, and rapid breath loss (15 units per event). Compound effects with brain damage accelerate respiratory failure.

Infection at level 2 causes bacterial pneumonia with sharp breathing pain and significant continuous oxygen loss.

---

## Non-Vital Organs

### Liver

Located in the groin. Filters toxins from the bloodstream at full efficiency. Bruised: 50% filter efficiency. Broken: 33% filter efficiency. At high toxin load (50+ units), a damaged liver causes toxin overflow to other organs.

Alcohol metabolization damages the liver proportionally to intake. The liver takes damage from ambient toxin buildup above 50 units even when healthy. Infection at level 2 causes upper-right abdominal pain and elevated toxin accumulation.

### Kidneys

Located in the groin. Process waste reagents including coffee metabolites. Bruised kidneys produce 0.1 toxin units per second from coffee exposure; broken kidneys produce 0.3 per second. When toxin levels fall below 10% of maximum, healthy kidneys can purge 1 to 3 toxin units passively.

Infection at level 2 causes stabbing lower back pain and forces the patient into walking pace.

### Spleen

Located in the torso. Filters blood and supports infection resistance. A dead spleen causes haemophilia (elevated bleeding), triggers an internal bleeding wound, and releases 15 units of toxins. Healthy unbruised spleens reduce active organ infections by 3 to 10 germ units per second.

High ambient toxins (30+ units) damage the spleen. Infection at level 2 produces haemophilia and either toxin accumulation or a secondary brain infection.

### Stomach

Located in the groin. Produces stomach acid (up to 30 units, 40 for Unathi). Broken stomach symptoms include twisting abdominal pain and intermittent vomiting. Infection at level 2 causes gastroenteritis with agony and vomiting.

### Appendix

Located in the groin. Functionally vestigial; serves no active role in healthy state. Inflammation causes stinging or stabbing abdominal pain and occasional vomiting.

### Intestines

Located in the groin. Nutrient absorption and waste processing. Infection at level 2 causes abdominal tearing pain and forces walking pace.

### Larynx

Located in the torso. Governs speech. Can assist with speaking non-native languages when healthy. Not vital; removal does not cause death but may affect communication.

### Eyes

Located in the head. Bruised eyes cause visual blurring (20 blur units). Broken eyes cause complete blindness. Infection (conjunctivitis) at level 2 causes eye irritation and 10 blur units. Robotic eyes can change color but are vulnerable to EMP damage.

---

## Infection System

Organs accumulate germ levels through environmental contamination and physical damage. The spleen reduces active infections when healthy.

| Level | Germ Threshold | Symptoms |
|---|---|---|
| Level 1 | 100 germs | Organ-specific mild symptoms begin |
| Level 2 | 500 germs | Significant symptoms; potential toxin damage |
| Level 3 | 1,000 germs | Severe necrosis; rapid damage to organ |
| Maximum | 1,500 germs | Infection ceiling |

Antibiotic treatment reduces germ levels at rates that depend on infection severity:

| Infection stage | Reduction rate |
|---|---|
| Below level 1 | Instant clearance |
| Level 1 to 2 | Fast reduction (approximately 1 minute at standard dosing) |
| Level 2 to 3 | Moderate reduction (approximately 5 minutes) |
| Level 3 and above | Slow reduction (10+ minutes) |

Overdosing on antibiotics prevents additional damage but does not accelerate clearance beyond normal rates.

---

## Organ Transplant and Rejection

Transplanted organs check blood type and species compatibility against the recipient. Incompatible organs enter a rejection process beginning immediately after transplant.

**Rejection progression:**

| Rejection stage | Germ gain rate | Additional effects |
|---|---|---|
| Initial | +1 germ per interval | None |
| Early | +1 to 2 germs per interval | None |
| Progressing | +2 to 3 germs per interval | None |
| Critical | +3 to 5 germs per interval | 1 to 2 toxin damage per interval |

Rejection proceeds identically to infection and ultimately kills the organ if untreated. Compatible transplants from blood- and species-matched donors do not trigger rejection. See [External Organs](ExternalOrgans.md) for surgical procedure details.

---

## Species Organ Variants

### Promethean (Slime Core)

The slime core replaces all standard organs. Located in the torso, it is an open reagent container with 50-unit capacity colored to match the individual's hue. It does not decay. A bruised slime core heals 1 damage per second passively.

Reviving a dead Promethean requires injecting the slime core with 40 units of phoron, which triggers body regeneration from stored DNA.

### Vox

The Vox cardiovascular and filtration system uses entirely non-standard anatomy. The heart is located in the groin (not the torso). Air capillaries replace lungs and process phoron-nitrogen atmospheres rather than oxygen-nitrogen. A filtration bladder (torso) and waste tract (torso) replace kidneys and liver respectively. The ribcage extends to encase the groin region.

### Unathi

The Unathi filtration organ replaces both liver and kidneys in a single structure. It takes damage from coffee and sugar exposure (bruised: 0.1 toxin units per second per substance, broken: 0.3 per second). The stomach holds 40 units of acid instead of the standard 30. Unathi lack kidneys and an appendix entirely.

Unathi are shielded by ribplates in both the chest (upper ribplates) and groin (lower ribplates). These must be incised before internal surgery in those body regions. See [Triage and Patient Assessment](Triage.md) for surgical considerations.

### Horror-Infused Organs

Cult-corrupted organs cannot decay, cannot be rejected, self-heal when bruised (1 damage per second), and produce aberrant physiological effects. The corrupted voicebox forces walking pace when used and cannot produce standard language output. Other corrupted organs generate unusual metabolites, spawn organisms, or produce light sensitivity. These organs should be removed surgically and incinerated.

---

*See also: [External Organs](ExternalOrgans.md), [Surgery](Surgery.md), [Triage and Patient Assessment](Triage.md), [Injuries](Injuries.md)*
