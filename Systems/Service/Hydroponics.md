[ARGUS Station Database](../../README.md) > [Systems](../README.md) > [Service](README.md) > Hydroponics

# Hydroponics

The hydroponics bay provides controlled growing trays for the cultivation of food crops, medicinal plants, and specialist botanical specimens. Botanists manage tray conditions, seed selection, chemical application, and mutations to supply the kitchen and other departments. The bay also houses beehives, whose colonies can be managed to produce honey and to improve tray yields through pollination.

---

## Hydroponics Trays

Each tray maintains independent values for water level, nutrient level, weed population, pest population, and the health of the plant it contains. Light and atmospheric conditions are drawn from the ambient environment unless supplemented directly. A plant that cannot meet its environmental requirements loses health each cycle.

### Water and Nutrients

Water is consumed each cycle according to the plant's water consumption trait. The default rate is 3 units per cycle; high-consumption plants can deplete a tray quickly. Nutrients are consumed at a lower rate (default 0.25 units per cycle). Both resources must be actively replenished; the tray has no automatic supply.

A plant deprived of either water or nutrients loses 1 to 3 health per cycle depending on severity of the deficit.

### Light and Temperature

Each plant species has an ideal light level and ideal temperature, along with tolerance ranges for each. If the ambient reading falls outside the tolerance range, the plant takes periodic health damage. Standard growing conditions (room temperature, ambient lighting) are sufficient for most food crops. Specialist plants may require dedicated heating, cooling, or supplemental lighting.

### Weeds and Pests

Weeds and pests accumulate independently over time. Weeds are more likely to appear when the tray has adequate water and nutrients. Pests appear at a low base rate regardless of conditions. Both values are bounded between 0 and 10.

A plant begins losing health once weeds or pests exceed its tolerance threshold (default 5 for both). Herbicides and pesticides applied to the tray reduce these values. Carnivorous plants consume pests directly. Parasite plants gain health from weed presence rather than being harmed by it.

### Plant Health and Death

A plant's health is bounded by its endurance trait (default 100). When health reaches zero the plant dies and cannot be harvested. A dead plant should be removed with a spade to clear the tray for replanting.

---

## Growth and Harvest

### Maturation and Production

A plant tracks its age in growth cycles. It becomes ready to harvest once its age meets or exceeds its maturation value. For plants with the repeat harvest trait, subsequent harvests become available each time the interval since the last harvest equals or exceeds the production value. Single-harvest plants yield once and are then spent.

### Yield and Potency

At harvest, the tray produces a number of units equal to the plant's yield trait. Potency governs the concentration of reagents within each unit and affects secondary effects such as damage from throwing, strength of injected compounds, and explosion intensity. Potency ranges from 0 to 200; the default for most species is between 5 and 20.

### Mutation Level

Each tray tracks a mutation level. Mutagenic reagents raise this value; it decreases slightly each cycle on its own. When mutation level reaches 100, the plant may mutate into a related variant. Highly mutable plants (marked immutable = -1 in their genetic profile) have a 5% chance to mutate each cycle regardless of mutation level. Plants marked immutable = 1 will never mutate under any conditions.

---

## Chemical Applications

Reagents applied to a tray affect plant health, growth, and mutation in various ways.

### Beneficial Reagents

| Reagent | Effect |
|---|---|
| Ammonia | +1 health per cycle |
| Diethylamine | +2 health per cycle |
| EZ-Nutrient | +1 health per cycle; replenishes nutrients |
| RobustHarvest | +1 health; +0.2 yield modifier |
| Left-4-Zed | +1 health; +0.2 mutation modifier |
| Cryoxadone | +3 health per cycle |
| Nutriment | +1 health per cycle |
| Beer | +0.25 health per cycle |
| Milk | +0.1 health per cycle; counts as water |

### Weed and Pest Control

| Reagent | Weed Effect | Pest Effect |
|---|---|---|
| Plant-B-Gone | -8 weeds | -- |
| Phosphoric acid | -4 weeds | -- |
| Chlorine | -3 weeds | -- |
| Sulfuric acid | -2 weeds | -- |
| Fluorine | -4 weeds | -- |
| Diethylamine | -- | -2 pests |
| Sugar | -- | +2 pests (attracts) |

### Mutagenic Reagents

Radium (minimum 8 units) and mutagen (minimum 15 units) trigger genetic mutation when present in the tray in sufficient concentration. Both raise mutation level and can produce random trait shifts when applied.

### Reagents Toxic to Plants

Antitoxin, toxin, fluorine, chlorine, sulfuric acid, phosphoric acid, Plant-B-Gone, and radium all cause health damage to the plant if present above the plant's toxin tolerance. Plant-B-Gone and phosphoric acid are the most damaging.

---

## Seed Traits

Plants carry genetic traits that govern their behaviour. Most traits have numerical values that can be shifted by mutation; a few are boolean flags. The following table covers all traits tracked by the genetic system.

| Trait | Description |
|---|---|
| Maturation | Cycles before first harvest |
| Production | Cycles between subsequent harvests |
| Yield | Units produced per harvest |
| Potency | Reagent concentration and secondary effect strength |
| Endurance | Maximum plant health |
| Nutrient Consumption | Nutrients consumed per cycle |
| Water Consumption | Water consumed per cycle |
| Ideal Heat | Preferred temperature in Kelvin |
| Heat Tolerance | Survivable deviation from ideal temperature |
| Ideal Light | Preferred light level |
| Light Tolerance | Survivable deviation from ideal light |
| Low Pressure Tolerance | Minimum survivable pressure in kPa |
| High Pressure Tolerance | Maximum survivable pressure in kPa |
| Toxin Tolerance | Threshold before chemical reagents cause damage |
| Weed Tolerance | Weed level before health loss begins |
| Pest Tolerance | Pest level before health loss begins |
| Harvest Repeat | Whether the plant produces multiple harvests |
| Spread | 0 = contained; 1 = creeping growth; 2 = full vine |
| Carnivorous | 0 = none; 1 = eats tray pests; 2 = attacks living things as vine |
| Parasite | Gains health from weeds instead of being harmed |
| Juicy | Creates a splatter when thrown |
| Explosive | Detonates on impact when thrown |
| Stings | Injects reagents into targets when thrown or handled |
| Teleporting | Teleports targets struck by the fruit |
| Bioluminescent | Emits light; colour configurable |
| Produces Power | Fruit can be used to generate electrical charge |
| Sporing | Periodically releases chemical spore clouds |

---

## Mutation Gene Categories

Genetic mutations fall into 12 categories, each of which modifies a specific subset of traits. A mutation event selects one or more categories at random and shifts the affected traits by a bounded random amount. Highly mutable plants apply two mutation degrees per event; standard plants apply one.

| Gene Category | Traits Affected |
|---|---|
| Biochemistry | Potency |
| Hardiness | Toxin tolerance, pest tolerance, weed tolerance, endurance |
| Environment | Ideal heat, ideal light, light tolerance |
| Metabolism | Nutrient and water requirements, temperature alteration |
| Diet | Carnivorous level, parasite flag, consumption rates |
| Atmosphere | Heat tolerance, pressure tolerances |
| Vigour | Production rate, maturation rate, spread level |
| Fruit | Stings, explosive, juicy flags |
| Output | Bioluminescence, power production, sporing |
| Special | Teleporting flag |
| Pigment | Plant and product colouration |

---

## Plant Catalogue

The following table lists common crop species with their base stats. Many species have mutant variants with modified reagent profiles or special traits; these are documented in-game in the seed vendor and dispensary interfaces.

| Plant | Maturation | Production | Yield | Potency | Reagents |
|---|---|---|---|---|---|
| Tomato | 8 | 6 | 2 | 10 | Nutriment, tomato juice |
| Apple | 6 | 6 | 5 | 10 | Nutriment, apple juice |
| Wheat | 6 | 1 | 4 | 5 | Nutriment, flour |
| Banana | 6 | 6 | 3 | 10 | Nutriment |
| Grapes | 3 | 5 | 4 | 10 | Nutriment, sugar, grape juice |
| Carrot | 10 | 1 | 5 | 10 | Nutriment, imidazoline, carrot juice |
| Corn | 8 | 6 | 3 | 20 | Nutriment, corn oil |
| Potato | 10 | 1 | 4 | 10 | Nutriment, potato juice |

Notable mutant varieties include the Blood Tomato (contains blood reagent), Poison Apple (cyanide), Bluespace Tomato (singularity reagent, causes teleportation when consumed), Voltato (electricity-producing potato), and Green Grapes (kelotane). All mutant variants are obtainable through genetic manipulation or mutagenic reagents applied to the base plant.

---

## Beekeeping

### Hive Basics

Beehives house self-sustaining colonies that produce honey and pollinate nearby trays. A hive's colony size is tracked as a percentage of maximum population (0-100%). Colonies grow slowly over time when the hive is closed and undisturbed. A colony at 90% capacity or above is ready to split.

### Pollination

When active, a hive checks for hydroponics trays within a moderate radius. Bees visit each tray and contribute a small health bonus per frame in the hive. The rate of honey production also scales with both colony size and the number of trays in range, up to a maximum of five trays contributing simultaneously.

### Frames

The hive holds up to five honey frames. Empty frames must be loaded by the botanist. Honey accumulates in the frames over time; a frame is ready to harvest when it has reached 100 units of stored honey. Loading additional frames increases total storage capacity and honey production rate.

### Harvesting and Handling

The hive lid must be opened with a crowbar before frames or bees can be accessed. If the colony is active (bee count above zero) and the hive is not pacified, the bees will attack. Using a bee smoker on an open hive pacifies the colony for approximately 30 seconds, permitting safe frame removal and colony management.

Harvested frames are processed in the honey extractor to yield bottled honey and raw wax.

### Colony Splitting

A colony at or above 90% strength can be split by a botanist holding a bee pack. The hive must be open and the bees pacified. Half the colony transfers to the pack, reducing the hive to a starter population; the filled pack can seed a new hive.
