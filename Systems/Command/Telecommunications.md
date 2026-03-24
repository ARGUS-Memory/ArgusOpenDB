[ARGUS Station Database](../../README.md) > [Systems](../README.md) > [Command](README.md) > Telecommunications

# Telecommunications

The station telecommunications network routes all subspace radio traffic through a server room containing five categories of hardware. Each machine performs a discrete step in signal processing; the failure of any component degrades or halts communications for the channels it handles. The network is pre-configured at station initialization and requires no routine operator intervention under normal conditions.

For crew-facing radio operation — frequencies, encryption keys, headset types, and intercom use — see [Radio System](RadioSystem.md).

---

## Signal Chain

All radio transmissions travel a fixed path through the network:

**Subspace Receiver** → **Bus Mainframe** → **Processor Unit** → **Telecommunication Server** → **Subspace Broadcaster**

A signal entering from space or a headset is captured by the Receiver, routed through the Bus for high-speed transfer, decoded by the Processor, logged and sorted by the Server, and then broadcast back out through the Broadcaster to receiving headsets. Each stage must be operational and linked for the chain to complete.

---

## Machine Types

### Subspace Receiver

Maintains a continuous subspace window that intercepts FTL-band radio signals passing nearby. Incoming signals produce a real-space copy that is forwarded to all linked machines — normally Bus Mainframes. The Receiver is the entry point for all incoming transmissions; without it, nothing reaches the rest of the network.

One Receiver is the minimum required for a functional network. Multiple Receivers covering different relay points (station, mining, external) allow the network to handle transmissions from off-station locations.

### Bus Mainframe

Handles high-speed bulk data transfer between machines. The Bus sits between the Receiver and the Processor, moving signal data at near-instantaneous speeds. Without a Bus, data transfer slows and output becomes unreliable.

The station runs multiple Bus units (Bus 1 through Bus 4) to distribute load. In an emergency the Receiver can be linked directly to a Processor, bypassing the Bus entirely, at the cost of significant network lag.

### Processor Unit

Decrypts and decompresses incoming signals. Radio transmissions are compressed for subspace transit using a hash-based process; the Processor reverses this to produce a readable signal for downstream machines. Without a working Processor, signals reach the Server and Broadcaster as garbled output that headsets cannot interpret.

The station runs four Processor units. A minimum of one is required for comprehensible communications.

### Telecommunication Server

Logs signal traffic, stores channel statistics, and manages transmission ordering. Each Server handles one or more named channels. The default configuration assigns a dedicated Server per department: Science, Medical, Supply, Service, Common, Command, Engineering, Security, and an additional spare.

Destroying a Server takes down the channels it manages. Security and Command Servers are priority targets for sabotage; losing them silences those channels while other traffic continues normally.

### Subspace Broadcaster

Opens outbound subspace windows and retransmits processed signals back to receiving radio devices. The Broadcaster is the exit point of the network; without it, signals are processed internally but never reach headsets. At least one Broadcaster must be operational for any outbound communications.

---

## Station Network Layout

The default network runs on the `tcommsat` network ID. Key machines by role:

| Role | Machine |
|---|---|
| Primary reception | Receiver A |
| External relays | Station Relay, Telecomms Relay, Mining Relay |
| CentCom link | CentCom Relay, CentCom Receiver, CentCom Hub, CentCom Bus, CentCom Processor, CentCom Server, CentCom Broadcaster |
| Signal processing | Bus 1–4, Processor 1–4 |
| Channel servers | Science, Medical, Supply, Service, Common, Command, Engineering, Security, Unused |
| Output | Broadcaster A |

The CentCom machines form an isolated parallel chain handling communications between the station and Central Command. Station-side machines and CentCom machines are linked through the relay layer but otherwise operate independently.

---

## Maintenance

### Heat Management

All active telecomms machines produce heat. The server room is cooled by a dedicated atmospheric system; without cooling, machine integrity degrades and eventually fails. If the cooling system goes offline, machines begin accumulating heat damage and will shut down if the temperature is not corrected.

Restoring cooling is the first priority in any telecomms emergency. Supercooled air must be pumped into the room; the machines cannot otherwise dissipate generated heat.

### Repairing Damaged Machines

Machines that have lost integrity but are still standing can be partially repaired with nanopaste. Each application restores 10–20 integrity points. For machines under 100% integrity, nanopaste is the fastest option without deconstruction.

### Reconstructing Destroyed Machines

If a machine is destroyed, it must be rebuilt from components:

1. Obtain a circuit board for the machine type from Research and Development. High-tier board components are required; request them from the Research Director or salvage from other destroyed machines.
2. Place a machine frame in the desired location and anchor it.
3. Insert the circuit board, then add cables.
4. Add stock parts matching the machine tier.
5. Secure the cover with a screwdriver to complete assembly.

A minimum viable network requires one of each: Receiver, Processor, Server, and Broadcaster. Bus Mainframes and additional units improve reliability but are not strictly required for basic function.

Machines can also be repaired short of full destruction by deconstruction and reassembly:
1. Unscrew the exterior bolts with a screwdriver.
2. Remove the plating with a wrench.
3. Cut the internal cables with wirecutters.
4. Pry out the components and circuit board with a crowbar.
5. Rebuild on the existing frame or deconstruct and replace it.

---

## Linking Machines

Machines are pre-linked at station initialization via autolinker IDs. If machines are replaced or the network needs to be restructured, manual linking is performed with a multitool.

To link two machines:
1. Use the multitool on the first machine. Select **Add Machine** to store it in the multitool's buffer.
2. Use the same multitool on the second machine.
3. Select **Link** to add the buffered machine to the second machine's link list.

The link is one-directional per operation; both machines should be linked to each other for bidirectional signal flow. Linking a machine to itself is harmless but has no effect.

### Emergency Link Substitutions

When standard links cannot be restored, machines can be cross-linked outside their normal chain positions at a performance cost:

| Missing machine | Emergency substitution | Performance cost |
|---|---|---|
| Bus Mainframe | Link Receiver directly to Processor | Substantial network lag |
| Bus Mainframe | Link Bus directly to Broadcaster (skipping Server) | Minor decrease |
| Processor Unit | Link Receiver directly to Server | Signals arrive unreadable |
| Telecommunication Server | Servers are not substitutable; remove from chain | Loss of affected channels and logging |
| Broadcaster | No substitution; network output ceases | Total broadcast failure |

---

*See also: [Radio System](RadioSystem.md), [Standard Operating Procedure](StandardOperatingProcedure.md), [Hacking](../../Engineering/Hacking.md)*
