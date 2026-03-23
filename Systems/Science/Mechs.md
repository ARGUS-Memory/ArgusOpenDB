[ARGUS Station Database](../../README.md) > [Systems](../README.md) > [Science](README.md) > Mechs and Exosuits

# Mechs and Exosuits

Exosuits are large mechanical frames piloted from an internal cockpit. They provide enhanced mobility, protection, and tool capacity beyond what a crew member can carry unassisted. Exosuits are constructed at the exosuit fabricator and require a power cell to operate. All movement consumes cell charge; heavier and faster suits drain more per step.

Exosuits accept modular equipment in hull, weapon, utility, universal, and special slots, the quantities of which vary by chassis. Equipment is installed and removed at the exosuit fabricator or by a roboticist using the appropriate tools.

---

## Chassis Catalogue

### APLU "Ripley"

The workhorse of the station exosuit fleet. A durable Autonomous Power Loader Unit designed for heavy cargo handling and mining operations. Fitted with an integrated cargo compartment that holds up to 10 items, and automatically collects ore tiles when a hydraulic clamp is installed. Ore is loaded into an ore box stored in the cargo compartment.

| Stat | Value |
|---|---|
| Max integrity | 200 |
| Max operating temperature | 20,000 K |
| Cargo capacity | 10 items |
| Step energy drain | 5 J |

---

### APLU "Firefighter"

A Ripley chassis refitted with enhanced thermal protection and an internal fire suppression cistern. The heavier protection comes at the cost of weapon hardpoints, which are entirely absent on this variant. Suited to fire response and atmospheric emergencies.

| Stat | Value |
|---|---|
| Max integrity | 250 |
| Max operating temperature | 65,000 K |
| Cargo capacity | (inherits Ripley) |

---

### Gygax

A lightweight security exosuit popular among corporate and private security contractors. The Gygax emphasizes mobility, with a faster step rate than heavier combat frames, and carries a special leg actuator overload mode that temporarily increases movement speed at the cost of accelerated energy consumption.

| Stat | Value |
|---|---|
| Max integrity | 250 |
| Deflection chance | 15% |
| Max operating temperature | 25,000 K |
| Step rate | 3 ticks/step |

---

### Durand

A heavier combat exosuit originally designed for engagement with hostile alien lifeforms. Slower than the Gygax but significantly more durable and better armored. Equipped with a defence mode that increases damage mitigation at the cost of mobility. Fitted with infrared illumination.

| Stat | Value |
|---|---|
| Max integrity | 300 |
| Deflection chance | 20% |
| Max operating temperature | 30,000 K |
| Step rate | 4 ticks/step |
| Minimum damage dealt (melee) | 15 |

---

### Marauder

A heavy-duty combat exosuit developed as a successor to the Durand. Rarely found among civilian populations. Requires Central Command special operations access to operate. Equipped with optional smoke dispenser, zoom optics, and thruster systems. Carries the most equipment slots of any standard chassis.

| Stat | Value |
|---|---|
| Max integrity | 350 |
| Deflection chance | 25% |
| Max operating temperature | 60,000 K |
| Step rate | 5 ticks/step |
| Access required | CentCom Special Operations |

---

### Odysseus

A medical exosuit produced by Vey-Med. The Odysseus is the most fragile chassis available but the fastest, designed for rapid response and patient transport rather than combat. Automatically equips the pilot with an integrated medical HUD upon boarding. The suit has no weapon hardpoints.

| Stat | Value |
|---|---|
| Max integrity | 70 |
| Deflection chance | 15% |
| Max operating temperature | 15,000 K |
| Step rate | 2 ticks/step |
| Special | Integrated medical HUD for pilot |

---

## Operation

### Boarding and Exiting

To board an exosuit, interact with the cockpit access panel on the front of the chassis. The suit seals around the pilot and begins consuming power. To exit, use the eject control on the internal panel. If the suit loses power entirely, the pilot may be unable to exit without external assistance; a crowbar applied to the cockpit panel from outside can force the hatch open.

### Power Management

Exosuits draw power from an internal cell on every movement step and when active equipment is used. Heavier suits drain more per step. Cells can be swapped by opening the maintenance panel with a screwdriver, removing the depleted cell, and inserting a charged replacement.

### Temperature Limits

Each chassis has a maximum safe operating temperature. Exceeding this threshold begins damaging the suit and can ultimately destroy it. Atmospherics emergencies and plasma fires are the primary concern. The Firefighter and Marauder have substantially higher thermal tolerances for hazardous operations.

### Deflection

Combat and medical chassis have a chance to partially deflect incoming damage. The Marauder has the highest deflection rate at 25%. The Ripley and Odysseus have no deflection mechanic.

---

## Equipment Slots

Exosuits accept modular equipment divided by slot category. Each chassis has a fixed number of slots per category; exceeding the limit requires removing an existing piece of equipment.

| Slot type | Description |
|---|---|
| Hull | Structural and passive modifications (armor plating, hull reinforcement) |
| Weapon | Active offensive equipment (drills, clamps, cannons) |
| Utility | Support tools (medical equipment, scanners, extinguishers) |
| Universal | Equipment compatible with any slot category |
| Special | Chassis-specific subsystems (overload systems, thrusters) |

Equipment is fabricated at the exosuit fabricator under the Robotics research tier or obtained from supply packs. Installing equipment requires placing it in the appropriate slot via the suit's equipment panel.

---

## Construction

Exosuits are assembled at the exosuit fabricator in the robotics lab. Construction requires:

1. Researching the target chassis type in the techweb.
2. Printing the required frame components from the fabricator.
3. Assembling the frame in sequence: chassis, then internal components (hull, actuator, armor, gas system, electrical).
4. Installing a power cell.
5. Attaching any desired modular equipment.

The Odysseus and Marauder require advanced research tiers before their frame components become available. The Marauder additionally requires Central Command authorization to operate once built.

---

*See also: [Research System](ResearchSystem.md), [Cyborgs](Cyborgs.md)*
