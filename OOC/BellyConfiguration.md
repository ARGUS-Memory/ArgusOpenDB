[OOC Reference](README.md) > Belly Configuration

# Belly Configuration

Complete reference for belly modes, configuration parameters, and behavioral flags. Each belly on a predator character is a named configuration with independently settable values across all parameters listed here.

---

## Belly Modes

The mode determines what happens to prey inside the belly each process tick.

| Mode | Constant | Behavior |
|---|---|---|
| Hold | DM_HOLD | Prey is retained with no processing. Default starting mode. |
| Digest | DM_DIGEST | Prey takes damage per tick across configured damage types and is converted to nutrition on death. |
| Absorb | DM_ABSORB | Predator takes prey's nutrition gradually. When prey's nutrition falls below 100, prey enters an absorbed state (integrated into the predator but not dead). |
| Unabsorb | DM_UNABSORB | Reverses absorption. Requires predator nutrition of 100 or higher. Returns absorbed prey to normal form. |
| Drain | DM_DRAIN | Continuous nutrition theft without absorption transformation. |
| Shrink | DM_SHRINK | Prey shrinks by 1% per tick toward the belly's configured minimum size. |
| Grow | DM_GROW | Prey grows by 1% per tick toward the belly's configured maximum size. |
| Size Steal | DM_SIZE_STEAL | Predator grows and prey shrinks simultaneously by 1% per tick. |
| Heal | DM_HEAL | Predator expends nutrition to heal prey injuries each tick. Cost: 5 nutrition per tick for synthetic prey; higher for organic prey. |
| Egg | DM_EGG | Prey is encased in an egg object. After 10 belly process cycles the egg is complete. |
| Selective | DM_SELECT | Behavior toggles: prey is processed under the belly's default mode normally, but struggle can switch it to Digest based on selectchance. |

---

## Digestion Parameters

These values control damage application in Digest mode.

| Parameter | Default | Function |
|---|---|---|
| digest_brute | 0.5 | Brute damage per tick |
| digest_burn | 0.5 | Burn damage per tick |
| digest_oxy | 0 | Oxygen damage per tick |
| digest_tox | 0 | Toxin damage per tick |
| digest_clone | 0 | Clone damage per tick |
| digest_max | 36 | Maximum total damage per tick across all types |
| slow_digestion | false | If enabled, all damage values are halved |
| nutrition_percent | 100% | What percentage of prey mass is converted to nutrition |

---

## Swallow Timing

| Parameter | Default | Function |
|---|---|---|
| human_prey_swallow_time | 100 deciseconds (10 sec) | Time to swallow a standard humanoid prey |
| nonhuman_prey_swallow_time | 30 deciseconds (3 sec) | Time to swallow non-humanoid prey |

---

## Escape and Release Configuration

| Parameter | Default | Function |
|---|---|---|
| escapable | Default | Controls whether and how prey can struggle free. Options: None (no escaping), Default (struggle triggers escape checks), Intent (escape depends on prey's active intent) |
| escapetime | 100 deciseconds | Time required to escape a non-escapable belly |
| escapechance | 0 to 100% | Probability of escaping per struggle attempt |
| escapechance_absorbed | 0 to 100% | Probability for absorbed prey to escape |
| escape_stun | -- | Weakness applied to the predator when prey successfully escapes, preventing immediate re-swallow loops |

---

## Struggle-Triggered Mode Changes

These parameters define what belly mode changes or behaviors can be triggered by prey struggling.

| Parameter | Function |
|---|---|
| selectchance | % chance struggle switches belly to Selective mode |
| digestchance | % chance struggle activates Digest mode |
| absorbchance | % chance struggle activates Absorb mode |
| belchchance | % chance predator belches when prey struggles |

---

## Transfer Parameters

| Parameter | Function |
|---|---|
| transferchance | % chance prey transfers to transferlocation belly on struggle |
| transferchance_secondary | % chance prey transfers to transferlocation_secondary |
| transferlocation | Name of the belly to transfer prey into on trigger |
| transferlocation_secondary | Name of a secondary transfer destination |

---

## Size and Resize

| Parameter | Default | Function |
|---|---|---|
| shrink_grow_size | 1.0 | Target size multiplier for Shrink, Grow, and Size Steal modes |

---

## Behavioral Flags

Mode flags are additive modifiers that apply to any belly mode, adding extra behaviors on top of the base mode.

| Flag | Effect |
|---|---|
| DM_FLAG_NUMBING | Numbs prey during digestion; reduces pain message output |
| DM_FLAG_STRIPPING | Removes prey's clothing during processing |
| DM_FLAG_LEAVEREMAINS | Indigestible items drop out rather than being destroyed |
| DM_FLAG_THICKBELLY | Muffles sounds from inside the belly |
| DM_FLAG_AFFECTWORN | Applies effects to equipped worn items as well |
| DM_FLAG_JAMSENSORS | Jams sensor implants on prey inside the belly |
| DM_FLAG_SPARELIMB | Prosthetic limbs are not digested |
| DM_FLAG_SLOWBODY | Slows the predator's own body digestion separately |
| DM_FLAG_MUFFLEITEMS | Muffles item interaction sounds |
| DM_FLAG_TURBOMODE | Accelerates all belly processing |
| DM_FLAG_ABSORBEDVORE | Allows absorbed prey to swallow other prey from inside |
| DM_FLAG_WETTENS | Makes prey wet on entry or processing |

---

## Auto-Transfer System

For predator-controlled automations, bellies can be configured to automatically move prey to a specified destination belly on a timer.

| Parameter | Function |
|---|---|
| autotransferchance | % chance of auto-transfer per attempt |
| autotransferwait | Seconds between transfer attempts |
| autotransferlocation | Belly name to transfer prey into |
| autotransfer_enabled | Master toggle for this system |
| autotransfer_whitelist / blacklist | Restricts auto-transfer to certain prey types |

---

## Reagent Belly System

Bellies can be configured to generate reagents into an internal fluid pool based on nutrition processing.

| Parameter | Function |
|---|---|
| reagentbellymode | Enables reagent generation |
| reagent_mode_flags | Which modes produce reagents (nutrition processing, digestion, absorption, drain) |
| generated_reagents | List of reagent IDs and generation amounts per cycle |
| gen_cost | Nutrition cost per generation cycle |
| gen_time | Seconds between generation cycles |
| custom_max_volume | Maximum liquid volume the belly can hold |
| custom_ingested_color | Color of the ingested reagent layer |

---

## Visual and Audio Settings

| Parameter | Default | Function |
|---|---|---|
| name | -- | Display name of the belly |
| vore_sound | Gulp | Sound played on prey entry |
| release_sound | Splatter | Sound played on prey exit |
| vore_verb | ingest | Verb used in entry messages |
| release_verb | expels | Verb used in exit messages |
| is_wet | true | Whether the belly produces wet audio textures |
| emote_time | 60 seconds | Interval between automatic belly emotes |
| emote_active | -- | Whether automatic emotes fire at all |
| belly_fullscreen | -- | Fullscreen overlay icon state shown to prey |

---

*See also: [Vore Overview](VoreOverview.md), [Prey Experience](PreyExperience.md)*
