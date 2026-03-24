[ARGUS Station Database](../../README.md) > [Systems](../README.md) > [Engineering](README.md) > Wiring Reference

# Wiring Reference

Station infrastructure components -- airlocks, APCs, atmospheric alarms, cameras, and major machinery -- expose internal wiring that can be cut, mended, or pulsed to alter their behaviour. Wire colours are randomised each shift but are consistent across all instances of the same device type throughout the station.

---

## Required Tools

| Tool | Use |
|---|---|
| Insulated gloves | Protection against electrical shock from live wires |
| Screwdriver | Opens and closes access panels |
| Wirecutters | Cuts and mends wires |
| Multitool | Pulses wires without cutting; used to identify wires safely |
| Crowbar | Pries open doors after wiring manipulations |

---

## Airlocks

Airlock wiring is accessed by applying a screwdriver to the door to open the access panel, then pressing the door with an empty hand to open the wiring interface.

Wire colours are the same for all airlocks on the station within a given shift. Identifying the correct wires on one door carries that knowledge to all other doors.

### Wire Functions

| Wire | Cut effect | Pulse effect |
|---|---|---|
| **ID** | Prevents anyone from opening a restricted door | Flashes the access-denied light |
| **AI Control** | Prevents the AI from operating the door (unless the AI cuts main power wires) | Flashes the AI control indicator |
| **Main Power (×2)** | Cuts main power; backup power activates after a delay | Temporarily cuts power for a short interval; causes sparks |
| **Backup Power (×2)** | Disables backup power | Temporarily cuts backup power (only if main power is already out) |
| **Bolt Control** | Drops the door bolts (door cannot open while bolted) | Toggles bolts between up and down |
| **Bolt Light** | Turns off the bolt status indicator light | Toggles the bolt indicator light |
| **Door Control** | Holds the door in its current open or closed state | Opens or closes the door (on unrestricted doors only) |
| **Electrify** | Permanently electrifies the door until mended; safety light flashes | Electrifies the door for 30 seconds |
| **Door Safeties** | Disables the sensor that prevents the door from closing on a person | Toggles the safety sensor state |
| **Door Timing** | Disables the automatic close timer (door stays open) | Toggles the close timer |

### Access via Multitool

To identify wires safely without cutting:

1. Open the wiring panel with a screwdriver.
2. Press the door with an empty hand to open the wiring interface.
3. Pulse each wire in sequence. Monitor the status indicators at the bottom of the interface for reactions.
4. The bolt control wire causes the bolt status indicator to change. The main power wires cause the test light to turn off.
5. Record wire colours. Close the wiring panel with a screwdriver to restore normal operation.

To open a bolted or restricted door using a multitool and crowbar:

1. Pulse the main power wire. The door loses power for approximately 10 seconds.
2. Apply the crowbar to the door while power is off to pry it open.

The door remains open after this method. Apply the crowbar again to close it, then rescrewdriver the panel to reseal it.

### Access Without Multitool

Without a multitool, wires must be identified by cutting. This is destructive: a door whose wires have been partially cut may not function normally until repaired by an engineer.

1. Open the wiring panel. Equip wirecutters.
2. Cut wires one at a time until the bolt status indicator shows the bolts have dropped. Record that wire colour. Mend all other cut wires.
3. On the target door, cut all wires except the identified bolt wire.
4. Apply a crowbar to pry the door open.

### Emergency Deconstruction

An airlock can be fully removed without power using the following steps:

1. Apply a welding tool to seal the door shut.
2. Strike the airlock electronics panel with a blunt object on harm intent to break the cover.
3. Apply a crowbar to remove the broken electronics.
4. Apply wirecutters to disconnect the internal wiring.
5. Apply a wrench to unsecure the door from the floor.

### Strategies

An airlock can be turned into a permanent barrier by dropping the bolts, cutting all wires, and welding the door sealed. A door electrified with the electrify wire shocks anyone who touches it; attaching a remote signaller to the bolt wire allows bolts to be toggled from a distance.

---

## APCs

Access the wiring by applying a screwdriver to open the APC cover, then pressing the unit with an empty hand.

| Wire | Cut effect | Pulse effect |
|---|---|---|
| **Main Power (×2)** | Shorts out the APC; must cut and mend both to restore power | Shorts out the APC |
| **AI Control** | Disables AI control of this APC | Flashes the AI control indicator |
| **APC Lock** | -- | Unlocks the APC interface |

A power short requires cutting and then immediately mending the wire to restore power. Leaving a shorted APC without mending the wire prevents remote restoration through the Power Monitoring Computer.

---

## Atmospheric Alarms

Access the wiring by applying a screwdriver to the alarm panel, then pressing with an empty hand.

| Wire | Cut effect | Pulse effect |
|---|---|---|
| **ID Scan** | Prevents anyone from accessing the alarm regardless of ID | Unlocks the alarm for 30 seconds |
| **Alarm** | Triggers an atmospheric alert in the area | Resets the current alarm status |
| **Panic Syphon** | Activates the panic syphon | Activates the panic syphon |
| **AI Control** | Prevents AI from using the alarm | Flashes the AI control indicator |
| **Power** | Deactivates the alarm entirely | Deactivates the alarm for 30 seconds |

The panic syphon activated by wire manipulation cannot be deactivated by mending; it must be turned off from the alarm interface directly.

---

## Cameras

Access the wiring by applying a screwdriver to the camera body, then applying wirecutters to open the wire panel.

| Wire | Cut effect | Pulse effect |
|---|---|---|
| **Power** | Disables the camera | Toggles the camera on and off |
| **Alarm** | Triggers a security alarm | Produces an audible tone (identification method) |
| **Light** | Prevents the AI from toggling the camera's illumination | Toggles the light on and off |
| **Focus** | Reduces vision range to a short distance | Toggles between normal and reduced range |
| **Nothing (×2)** | No effect | No effect |

The alarm wire is identified by the audible tone produced when pulsed. Cutting the alarm wire triggers the alarm immediately; use the multitool to confirm this wire before cutting.

---

## Particle Accelerator

The PA is wired through its control console. Apply a screwdriver to the console to open the panel, then press the console with an empty hand to access the wiring.

| Wire | Cut effect | Pulse effect |
|---|---|---|
| **Toggle** | Disables the PA (cannot be turned on while cut) | Toggles the PA on or off |
| **Strength** | Forces output strength to 0 and prevents adjustment | Increases output strength by one step |
| **Interface** | Locks the control console (toggles) | Toggles the interface lock |
| **Limit Power** | Allows output strength to reach level 3 | Produces a beep (identification method) |
| **Nothing** | No effect | No effect |

> [!IMPORTANT]
> After any wiring manipulation on the PA console, close the panel with a screwdriver and perform a **Scan for Parts** from the console before operating the accelerator. The link between the console and the physical assembly must be re-established after panel manipulation.

---

## SMES Units

See [SMES](SMES.md#wiring) for the complete SMES wire reference. SMES wiring includes input control, output control, RCON control, failsafe bypass, and grounding.

---

## Syndicate Bomb Defusal

A syndicate bomb has five wires accessible by applying a screwdriver to the casing, then pressing the bomb with an empty hand.

> [!CAUTION]
> Randomly pulsing a live bomb carries significant risk of detonation. Cutting carries higher risk. Methodical identification before cutting is strongly recommended.

| Wire | Cut effect | Pulse effect |
|---|---|---|
| **Boom** | Detonates the bomb if live; disables it if not yet armed | Detonates the bomb if live |
| **Bolt** | Releases floor bolts if active, freeing the bomb | Hints at wire function |
| **Delay** | No effect | Adds time to the countdown |
| **Proceed** | Detonates the bomb if live | Reduces countdown time |
| **Activate** | Stops the countdown if the bomb is live | Starts the countdown if the bomb is not yet armed |

Identifying the activate wire via the delay or proceed wire's pulsed responses, then cutting it, is the primary defusal method.

---

## Minor Systems

### Fire Alarms

Cutting the wire inside a fire alarm panel disables fire detection and fire door activation for that alarm. The alarm will not respond to smoke or temperature changes until the wire is mended.

### Radios and Intercoms

Radios expose two functional wires after opening the casing with a screwdriver:

| Wire | Cut effect |
|---|---|
| **Output** | Disables the speaker (incoming signal is not heard) |
| **Input** | Disables the microphone (outgoing signal is not transmitted) |

This applies to station-bounced radios, signalers, and intercom units.

### Secure Briefcases and Safes

The combination lock memory can be reset by applying a multitool repeatedly until a confirmation message appears. After reset, a new combination can be set.

### Vending Machines

Vending machine wiring exposes four wires:

| Wire | Cut effect | Pulse effect |
|---|---|---|
| **Firing** | Causes machine to periodically eject items | Ejects an item |
| **Contraband** | No effect | Unlocks restricted or rare items in the machine's inventory |
| **Access** | Removes the ID restriction from a locked departmental machine | Toggles the access restriction |
| **Shock** | Causes the machine to electrify users on contact | Electrifies the next user |

### Hardsuits

Hardsuit wiring is accessed by unlocking the hardsuit panel (using an ID card or an emag), then applying a screwdriver to open it.

| Wire | Cut effect | Pulse effect |
|---|---|---|
| **Security** | Disables security checks on the suit | Causes the suit to twitch |
| **AI Override** | -- | Toggles AI control of the suit |
| **System Control** | -- | Toggles certain suit malfunctions |
| **Interface Lock** | -- | Toggles interface access lock |
| **Interface Shock** | -- | Toggles whether the suit shocks the user |
