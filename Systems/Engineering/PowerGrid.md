[ARGUS Station Database](../../README.md) > [Systems](../README.md) > [Engineering](README.md) > Power Grid

# Power Grid

The station power grid distributes electricity from generation sources through storage banks to every powered area on the station. Understanding the grid's topology and failure modes is essential for engineering personnel responding to power loss events.

---

## Grid Topology

Power flows in one direction through a fixed hierarchy:

**Generator** (Supermatter engine, solar arrays, or TEG) produces power and feeds it to **SMES units** via powernet cable. The SMES stores surplus and regulates output. From the SMES, power flows through the powernet cable network to **APC terminals**, which charge the **Area Power Controllers** (APCs) located in each room or department zone. APCs distribute power to the devices within their coverage area through three separate channels.

A break or overload at any stage of this chain cuts power to everything downstream of the failure point.

---

## SMES Units

Station Mechanical Energy Storage (SMES) units are the primary buffer between generation and distribution. Each unit accepts power from upstream generators, accumulates it, and delivers regulated output to the APC network downstream. A depleted SMES with no active generation source causes a complete power failure for all APCs downstream of it.

For configuration, specifications, construction, upgrading, wiring, and failure mode reference, see [SMES](SMES.md).

---

## Area Power Controllers

An APC is installed in every powered area of the station. It accepts charge from the powernet via a wall terminal, stores that charge in an internal power cell, and distributes power to three independently switchable channels within its coverage area.

### Power Channels

| Channel | Controls |
|---|---|
| Lighting | Area lighting fixtures |
| Equipment | Machines, computers, and most devices |
| Environmental | Climate control, vents, scrubbers, and HVAC systems |

Each channel can be set to one of four states:

- **Off:** Channel disabled, no power supplied.
- **Off (Auto):** Channel off but will re-enable automatically when the APC cell charges above the activation threshold.
- **On:** Channel active, power supplied continuously.
- **On (Auto):** Channel active; will automatically disable during low-cell conditions and re-enable when the cell recovers.

The default station configuration runs all three channels on Auto. During a power shortage the APC will shed lighting and environmental load to preserve equipment power, following the priority order built into the auto-management logic.

### APC Power Cells

The internal cell determines how long an APC can sustain its channels without grid input. Higher-capacity cells extend runtime significantly during generator outages or grid instability.

| Cell Type | Capacity |
|---|---|
| Standard (heavy-duty) | 5,000 |
| High-capacity | 10,000 |
| Super-capacity | 20,000 |
| Hyper-capacity | 30,000 |
| Giga-capacity | 40,000 |

Replacing an APC cell requires opening the APC panel with a screwdriver. Cells can also be charged externally at a recharger station before installation. Standard station APCs ship with heavy-duty cells; engineering supply stocks higher-capacity replacements.

### APC Charge Behavior

When powernet supply is available, the APC draws from the grid first and directs surplus to the internal cell. When grid supply drops below demand, the APC draws from the internal cell to compensate. If both grid and cell are depleted, the APC deactivates all channels until power is restored.

The APC charges its cell at a capped rate per processing cycle. This means a fully depleted hyper-capacity cell takes longer to bring back to operational charge than a standard cell, even with the same grid input rate.

---

## Cable and Terminal Infrastructure

Powernet cables carry electricity between SMES units, APC terminals, and generators. Cable can be routed through walls, floors, and maintenance crawlways. Standard cable runs are documented on the station wiring maps.

APC terminals are the wall-mounted connection point between the powernet cable and the APC unit. Each APC has exactly one terminal. Damaging or removing the terminal disconnects the APC from the grid entirely, regardless of internal cell charge.

> [!CAUTION]
> Cutting a powernet cable upstream of multiple APCs will drop all downstream areas simultaneously. Identify the affected segment on the wiring map before cutting any cable during repairs.

---

## Common Failure Scenarios

**Single area outage:** The APC cell is depleted and no grid input is reaching the terminal. Check the APC panel for cell status. If the cell is present and the grid is live, the terminal connection may be damaged. If the cell is missing or dead, replace it.

**Multi-area outage in one wing:** A cable break upstream of the affected APCs, or a tripped/depleted SMES serving that segment. Trace the wiring map to locate the break. Check the SMES output level and charge.

**Station-wide power failure:** The primary generator is offline and all SMES units have depleted. Restore the Supermatter engine, bring the TEG online as backup, or connect the emergency solar array. Priority areas (medical, bridge, atmospherics) should be switched to manual On with non-Auto channels to conserve remaining cell charge while generation is restored.

**Nightshift lighting loss:** Expected behavior on stations running lighting channels in Auto mode. The APC is managing load by shedding non-critical channels. Not a fault condition unless equipment channels are also dropping.

---

*See also: [SMES](SMES.md), [Supermatter Engine](SupermatterEngine.md), [Atmospherics](Atmospherics.md)*
