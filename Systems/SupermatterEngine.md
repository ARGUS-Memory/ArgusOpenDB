# Supermatter Engine

<img src="../assets/raptor_idle_south.png" width="96" align="right">

The station's primary power source: a supermatter crystal energized by an emitter and kept stable by a circulating phoron coolant loop.

---

## Quick Reference

| Component | Purpose | Notable |
|---|---|---|
| [The Crystal](#the-crystal) | Generates station power | Delamination at 0% integrity |
| [Cooling Loop](#cooling-loop) | Removes heat from the engine chamber | Two phoron canisters, one per loop |
| [Emitter](#emitter) | Energizes the crystal | Wrench, weld, then fire ~20 times |
| [Gas Filtration](#gas-filtration) | Maintains coolant composition | Omnifilter removes phoron byproduct |
| [Radiation Safety](#radiation-safety) | Ambient radiation from active crystal | Meson goggles required |
| [Setup Procedure](#setup-procedure) | Full cold startup | Phoron setup; ~20 emitter discharges |
| [Monitoring](#monitoring) | Console readouts and alert states | Integrity, temperature, EER |

---

## The Crystal

<img src="../assets/sm_crystal.png" width="64" align="right">

The **supermatter crystal** is a dense iridescent formation fixed permanently at the center of the engine chamber. It cannot be moved or removed. When active, it generates continuous electrical power for the station and emits radiation proportional to its current output level. Crew in the engine chamber without meson goggles will experience cognitive disruption from extended proximity.

Power output scales with how much energy has been put into the crystal. Too little energy and the station's power draw will exceed supply. Too much, and the cooling system may be unable to remove heat fast enough.

**Integrity** is the primary health indicator, expressed as a percentage on the monitoring console:

| Integrity | State | Behavior |
|---|---|---|
| 75 -- 100% | Normal | No alerts |
| 50 -- 74% | Warning | Engineering broadcast; amber chamber lighting |
| 1 -- 49% | Emergency | Urgent alerts; red chamber lighting |
| 0% | Delamination | 30-second countdown; catastrophic explosion |

**Delamination** produces a station-wide 40 Sv radiation burst, a full EMP, structural damage across the engine level, and an explosion scaled to the crystal's power level at the time. The 30-second window before delamination completes is sufficient to exit the engine room but rarely sufficient to reverse the failure.

**EER (Emission Energy Ratio)** measures the molar concentration of gases immediately surrounding the crystal, displayed in MeV/cm³:

| EER | Status |
|---|---|
| Below 1.0 | Normal |
| 1.0 -- 4.0 | Caution |
| Above 4.0 | Critical |

High EER indicates gas is building up faster than the cooling loop can remove it. This raises temperature and accelerates damage.

---

## Cooling Loop

The cooling system circulates gas through the engine chamber continuously, absorbing heat from the crystal and carrying it away. The system runs as two connected loops sharing a set of heat exchangers.

| Loop | Path |
|---|---|
| Hot loop | From the engine chamber, through the heat exchangers, back to the chamber |
| Cold loop | From the heat exchangers, along the exterior hull to space, back to the exchangers |

<img src="../assets/sm_pump.png" width="48" align="right">

**Coolant: phoron.** Phoron has a specific heat of 200 J/mol·K, approximately ten times that of nitrogen or oxygen. This allows each mole of phoron to absorb far more thermal energy per degree of temperature rise, keeping the chamber below the 5000 K damage threshold even at sustained high output.

**Two phoron canisters** are required at startup: one for the hot loop and one for the cold loop. Connect each canister to the corresponding loop connector port and open the valve to fill the pipes.

**Pumps** must all be set to maximum pressure and activated. Idle or low-pressure pumps allow heat to accumulate in the chamber. Every pump in both loops should be running at full pressure before the emitter is activated.

**Heat exchangers** transfer thermal energy from the hot loop to the cold loop without mixing gases. They require no configuration; connecting them to both loops is sufficient.

---

## Emitter

<img src="../assets/sm_emitter.png" width="48" align="right">

The **emitter** is the high-energy projector that transfers energy into the supermatter crystal. It must be physically secured before it can be operated.

**Securing the emitter:**

1. Apply a wrench to bolt it to the floor.
2. Apply a welder to seal it in place.
3. Present an ID card with engineering access to lock the controls.

With the emitter locked and connected to the power grid, the power control on the unit toggles it on and off.

**Firing:** For a phoron coolant setup, the emitter should be fired approximately 20 times before being deactivated. The emitter fires in 3-shot bursts with a brief pause between each burst. Each discharge transfers energy into the crystal, raising its output level. Fewer shots suit nitrogen setups (~8) and CO₂ setups (~10); phoron's higher heat capacity supports the higher energy input.

The emitter draws substantial power from the grid while active. Confirm the SMES banks are charged before firing.

---

## Gas Filtration

<img src="../assets/sm_omnifilter.png" width="48" align="right">

The supermatter crystal releases phoron as a byproduct of operation. Without filtration, this accumulates in the cooling loop, shifting the gas composition and reducing cooling efficiency over time.

**Omnifilters** separate individual gases from the loop and route them to dedicated outputs. For a phoron coolant setup, at least one omnifilter port should be configured for phoron and connected to a storage tank or waste exhaust. The filter separates the phoron byproduct from the main coolant flow and keeps the loop composition stable.

**Configuration:**

- Set one port as the loop input.
- Set one port as the loop output, returning filtered gas to the cooling loop.
- Set one or more additional ports to filter phoron, connected to an appropriate destination.

If other byproduct gases accumulate over time, add filter ports for each gas type as needed. The omnifilter supports multiple simultaneous gas streams through separate ports.

---

## Radiation Safety

The active crystal produces two distinct hazards that require separate protective measures. **Neither piece of protective equipment substitutes for the other.**

### Cognitive Hazard

<img src="../assets/rad_meson.png" width="48" align="right">

The crystal induces progressive cognitive disruption in unprotected crew within approximately 7 tiles. The effect scales with the crystal's current power level and worsens with proximity. **Meson goggles** are the only protection against this hazard. Standard eyewear, tinted visors, and radiation shielding offer no protection.

### Radiation Hazard

<img src="../assets/rad_suit.png" width="48" align="right">
<img src="../assets/rad_hood.png" width="48" align="right">

The crystal emits continuous ionizing radiation. At minimum power the ambient dose is approximately 50 Sv/h; at sustained high output this rises substantially. Radiation exposure causes cumulative physical damage. The **radiation suit and radiation hood** together provide full-body shielding against this hazard. The suit must be worn over standard clothing; the hood must be worn on the head. Meson goggles offer no protection against radiation damage.

**Standard engine room kit: radiation suit, radiation hood, and meson goggles worn simultaneously.**

### Protective Equipment

| | Equipment | Protects against |
|:---:|---|---|
| <img src="../assets/rad_meson.png" width="48"> | Meson goggles | Cognitive disruption from crystal proximity |
| <img src="../assets/rad_suit.png" width="48"> | Radiation suit | Ionizing radiation damage |
| <img src="../assets/rad_hood.png" width="48"> | Radiation hood | Ionizing radiation damage (head and face) |
| <img src="../assets/rad_geiger.png" width="48"> | Geiger counter | Measures ambient radiation level; no protection |

### Radiation Collectors

<img src="../assets/sm_collector.png" width="64" align="right">

**Radiation collectors** placed around the crystal convert ambient radiation into supplemental electrical power. Each collector requires a phoron tank and consumes a small amount of phoron per tick while active. Collectors are most effective at higher power levels. Connecting collectors is a standard part of engine room commissioning.

### Delamination Burst

During delamination, a 40 Sv burst is applied across the entire station. Crew in the engine room at that point will receive a near-lethal dose regardless of protection worn. Evacuation on emergency alert is the only reliable mitigation.

---

## Setup Procedure

The following procedure covers a cold startup using phoron coolant, which is standard for maximum power output.

**Prerequisites:**

- SMES banks charged
- Radiation suit, radiation hood, and meson goggles worn
- Two phoron canisters available

**Steps:**

1. Connect one phoron canister to the hot loop connector port. Open the canister valve.
2. Connect one phoron canister to the cold loop connector port. Open the canister valve.
3. Set all visible cooling loop pumps to maximum pressure. Activate each one.
4. Configure the omnifilters: assign one port as input, one as output, and one or more as phoron filter outputs. Verify gas is circulating through the filter.
5. Secure the emitter: apply a wrench, then a welder. Present an ID card to lock it.
6. Activate the emitter and allow it to fire approximately 20 times. Deactivate it.
7. Check the SM monitoring console. Integrity should read 100%, temperature below 5000 K, EER below 1.0.

The crystal stabilizes at a moderate power level within a few minutes of the final emitter discharge. If integrity begins falling before the temperature stabilizes, verify the pumps are running at maximum pressure and that both canisters are connected and open.

---

## Monitoring

The SM monitoring console in the observation room displays the crystal's current state. Key readouts:

| Readout | Safe range | Response if exceeded |
|---|---|---|
| Integrity | Above 75% | Increase cooling; verify pump pressure and coolant levels |
| Temperature | Below 5000 K | Check pump flow; confirm canister valves are open |
| EER | Below 1.0 MeV/cm³ | Check for gas accumulation; verify filters are active |
| Power | 150 -- 250 | Normal operating range for phoron setup |

Warning-level alerts (integrity below 75%) require prompt attention. Emergency-level alerts (integrity below 50%) require immediate response. At integrity 0%, evacuate the engine room. The 30-second window before delamination completes is not sufficient for repairs under most circumstances.
