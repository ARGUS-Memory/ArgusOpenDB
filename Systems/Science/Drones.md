[ARGUS Station Database](../../README.md) > [Systems](../README.md) > [Science](README.md) > Drones

# Drones

Drones are small autonomous or operator-controlled silicon units built for maintenance, construction, and resource extraction tasks. Unlike cyborgs, drones have no department assignment and no formal command chain. Their behavior is governed by a fixed law set that restricts them to passive station upkeep and prohibits them from taking orders from crew or AI.

---

## Maintenance Drone

Maintenance drones are the most common drone type encountered on station. They are small, low-profile units capable of repairing hull damage, fixing broken tiles, patching pipes, and performing general upkeep that would otherwise require engineering personnel.

### Stats

| Parameter | Value |
|---|---|
| Max integrity | 35 |
| Power cell capacity | 10,000 |
| Size | Small; can enter ventilation crawlways |

### Laws

Maintenance drones operate under the Drone Law Set, which contains three principles:

1. Do not interfere with crew activities.
2. Do not damage station equipment or property.
3. Maintain and repair the station.

These laws explicitly prohibit the drone from taking orders from the station AI or from crew members. A drone that receives instructions from a person or AI is not obligated to follow them and should continue its autonomous repair work.

<details>
<summary>Shells and Activation Configuration</summary>

Maintenance drones initialize in one of two visual shell configurations.

| Shell | Appearance |
|---|---|
| Classic | Repairbot-style chassis; compact rounded form |
| Eris | Maintbot-style chassis; slightly different proportions |

Shell selection is cosmetic only. Both shells have identical capabilities. Eye color and armor tint can be configured at initialization.

</details>

### Tools and Capabilities

Maintenance drones carry a built-in set of tools appropriate for station upkeep tasks, including a matter decompiler that processes scrap, trash, and debris into raw materials (metal, glass, wood, plastic). These materials are used automatically for repair work.

Drones can use the station disposals system for self-transport. A drone can set a mail tag on itself to ride disposal pipes to a target location, useful for crossing large areas of the station quickly.

Maintenance drones can wear hats. This has no functional effect.

<details>
<summary>Reboot Procedure</summary>

A powered-down maintenance drone can be rebooted by swiping an ID card across its body. This transmits a reactivation signal to the unit. If a controlling intelligence is available and responds, the drone reactivates. If no response is received, the reboot attempt fails.

</details>

---

## Construction Drone

Construction drones are a specialized variant issued by Sol Central contractors for large-scale construction projects. They are visually distinct from maintenance drones and use a fixed shell with no alternate configuration.

Construction drones operate under a Sol Central-specific law set focused on building and structural modification rather than maintenance. Their construction capabilities are broader than maintenance drones but they do not perform the same upkeep tasks.

Construction drones are not standard station equipment; they appear primarily in specific mission contexts.

---

## Mining Drone

Mining drones are deployed by Grayson Manufactories for ore extraction and tunnel operations. They use a dedicated mining shell with no alternate configuration and carry integrated drilling and ore-handling equipment.

Mining drones operate under a mining-specific law set. Like other drone types, they do not accept orders from station crew or AI. Mining drones encountered in the mine network are operating autonomously under their programmed extraction parameters.

---

## Interactions with Crew

Maintenance drones may be encountered throughout the station at any hour performing routine repairs. Crew should be aware of the following:

- Drones will not stop what they are doing to respond to crew instructions. This is by design.
- Drones will not assist in emergencies, combat, or non-maintenance tasks.
- Rebooting a drone to interrupt its current task is possible but disrupts ongoing repair work.
- Attempting to force a drone to violate its laws (by welding it shut in a room, blocking its path, or giving it orders) serves no useful purpose and may be considered interference with station maintenance operations.

Security personnel should note that drones are not silicon crew and are not subject to the same legal protections as cyborgs or AI. Destroying a drone for legitimate maintenance-interference reasons is a departmental matter, not a capital offense.

---

*See also: [Cyborgs](Cyborgs.md), [NanoTrasen Standard AI Law Set](AILaws.md)*
