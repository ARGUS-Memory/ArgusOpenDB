[ARGUS Station Database](../../README.md) > [Systems](../README.md) > [Engineering](README.md) > SMES

# SMES

A Superconducting Magnetic Energy Storage unit (SMES) is a power storage and conditioning device that accepts input from a power source, accumulates charge in a magnetic field, and outputs regulated power to the downstream distribution network.

---

## Configuration

The SMES interface opens by pressing the unit with an empty hand. The same controls are accessible remotely through an RCON console if the unit has been assigned an RCON tag.

### Input

The input setting governs how much power the unit draws from the upstream network. The maximum allowable input rate is set by the coil configuration and can be raised by adding higher-grade coils. Two modes are available:

| Mode | Behaviour |
|---|---|
| OFF | No power is drawn from the upstream network |
| AUTO | The unit charges from whatever power is available, up to the configured cap |

If the configured input rate exceeds the available supply, the unit enters a **Partially Charging** state and continues to charge at the reduced available rate.

### Output

The output setting governs how much power the unit delivers to the downstream network. The output cap is also raised by upgrading the coils. Two modes are available:

| Mode | Behaviour |
|---|---|
| OFFLINE | No power is delivered to the downstream network |
| ONLINE | Power is delivered at the configured rate |

### RCON Tagging

Assigning an RCON tag allows the unit to be operated from a Remote Control console. Tags must be unique across all SMES units on the network. Applying the multitool to the unit opens the tag entry interface. Setting the tag to `NO_TAG` disables RCON operation.

---

## Construction

### Required materials

| Item | Quantity |
|---|---|
| Metal sheets | 5 |
| Cable coil (full) | 2 |
| SMES circuit board | 1 |
| Superconducting magnetic coil | 1 (minimum) |

The circuit board is available from the Research department or salvaged from an existing unit. Coils are available from Cargo or salvaged from existing units. Up to 6 coils total can be installed.

### Assembly steps

1. Construct a machine frame from metal sheets.
2. Apply a cable coil to the frame.
3. Optionally lay wire under the frame position -- the SMES delivers output into this wire.
4. Insert the SMES circuit board into the wired frame.
5. Add 30 pieces of cable (one full coil).
6. Insert one superconducting magnetic coil.
7. Apply a screwdriver to finalise the unit.

### Terminal

A new unit starts without a terminal. Without a terminal the unit cannot charge or discharge. Terminal installation:

1. Open the SMES interface and set both input and output to OFF.
2. Apply a screwdriver to open the access panel.
3. Apply a cable coil to add the terminal (10 pieces of cable required). Applying wirecutters removes the terminal if a mistake is made.
4. Apply a screwdriver to close the panel.

---

## Upgrading

Up to 5 additional coils can be installed after initial construction, for a maximum of 6 total. Three coil types are available; 2 of each type are stored in the Engineering hard storage locker.

| Coil type | Effect |
|---|---|
| **Superconductive Capacitance Coil** | Greatly increases maximum stored energy |
| **Superconductive Transference Coil** | Greatly increases maximum input and output rate |
| **Superconductive Magnetic Coil** | Moderately increases both storage and transfer rate |

### Upgrade procedure

> [!CAUTION]
> Modifying a charged SMES without disabling the failsafes risks a catastrophic failure event. See [Failure Modes](#failure-modes) before proceeding.

1. Discharge the unit fully, or disable the failsafes (see [Wiring](#wiring)).
2. Open the SMES interface and set both input and output to OFF.
3. Apply a screwdriver to open the access panel.
4. Insert the additional coil or coils.
5. If failsafes were disabled, re-enable them before closing the panel.
6. Apply a screwdriver to close the panel.

---

## Deconstruction

### Required tools

Screwdriver, crowbar, wirecutters, welding tool, wrench. Insulated gloves are strongly recommended. A multitool is required only if disabling the failsafes.

### Steps

1. Ensure the unit is fully discharged, or disable the failsafes first.
2. Open the SMES interface and set both input and output to OFF.
3. Apply a screwdriver to open the access panel.
4. Apply wirecutters to remove the terminal, if present.
5. Apply a crowbar to begin removing internal components. A basic unit takes approximately 10 seconds; a fully loaded 6-coil unit takes up to 60 seconds.
6. Apply wirecutters to remove the cable from the resulting machine frame.
7. Apply a wrench to dismantle the machine frame.

---

## Wiring

The SMES access panel exposes 5 wires. Wire colours are randomised each shift but are consistent across all SMES units on the station. Open the panel with a screwdriver, then press the unit with an empty hand to open the wiring interface.

| Wire | Cut effect | Pulse effect |
|---|---|---|
| **Input** | Stops all power input | Temporarily disables input |
| **Output** | Stops all power output | Temporarily disables output |
| **RCON** | Disables remote control and AI access | No effect |
| **Failsafes** | Allows modification while charged (see below) | No effect |
| **Grounding** | Triggers rapid charge dissipation to the output network | Triggers the same dissipation |

Cutting the grounding wire discharges the unit rapidly. The released energy can overload or destroy APCs connected to the output network. Mending the grounding wire stops the dissipation. This is similar to a failure event but with reduced risk to personnel.

---

## Failure Modes

When the failsafes are disabled and components are added or removed while the unit is charged, one or more failure events may occur. The probability of each event scales with the current charge percentage.

| Event | Trigger threshold | Effect |
|---|---|---|
| **Discharge** | Always | All remaining stored charge is lost |
| **Sparks** | Always | Sparks emit from the unit; may ignite nearby flammables |
| **Electrocution** | Always | Shocks the operator; insulated gloves reduce but do not eliminate risk; above 60% charge the shock is lethal even with gloves |
| **EMP** | Above 15% charge | Electromagnetic pulse disables nearby electronics; range and intensity scale with stored power |
| **APC Overload** | Above 35% charge | Overloads lighting circuits in several APCs on the output network |
| **APC Failure** | Above 35% charge | Destroys several APCs on the output network |
| **Magnetic Containment Failure** | Above 60% charge | Stored charge releases as a violent explosion after 30 to 60 seconds, destroying the unit and breaching the surrounding structure |

Any SMES or other device between the failing unit and the APCs provides isolation and prevents overload propagation to that segment of the network.
