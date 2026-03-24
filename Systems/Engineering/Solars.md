[ARGUS Station Database](../../README.md) > [Systems](../README.md) > [Engineering](README.md) > Solar Arrays

# Solar Arrays

The solar arrays are a distributed backup power system that generates electrical power from the local sun, independent of the primary engine.

---

## Overview

Four independent solar arrays serve the station, each comprising a field of panels, a solar tracker, and a dedicated SMES unit. Each array is wired to its own isolated power grid and must not share a grid with any other array; conflicting array controllers cause both arrays to cease tracking and stop generating power.

Output per array fluctuates between 0 and 90,000 W as station rotation periodically blocks sunlight. The SMES units buffer this variation. With all four arrays active and their SMES units delivering power, the combined output is sufficient to sustain life support, the AI core, and other critical station systems.

---

## Arrays

| Array | Location |
|---|---|
| Fore Port | Third deck maintenance, west of the AI satellite |
| Fore Starboard | Third deck maintenance, east of the particle accelerator |
| Aft Port | Third deck maintenance, west of the bridge |
| Aft Starboard | Third deck maintenance, east of the bridge |

Three of the four arrays are connected to the station network at the start of each shift. The Fore Starboard array requires wiring to be connected.

---

## Wiring

### Required equipment

Cable coils (yellow recommended), a vacuum-capable suit with internals supply, and insulated gloves.

### Procedure

Hold a cable coil in hand. Press an adjacent section to run a wire from the current position toward that section; the wire extends in the direction of the press. A small junction point appears at the centre of the section being wired. When extending wire across a section, press the junction point to create a straight pass-through rather than a branch.

Connect each solar panel and the solar tracker to the wire already leading back into the station. Avoid creating unnecessary junction points; excess junctions can cause power loss on the line.

The array's existing pre-connected panels demonstrate the correct wiring geometry for their segment. New panels are wired the same way, using curves to route through corners rather than knotted junctions.

> [!WARNING]
> Never wire two solar arrays into the same power grid. Each array's auto-tracking controller conflicts with others sharing its network, causing both controllers to fail and both arrays to stop generating power.

---

## Calibration

Each solar array includes a **solar tracker** that maintains automatic alignment with the local sun. Opening the solar array control console and pressing the **Auto** button activates automatic calibration. Once active and correctly wired, the tracker adjusts panel angle continuously without further operator input.

---

## SMES Configuration

Each array connects to a dedicated SMES unit that buffers the fluctuating output and holds reserve power for engine failure contingencies.

Recommended baseline settings:

| Setting | Value |
|---|---|
| Input | 90,000 W, AUTO |
| Output | 40,000 W, OFFLINE |

With output set to OFFLINE, the SMES charges as a reserve. If the primary engine fails, output is switched to ONLINE to supply the station. The AI can perform this switch remotely if the SMES RCON wire is intact.

See [SMES](SMES.md) for configuration and maintenance procedures.

---

## Maintenance

### Wiring damage

Damaged or missing wire segments are replaced by running new cable along the affected path using a cable coil.

### Panel damage

Each solar panel is protected by a double layer of glass sheets. If the protective glass is damaged, crowbar the broken glass out and install replacement glass sheets. If the panel assembly itself is destroyed, obtain a replacement solar panel assembly from Engineering storage or from Cargo, wrench it into the correct position, and add the two glass sheet layers.

### Tracker damage

If the solar tracker is destroyed, replace the assembly: obtain a new solar panel assembly, wrench it into the tracker position, insert a solar tracker circuit board, and add two glass sheets. Each array supports only one tracker; installing additional trackers on the same array causes conflicts.

### SMES damage

SMES units are expensive to replace. See [SMES](SMES.md) for deconstruction and reconstruction procedures.
