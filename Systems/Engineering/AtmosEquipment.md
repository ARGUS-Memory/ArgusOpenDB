[ARGUS Station Database](../../README.md) > [Systems](../README.md) > [Engineering](README.md) > Atmospherics Equipment

# Atmospherics Equipment

Reference for all pipe network components, portable atmospheric equipment, and the configuration parameters for vents and scrubbers. For gas properties and hazard thresholds, see [Atmospherics](Atmospherics.md).

---

## Binary Devices

Binary devices connect two pipe segments and regulate flow between them.

| Component | Power Draw | Max Pressure | Notes |
|---|---|---|---|
| Gas Pump | 7,500 W | 15,000 kPa | Moves gas at a target output pressure (default 101.325 kPa). Primary workhorse for moving gas between pipe loops. |
| Volume Pump | 15,000 W | 9,000 kPa | Moves gas by volume per second (default 20 L/s) rather than by pressure target. 4% of transferred gas leaks into the environment. |
| Pressure Regulator (Passive Gate) | None | 15,000 kPa | One-way valve. Allows gas to flow only when input pressure exceeds the set threshold. No power required. Flow rate: 500 L/s. |
| Pipe Turbine | None | -- | Converts pressure differential to electricity. Passive; used in TEG setups. |
| Circulator | None | -- | Moves gas passively along a pipe loop without power. |

---

## Unary Devices

Unary devices connect to a single pipe segment and interact with the ambient environment of their tile.

### Air Vent

Pumps gas between the pipe network and the surrounding room. Power draw: 30,000 W standard (45,000 W for high-volume variant). Volume per cycle: 200 L (1,000 L high-volume).

**Pump directions:**

| Direction | Behavior |
|---|---|
| Release (out) | Moves gas from internal pipe to room. Stops when room reaches external pressure bound. |
| Siphon (in) | Moves gas from room to internal pipe. Stops when pipe reaches internal pressure bound. |

**Pressure control parameters:**

| Parameter | Default | Function |
|---|---|---|
| External pressure bound | 101.325 kPa | Maximum room pressure before release mode stops pumping |
| Internal pressure bound | 0 kPa | Minimum pipe pressure before siphon mode stops pulling |
| Pressure checks | Both | Can be set to check only external, only internal, or both |

For pressurizing a room, set direction to Release with external bound at 101.325 kPa. For evacuating a room, set direction to Siphon. To flood a room to a specific pressure, raise the external bound accordingly.

### Air Scrubber

Removes selected gases from the ambient room air. Power draw: 7,500 W. Volume per cycle: 200 L.

**Scrubbing mode:** Filters only selected gases. Default filter list: carbon dioxide, phoron, methane. Can be individually toggled for any gas type. Flow rate: 200 L/s.

**Siphon mode:** Removes all air from the room regardless of composition. Flow rate: 2,500 L/s.

**Panic siphon:** Emergency full evacuation. Automatically switches to siphon mode and maximizes flow rate. Used to rapidly decontaminate areas flooded with toxic or hazardous gas.

Individually configurable gases for scrubbing: O2, N2, CO2, phoron, N2O, volatile fuel, methane. Disabling O2 and N2 scrubbing while enabling all others is the standard operational configuration for habitable spaces.

### Heat Exchanger

Equalizes temperature between two paired heat exchanger units. No power required. Used in TEG systems and in supermatter cooling loops to transfer heat from one gas circuit to another without mixing the gases.

### Freezer (Cold Sink)

Actively cools gas in the attached pipe. Power draw: up to 20,000 W. Internal volume: 600 L. Heat sink temperature: approximately 20°C. Used in supermatter cooling loops and cryogenics.

### Outlet Injector

Injects gas from the pipe network directly into the environment at the injector's tile. No power required. Used for targeted delivery, such as CO2 injection for fire suppression or N2O delivery.

---

## Omni Devices

Omni devices have multiple pipe ports for mixing or separating gas streams.

| Component | Power Draw | Flow Rate | Function |
|---|---|---|---|
| Gas Mixer | 3,700 W | 200 L/s | Combines two input gas streams into one output. Mix ratio is configurable by port. |
| Gas Filter | 7,500 W | 200 L/s | Separates a selected gas type from the main stream into a secondary output port. All other gases pass through to the main output. |

Gas filters are used to isolate specific gases for storage or disposal. A series of filters can separate a mixed gas stream into its components.

---

## Passive Devices

These components require no power and function as structural elements of the pipe network.

| Component | Function |
|---|---|
| Manual Valve | Opens or closes a pipe section manually. A closed valve fully stops flow. |
| T-Valve | Three-way junction. Allows branching or merging pipe runs without active equipment. |
| Shutoff Valve | Automated valve controlled by atmospheric sensors. Closes when a set condition is met. |

---

## Portable Equipment

### Gas Canister

Standard pressurized storage. Volume: 1,000 L. Maximum safe operating pressure: approximately 7 atmospheres (709 kPa) before leak threshold.

Canisters connect to connector ports on atmos machinery, filling stations, and portable systems. They can be wheeled to locations where permanent piping does not reach.

Supply storage pressures for reference: N2 at 90,000 kPa, O2 at 40,000 kPa, CO2 and phoron each at 25,000 kPa, N2O at 10,000 kPa, methane at 5,000 kPa. Canisters approaching or exceeding 30 atm (3,040 kPa) are approaching rupture territory and should be handled with pressure-reducing equipment.

---

## Component Volumes

For calculating gas flow and storage in a network:

| Component | Internal Volume |
|---|---|
| Standard pipe segment | 70 L |
| Pump, vent, filter, mixer | 200 L |

---

*See also: [Atmospherics](Atmospherics.md), [Atmospheric Emergencies](AtmosEmergencies.md), [Supermatter Engine](SupermatterEngine.md)*
