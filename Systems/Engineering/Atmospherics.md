[ARGUS Station Database](../../README.md) > [Systems](../README.md) > [Engineering](README.md) > Atmospherics

# Atmospherics

The station atmospheric system maintains breathable air across all pressurized areas through a network of pipes, vents, scrubbers, and gas storage. This document covers gas types and properties, standard air composition, pressure and temperature hazards, fire mechanics, and tank behavior.

---

## Gas Types

| Gas | Specific Heat | Molar Mass | Properties |
|---|---|---|---|
| Oxygen (O2) | 20 J/(mol·K) | 0.032 kg/mol | Oxidizer; required for respiration and fire |
| Nitrogen (N2) | 20 J/(mol·K) | 0.028 kg/mol | Inert; primary atmospheric buffer |
| Carbon Dioxide (CO2) | 30 J/(mol·K) | 0.044 kg/mol | Contaminant; scrubbers filter by default |
| Phoron | 200 J/(mol·K) | 0.405 kg/mol | Fuel; contaminant; extremely flammable; visible in air above 0.7 moles |
| Nitrous Oxide (N2O) | 40 J/(mol·K) | 0.044 kg/mol | Oxidizer; sedative at breathing concentrations |
| Methane (CH4) | 34 J/(mol·K) | 0.016 kg/mol | Fuel; contaminant; scrubbers filter by default |
| Volatile Fuel | 253 J/(mol·K) | 0.114 kg/mol | Fuel; high-energy combustible |

**Standard breathable atmosphere:** 21% oxygen, 79% nitrogen at 101.325 kPa (one atmosphere) and approximately 20°C (293.15 K). This composition sustains respiration and does not support spontaneous combustion.

---

## Pressure Hazards

Pressure outside the normal range causes physical damage to unprotected personnel.

| Threshold | Value | Effect |
|---|---|---|
| Low pressure warning | 50 kPa | Environmental warning; suits recommended |
| Low pressure hazard | 20 kPa | Active damage; unprotected personnel take 2 brute per tick |
| High pressure warning | 325 kPa | Environmental warning |
| High pressure hazard | 550 kPa | Active damage; damage scales with pressure: (pressure / 550) × 4, maximum 4 per tick |

Standard space suits and hardsuits provide full protection against vacuum and high-pressure environments.

**Volume reference:** Standard atmospheric cells hold 2,500 liters. At standard conditions this corresponds to approximately 102 moles of gas per cell (roughly 21.5 moles O2 and 81 moles N2).

---

## Temperature Hazards

The optimal body temperature is 310.15 K (37°C). Deviations from this cause progressive thermal damage.

| Threshold | Temperature | Condition |
|---|---|---|
| Cold damage begins | 260.15 K (-13°C) | Crew take thermal damage from cold exposure |
| Heat damage begins | 360.15 K (87°C) | Crew take thermal damage from heat exposure |
| Fire resistance limit (carbon) | 473.15 K (200°C) | Above this, standard fire protection gear loses effectiveness |

Thermal damage coefficient is 1.5 per tick. The body self-regulates toward optimal temperature at approximately 8 K per tick when environmental temperature is within a safe range. Extreme cold or hot environments drive temperature change at a rate six times faster than normal recovery.

Firesuits and hardsuits provide substantial thermal protection. Fire stacks accumulate separately; above 25 stacks even fire protection degrades.

---

## Fire Mechanics

Fire on the station requires three conditions simultaneously: an oxidizer (oxygen or nitrous oxide), fuel (phoron, methane, or volatile fuel), and sufficient temperature.

**Phoron ignition thresholds:**
- Minimum ignition temperature in an enclosed space: 399.15 K (126°C)
- Auto-ignition temperature in open air: 519.15 K (246°C)

**Combustion ratio:** Phoron fires consume approximately 3 moles of oxidizer per 2 moles of fuel. Fires sustain until one reactant is exhausted or temperature drops below ignition threshold.

**Fire stacks:** Burning personnel accumulate fire stacks (minimum -20, maximum 25). Personnel take 4 brute damage per tick while burning. Rolling in the floor or using fire extinguishers reduces stacks. Above 20 stacks, standard fire suits begin losing effectiveness.

**Suppression:** Carbon dioxide does not support combustion and displaces oxygen when released in quantity. CO2 flooding from fire suppression systems is the primary approach for containing compartment fires. Phoron fires produce extreme heat rapidly; immediate compartment isolation is preferable to attempting manual suppression.

---

## Gas Canister Behavior

Portable gas canisters are standard pressurized containers used throughout the station.

| Threshold | Pressure | Effect |
|---|---|---|
| Leak threshold | 30 atm (3,040 kPa) | Canister begins leaking gas |
| Rupture threshold | 40 atm (4,053 kPa) | Canister empties entirely |
| Fragment threshold | 50 atm (5,066 kPa) | Canister explodes, 3×3 tile blast |
| Fragment scaling | +10 atm above fragment threshold | Blast radius increases by 1 tile per 10 atm |

Standard supply storage pressures: nitrogen 90,000 kPa, oxygen 40,000 kPa, CO2 25,000 kPa, phoron 25,000 kPa, N2O 10,000 kPa, methane 5,000 kPa.

---

## Heat Transfer

Gas temperature equalizes between tiles based on surface conductivity coefficients. Open floors transfer heat efficiently (0.4). Walls and closed doors conduct negligibly (0.0). Windows conduct at 0.1. Space tiles radiate heat at 0.2. In practice, a sealed room retains heat far longer than an open area, which is relevant both for fire containment and for emergency heating scenarios.

---

*See also: [Atmospherics Equipment](AtmosEquipment.md), [Atmospheric Emergencies](AtmosEmergencies.md), [Supermatter Engine](SupermatterEngine.md)*
