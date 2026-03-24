[ARGUS Station Database](../../README.md) > [Systems](../README.md) > [Medical](README.md) > Virology

# Virology

The virology laboratory provides equipment for the isolation, study, and engineering of advanced pathogenic agents. Where the standard disease system involves naturally occurring or environmentally introduced conditions, virology concerns itself with constructed viruses: multi-symptom pathogens assembled from discrete symptom vectors and tuned through four modifiable properties. Virologists may engineer beneficial strains for distribution across the crew, or analyse and counter hostile outbreaks.

This article covers the advanced virus system. For preset diseases (common cold, influenza, food poisoning, etc.), see [Diseases](Diseases.md).

---

## Virus Properties

Every advanced virus carries four properties that govern its behaviour in a host. Each symptom contributes a positive or negative delta to each property; the final virus value is the sum of all symptom contributions.

| Property | Effect |
|---|---|
| **Stealth** | How detectable the virus is. High stealth hides the virus from medical scanners. Negative stealth produces obvious symptoms that are readily identified. |
| **Resistance** | How difficult the virus is to treat. Higher resistance requires more specialised treatment compounds and slows the rate at which each stage clears. |
| **Stage Speed** | How quickly the virus progresses through its stages. High stage speed accelerates symptom onset; negative values cause slow, chronic progression. |
| **Transmission** | How readily the virus spreads between hosts. Low values limit spread to blood-to-blood contact; higher values add fluid exposure as a vector; very high values extend spread to direct physical contact. |

---

## Symptom System

A virus can carry up to six active symptom vectors simultaneously. When a seventh is introduced, one existing symptom is displaced at random to make room. Symptom selection and combination is performed at the virology lab console using isolated symptom cultures.

Each symptom fires on a per-stage cycle. Most symptoms are conditional: they only activate from a certain stage onward, or only under specific threshold conditions derived from the virus's combined stat values. Threshold behaviours unlock additional effects when a relevant property exceeds a defined value, typically allowing more damaging, more transmissible, or more concealed operation.

### Severity Levels

Symptoms are rated on a severity scale that governs research point value and the default stage at which effects begin. Level 0 symptoms are cosmetic or mildly inconvenient; level 9 symptoms represent life-threatening or structurally destructive effects.

---

## Symptom Catalogue

### Damaging Symptoms

| Symptom | Stealth | Resistance | Stage Speed | Transmission | Primary Effect |
|---|---|---|---|---|---|
| Acute Respiratory Distress (Choking) | -2 | 0 | -1 | -2 | Continuous oxygen loss; rate doubles at Transmission 8 |
| Necrotizing Fasciitis | -3 | -2 | 0 | -1 | Brute damage and bleeding wounds; severe bleeding at Transmission 8 |
| Spontaneous Combustion | 1 | -1 | -2 | -1 | Ignites host; spreads via shed skin at Transmission 8 |
| Photosensitivity | -2 | 2 | 1 | -4 | Fire damage scaling with ambient light level |
| Hyphema | -1 | -3 | -4 | -2 | Progressive eye damage; eye loss at Resistance 12 |
| Irradiant Cells | -1 | 2 | 1 | 2 | Radiation damage; increases at Stage Speed 8 |
| Aptopic Culling | 1 | 1 | 1 | -2 | Converts radiation and toxin damage into wounds |

### Motor and Behavioural Symptoms

| Symptom | Stealth | Resistance | Stage Speed | Transmission | Primary Effect |
|---|---|---|---|---|---|
| Choreomania | 2 | 0 | 3 | 1 | Forces dance movements |
| Flippinov | 2 | 0 | 3 | 1 | Forces tumbling |
| Spyndrome | -1 | 3 | 3 | 1 | Forces spinning; floor spin at Resistance 6 |
| Mlemington | 0 | 3 | 3 | 1 | Forces licking behaviour; spreads via saliva at Transmission 8 |

### Neural and Sensory Symptoms

| Symptom | Stealth | Resistance | Stage Speed | Transmission | Primary Effect |
|---|---|---|---|---|---|
| Confusion | 1 | -1 | -3 | 0 | Disorientation; hidden until active at Stealth 4 |
| Hallucigen | 1 | -1 | 1 | 1 | Hallucinations; mimics beneficial symptoms at Stealth 2 |
| Headache | -1 | 4 | 2 | 0 | Weakness at Stage Speed 6; stun at Stage Speed 9 |
| Deafness | -1 | -1 | 1 | -3 | Ear damage; permanent hearing loss at Resistance 9 |
| Lingual Dislocation | 0 | 2 | 1 | 1 | Randomises host language; gibberish at Resistance 5 |
| Narcolepsy | 1 | -1 | -2 | -2 | Drowsiness and uncontrolled sleep |

### Metabolic and Physiological Symptoms

| Symptom | Stealth | Resistance | Stage Speed | Transmission | Primary Effect |
|---|---|---|---|---|---|
| Fever | -1 | 3 | 3 | 2 | Elevated body temperature; unsafe heat at Resistance 5 |
| Shivering | 0 | 2 | 2 | 2 | Depressed body temperature; unsafe cold at Stage Speed 5 |
| Weight Loss | 0 | 2 | -2 | -1 | Nutritional drain and starvation risk |
| Hyperactivity | -4 | 0 | 2 | -3 | Stimulant effect; paranoia and hallucinations at Stage Speed 8 |

### Respiratory and Transmission Symptoms

| Symptom | Stealth | Resistance | Stage Speed | Transmission | Primary Effect |
|---|---|---|---|---|---|
| Cough | -1 | 3 | 1 | 2 | Item loss; coughing fits at Resistance 10; airborne spread at Transmission 11 |
| Sneezing | -2 | 3 | 0 | 4 | Sneezing fits; airborne spread at Transmission 12 |
| Bluespace Sneezing | -2 | 3 | 0 | 1 | Teleports host to a nearby location on sneeze |
| Vomiting | -2 | 0 | 1 | 2 | Projectile emesis; blood vomit at Stage Speed 5 |

### Dermal Symptoms

| Symptom | Stealth | Resistance | Stage Speed | Transmission | Primary Effect |
|---|---|---|---|---|---|
| Itching | 0 | 3 | 3 | 1 | Scratching behaviour; minor damage at Stage Speed 7 |
| Alopecia | 0 | 3 | 2 | 2 | Hair loss |

### Healing Symptoms

These symptoms produce beneficial effects and are used to engineer therapeutic virus strains.

| Symptom | Stealth | Resistance | Stage Speed | Transmission | Primary Effect |
|---|---|---|---|---|---|
| Metabolic Boost | -1 | -2 | 2 | 1 | Doubles chemical metabolism; triples at Stage Speed 10 |
| Oxygenation | 1 | -3 | -3 | -4 | Regenerates oxygen loss; regenerates blood at Resistance 8 |
| Tissue Hydration | 0 | -1 | 0 | 1 | Heals burn damage using water from bloodstream |
| Toxolysis | 0 | -2 | 2 | -2 | Purges chemicals from bloodstream |
| Eternal Youth | 3 | 4 | 4 | -4 | Rejuvenation messaging with high stealth and resistance |
| Pituitary Disruption | -3 | -2 | 1 | -2 | Size increase, brute healing; limb regeneration at Stage Speed 12 |

### Structural and Rare Symptoms

| Symptom | Stealth | Resistance | Stage Speed | Transmission | Primary Effect |
|---|---|---|---|---|---|
| Mass Revectoring | 1 | 0 | 2 | 2 | Resizes host (subtypes: growth or shrinkage) |
| Biometallic Replication | 0 | 1 | 4 | -1 | Converts biological tissue to biometallic analogues; can infect synthetics |
| SBG Syndrome | 1 | 2 | 3 | 1 | Produces cockroaches |
| Macrophage | -4 | -1 | -2 | 2 | Spawns phage organisms from the host |
| Blob Spores | 1 | 6 | -2 | 1 | Spawns blob structures (not naturally occurring; requires administrative introduction) |

### Viral Control Symptoms

These symptoms modify the virus's own properties rather than directly affecting the host.

| Symptom | Stealth | Resistance | Stage Speed | Transmission | Primary Effect |
|---|---|---|---|---|---|
| Viral Self-Adaptation | 3 | 5 | -3 | 0 | Boosts virus stealth and resistance |
| Viral Evolutionary Acceleration | -2 | -3 | 5 | 3 | Accelerates spread and stage progression |
| Viral Power Multiplier | 2 | 2 | 2 | 2 | Multiplies effectiveness of other symptoms |
| Viral Aggressive Metabolism | 1 | 1 | 3 | -4 | Begins at advanced stage; self-resolves over time |
| Viral Suspended Animation | 4 | -2 | -2 | 1 | Suppresses all other symptoms until stage 5 |
| Synthetic Infection | 1 | 2 | 0 | 1 | Enables infection of synthetic and robotic hosts |
| Necrotic Agent | 2 | -2 | -1 | 0 | Enables spread from and infection of deceased hosts |

---

## Treatment

### Cure Compounds

The compounds capable of treating an advanced virus are determined by its resistance value, adjusted for symptom count. The effective resistance tier is calculated as the virus's total resistance minus half the number of symptoms it carries, clamped between 1 and 11. More symptom complexity therefore reduces effective resistance and makes treatment more accessible.

The treatment reagents available at each tier are listed below. All are drawn at random; only one cure compound is assigned to any given virus instance.

| Effective Resistance Tier | Possible Treatment Compounds |
|---|---|
| 1 | Water, nutriment, iron supplement |
| 2 | Ethanol, radium, potassium, lithium |
| 3 | Sodium chloride, nicotine, bliss |
| 4 | Antitoxin, ethylredoxrazine, fuel, cleaning fluid |
| 5 | Spaceacillin, mindbreaker toxin, cryoxadone |
| 6 | Tramadol, kelotane, inaprovaline |
| 7 | Leporazine, holy water, alkysine |
| 8 | Paroxetine, radium, phoron |
| 9 | Adranol, mutagen, arithrazine |
| 10 | Lipozine, liquid silicone, sulfuric acid |
| 11 | Alien sustenance, cordrazine, oxycodone |

### Cure Rate

The probability of clearing a stage per cycle scales inversely with total resistance. A low-resistance virus clears readily when treated; a high-resistance strain clears slowly even with the correct compound present. The cure compound must be present in the host's bloodstream continuously for treatment to progress.

### Scanning and Identification

A virus with high stealth will not appear on standard medical scanners. Dedicated virology equipment can detect concealed strains. Identifying the assigned cure compound requires either a virus analyser or laboratory culture work.

---

## Engineering Notes

Combining symptoms with complementary stealth and resistance values produces more resilient viruses; combining high stage speed with strong transmission vectors accelerates outbreak potential. Beneficial viruses are typically designed with healing symptoms, negative transmission (to prevent unwanted spread), and low resistance to allow easy self-treatment if needed. Any strain reaching the stage where Cough or Sneezing hits its spread threshold becomes a significant containment risk.

Viruses requiring two or more specific cure compounds simultaneously are possible using the relevant disease flags but are rare in natural or engineered strains encountered on station.
