[ARGUS Station Database](../../README.md) > [Systems](../README.md) > [Engineering](README.md) > Atmospheric Emergencies

# Atmospheric Emergencies

Response procedures for the four categories of atmospheric emergency: fire, breach, toxic contamination, and gas mix failure. For hazard thresholds and component reference, see [Atmospherics](Atmospherics.md) and [Atmospherics Equipment](AtmosEquipment.md).

---

## Fire

**Assessment:** A fire is confirmed when an area shows elevated temperature, visible plasma/methane/fuel combustion, or crew reporting burning. Fire alarm systems trigger automatically when temperature exceeds safe thresholds.

**Containment priority:** Seal the compartment before attempting suppression. Closing blast doors and airlocks prevents fire from spreading to adjacent areas and cuts off fresh oxygen supply. A sealed phoron fire will self-extinguish when oxidizer is exhausted.

**Active suppression:** Fire suppression systems release CO2 into the affected compartment. CO2 displaces oxygen, suppressing combustion without itself being toxic to personnel who have evacuated. Engineering staff using CO2 canisters via outlet injectors can manually flood small areas.

**Burning personnel:** Crew on fire should be treated with a fire extinguisher or by entering a pressurized area with fire suppression foam. Fire stacks reduce naturally in temperate environments or rapidly with active suppression. Crew with 20+ fire stacks have likely exceeded fire suit protection; immediate medical attention for burn damage is required.

**Phoron fire hazard:** Phoron burns at high temperature and generates significant heat. Even a small phoron fire in a confined space can rapidly exceed hardsuit thermal tolerances. Priority is always compartment isolation; do not send personnel into active phoron fires without pressure suit protection and only when strictly necessary.

**Post-fire ventilation:** After suppression, the affected area contains depleted air (high CO2, low O2). Scrubbers in siphon mode clear the area; vents restore breathable air once CO2 levels normalize. Do not return personnel to the area until atmospheric readouts confirm safe O2 and acceptable CO2 concentrations.

---

## Breach

**Assessment:** A breach is confirmed by pressure alerts in affected areas, visible gaps in hull or windows, or crewmembers reporting loss of atmosphere. Low pressure warnings trigger at 50 kPa; the hazard threshold is 20 kPa (approximately 20% standard pressure).

**Immediate response:** All personnel in the affected area should don emergency breath masks at minimum; full space suits or hardsuits provide complete protection from vacuum exposure. Do not remain in a low-pressure area without respiratory protection.

**Sealing the breach:** Standard repair materials (metal rods, floor tiles, plasteel) can restore hull integrity. Windows can be replaced from emergency lockers. The priority sequence is: evacuate unprotected personnel, seal the breach, then restore atmosphere.

**Atmosphere restoration:** After sealing, set area vents to Release mode with standard pressure target (101.325 kPa). Gas supply from the atmospheric distribution network will refill the area. Verify scrubbers are in standard scrubbing mode (CO2 and phoron filtered) before returning personnel without suits.

**Space exposure:** Personnel in vacuum without protection rapidly lose air supply and begin suffering oxygen damage within seconds. Rescue is possible if the individual is brought into a pressurized area promptly; oxygen damage is treatable. Pressure damage from vacuum exposure is in the brute category.

---

## Toxic Contamination

**Assessment:** Toxic gas events include phoron leaks from piping failures, N2O (laughing gas) releases, or methane accumulation. Atmospheric monitors and scrubber alarms are the primary detection systems.

**Phoron leak:** Phoron is visible in quantities above approximately 0.7 moles per tile. It is not immediately toxic to breathe in small amounts but poses extreme fire risk. Scrubbers with phoron filtering enabled will clear it; if scrubbers are offline, evacuate the area and seal it until repairs are made. Do not introduce ignition sources into a phoron-contaminated environment.

**N2O exposure:** Nitrous oxide at breathing concentrations causes sedation and incapacitation. Affected personnel appear confused and unable to stand. Move them to a clean-air environment; recovery is spontaneous once clean air is restored. N2O is otherwise non-toxic.

**Methane:** Flammable but non-toxic directly. Treat as a fire precursor; scrubbers clear it. Evacuate and seal against ignition sources.

**Decontamination procedure:** Activate scrubber panic siphon in the affected area to rapidly evacuate all atmosphere. Restore clean air from distribution supply. Verify atmospheric readout is within normal parameters before permitting re-entry without respiratory protection.

---

## Gas Mix Failure

**Assessment:** An area may receive incorrect atmospheric composition from pipe network misconfiguration, damage to gas supply lines, or cross-contamination between pipe loops.

**Identifying the failure:** Atmospheric readouts on engineering monitors show per-gas concentrations. The target readings for habitable areas are approximately 21% O2 and 79% N2. Any significant deviation (excess CO2, presence of phoron or methane, O2 below 18% or above 30%) indicates a mix problem.

**Oxygen deficiency:** Low O2 causes suffocation. Crew in O2-deficient areas should use emergency oxygen masks from emergency lockers immediately. Fix: ensure O2 supply is connected and functioning; check that scrubbers are not stripping O2 (O2 should not be in the scrubber filter list).

**Oxygen excess:** High O2 concentration dramatically lowers the ignition temperature for any fuel present and accelerates fire spread. Scrubbers set to filter O2 can correct this; if the cause is an O2 supply misconfiguration, trace and correct the pipe connection.

**N2 supply failure:** Loss of nitrogen allows O2 concentration to rise proportionally as nitrogen is not replenished. Restore N2 supply connections and verify mixer ratios if using mixed-gas injection.

**Restoring normal mix:** Once the source of contamination or deficiency is corrected, siphon out the existing atmosphere and refill from verified clean supply. This is faster than attempting to titrate toward target concentrations while the problem persists.

---

*See also: [Atmospherics](Atmospherics.md), [Atmospherics Equipment](AtmosEquipment.md), [Supermatter Engine](SupermatterEngine.md)*
