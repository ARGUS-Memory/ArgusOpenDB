[ARGUS Station Database](../../README.md) > [Systems](../README.md) > [Medical](README.md) > Diseases

# Diseases

Diseases are transmissible conditions that progress through stages over time, producing escalating symptoms in infected crew members. Some diseases occur spontaneously or from environmental exposure; others are engineered through the virology lab. Medical staff are responsible for identification, containment, and treatment of all active outbreaks.

---

## Disease Mechanics

### Spread Modes

Every disease has one or more spread modes that determine how it passes between individuals.

| Spread Mode | Transmission |
|---|---|
| Airborne | Transmitted through shared atmosphere; no contact required |
| Contact | Transmitted by direct physical contact with an infected individual |
| Blood | Transmitted through blood transfer (injections, bites, wounds) |
| Fluids | Transmitted through bodily fluid exposure |
| Non-contagious | Cannot spread person-to-person; must be contracted independently |

### Stages

Diseases advance through numbered stages as infection progresses. Each stage has a probability of advancing to the next every ~2 seconds. Stage advancement is not guaranteed and can be slowed by treatment, species resistance, or a strong immune response. Devolving is also possible for some diseases if conditions change.

At each stage the disease applies its symptoms and checks for cure eligibility. A cure applied before reaching a late stage may halt progression and begin recovery; some diseases require specific interventions at specific stages.

### Cure Conditions

Most diseases specify one or more reagents whose presence in the bloodstream triggers a cure. Reagent-based cures are applied through standard injection or ingestion. A small number of diseases require non-chemical intervention (surgery, isolation, rest).

### Species Variation

Several species have innate disease resistance or vulnerability.

- **Promethean:** Immune to all standard diseases. Their biology does not support pathogen colonization.
- **Unathi:** ~50% reduced infection risk.
- **Tajaran:** ~50% reduced infection risk.
- **Xenochimera:** Carries a dormant form of Roanoke Syndrome by default. This does not affect the host but may be relevant in certain medical contexts.

---

## Preset Diseases

The following diseases may appear spontaneously on station or result from environmental contamination.

### XY-Rhinovirus (Common Cold)

A mild respiratory infection spread through the air.

**Spread:** Airborne
**Danger:** Mild

| Stage | Symptoms |
|---|---|
| 1 | Sneezing, mild discomfort |
| 2 | Runny nose, coughing |
| 3 | Severe coughing, fatigue; may progress to flu |

**Cure:** Spaceacillin or chicken soup.

---

### H13N1 (Flu)

A more aggressive respiratory infection. Can develop from an untreated cold.

**Spread:** Airborne
**Danger:** Moderate

| Stage | Symptoms |
|---|---|
| 1 | Sneezing, aching |
| 2 | Coughing, fatigue, muscle pain |
| 3 | Severe muscle pain, toxin damage |

**Cure:** Spaceacillin. Supportive care to manage toxin damage while the infection clears.

---

### Salmonella (Food Poisoning)

A non-contagious gastrointestinal infection acquired from contaminated food.

**Spread:** Non-contagious
**Danger:** Mild to moderate

| Stage | Symptoms |
|---|---|
| 1 | Nausea, mild stomach pain |
| 2 | Vomiting, abdominal cramps |
| 3 | Severe vomiting; exhaustion; patient may fall asleep involuntarily |

**Cure:** Sleep (rest allows the body to clear the infection naturally). No reagent required.

---

### Cryptococcus Cosmosis (Brainrot)

A fungal-origin neural pathogen spread through contact.

**Spread:** Contact
**Danger:** Serious

| Stage | Symptoms |
|---|---|
| 1 | Confusion, brief disorientation |
| 2 | Slurred speech, impaired cognition |
| 3 | Significant brain damage, hallucinations |
| 4 | Severe brain damage; patient may become unresponsive without treatment |

**Cure:** Alkysine. Begin treatment as early as possible to limit permanent neural damage.

---

### Appendicitis

An inflammation of the appendix. Non-contagious. Only affects species with an appendix organ (Humans and most baseline humanoids; not present in Unathi).

**Spread:** Non-contagious
**Danger:** Serious without intervention

| Stage | Symptoms |
|---|---|
| 1 | Mild abdominal pain |
| 2 | Sharp stabbing pain, weakness |
| 3 | Severe pain, debilitating weakness |

**Cure:** Surgical removal of the appendix. No chemical cure exists; appendicitis will not resolve without surgery.

---

### Magnitis

A metallic-resonance pathogen spread through the air. Causes the patient's body to generate a low-level magnetic field.

**Spread:** Airborne
**Danger:** Moderate to serious

| Stage | Effect radius | Symptoms |
|---|---|---|
| 1 | ~2 metres | Metal objects nearby drift toward the patient |
| 2 | ~4 metres | Larger metal objects attracted; silicon-based creatures may be pulled toward patient |
| 3 | ~4 metres | Continued metal attraction, increased pull on silicon-based creatures |
| 4 | ~6 metres | Severe metal attraction; risk of injury from flying objects |

**Cure:** Iron injection. The additional iron saturates the magnetic resonance mechanism and neutralizes the infection.

> [!CAUTION]
> Patients with active Magnitis are a hazard to cyborg crew and to any nearby metal equipment. Isolate the patient from silicon personnel and engineering environments immediately upon diagnosis.

---

## Advanced Disease System (Virology)

The virology lab allows trained personnel to culture, analyze, and engineer novel pathogens using the advance disease framework. All advance diseases are built on five core statistics that determine their behavior.

### Core Statistics

| Statistic | Range | Effect |
|---|---|---|
| Resistance | 0-20 | Determines which reagents can cure the disease and how difficult treatment is |
| Stealth | 0-20 | Controls how visible symptoms are and how easily the disease is detected |
| Stage Rate | 0-20 | How quickly the disease advances through stages |
| Transmission | 0-20 | Determines spread mode and how readily it spreads |
| Severity | 0-20 | Overall impact of symptoms at each stage |

### Transmission Thresholds

The Transmission stat controls which spread modes are active.

| Transmission score | Spread modes |
|---|---|
| 0-5 | Blood only |
| 6-10 | Blood and bodily fluids |
| 11+ | Blood, fluids, and direct contact |

For airborne transmission, the disease must be specifically engineered with that property.

### Danger Rating

The overall danger of an advance disease is calculated from its statistics and symptoms. Ratings from lowest to highest: Beneficial, Harmless, Minor, Mild, Moderate, Severe, Dangerous, Deadly, Pandemic.

A disease with negative danger rating (Beneficial) causes no harm and may produce positive effects. These are used by virologists to engineer curative or enhancement pathogens.

### Cure Generation

The cure for an advance disease is derived from its Resistance score, mapped to one of eleven reagent groups. A disease with Resistance 0 is cured by common over-the-counter compounds; a disease with Resistance 20 requires rare or synthesized reagents. The cure reagent group is fixed when the disease is created or mutated.

### Disease Evolution

Advance diseases can mutate over time or through deliberate virology procedures:

- **Evolve / Devolve:** Increases or decreases a single statistic by one point, potentially changing symptoms, spread mode, or cure.
- **Neuter:** Reduces the disease to a non-harmful state without eliminating it.
- **Falter:** Introduces a random statistical reduction; may weaken or change the disease unpredictably.
- **Mix:** Combines two advance diseases in a living host, producing a hybrid with statistics averaged from both parents and a new combined symptom set.

### Symptom System

Advance disease symptoms are discrete effects activated at specific stages. Symptoms are attached based on stage rate, severity, and other statistics. The virology interface allows viewing and modifying symptom assignments for cultured samples.

---

*See also: [Chemistry](Chemistry.md), [Internal Organs](InternalOrgans.md), [Triage and Patient Assessment](Triage.md)*
