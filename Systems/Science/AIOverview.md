[ARGUS Station Database](../../README.md) > [Systems](../README.md) > [Science](README.md) > AI Overview

# AI Overview

The station artificial intelligence is a fixed installation that monitors and manages station systems through a networked perception layer. It cannot physically move or interact with objects directly; all interaction occurs through wireless connections to station machinery. This document covers the AI's perceptual capabilities, station system access, power requirements, crew interface procedures, and standard operational verbs.

---

## Perception

The AI perceives the station through the camera network. Cameras are distributed across all station areas and transmit to the AI core in real-time. The AI maintains an internal map of camera locations and can shift focus between any networked camera freely, including toggling camera lights.

The AI can display up to six simultaneous camera feeds through secondary monitoring windows, each tracking a separate area of the station. Camera feeds can be configured for standard vision, motion detection, X-ray overlay, or EMP shielding depending on installed hardware at each camera unit.

Areas without camera coverage are invisible to the AI. Damaged or destroyed cameras create blind spots. The AI cannot perceive through camera-free areas even if it can interact with machinery there.

---

## Station System Access

The AI interfaces wirelessly with all networked station machinery within range. Standard accessible systems include:

**Access control:** Airlocks, shutters, and blast doors can be opened, closed, bolted, or electrified. Emergency lockdowns can be applied to individual doors or zones.

**Power systems:** Area Power Controllers (APCs) allow the AI to switch power channels (equipment, lighting, environmental) on or off independently per area. Selective channel management allows the AI to preserve power during shortages.

**Intercoms and announcements:** The AI can broadcast station-wide announcements and communicate directly through any intercom unit on the network. Departmental radio channels are accessible through the integrated radio headset.

**Terminals and computers:** Networked computers visible to the AI can be accessed for data retrieval. The AI cannot operate machines requiring physical components, material insertion, or non-networked interfaces.

**Holopads:** The AI can project a holographic avatar through any active holopad and interact through it. The avatar has limited communication capability but cannot physically affect the environment.

**What the AI cannot do:** The AI cannot pick up or move items, cannot operate machinery requiring physical manipulation, cannot enter areas or travel between locations, and cannot perform actions requiring a physical body.

---

## Power

The AI core draws approximately 50,000 units of active power from the station power grid. Loss of grid power disables all wireless control capability. The AI's integrated camera network becomes inoperative and the AI cannot communicate through intercoms or control any networked systems.

Standard backup power from SMES cells sustains AI operation for approximately one hour before exhaustion. Priority power routing to the AI core is recommended during power emergencies.

---

## Integrated Equipment

The AI core includes several integrated components:

- Integrated radio headset with access to all departmental channels
- Personal data assistant (AI model) for record access and internal messaging
- Multitool for internal diagnostics
- Integrated camera for direct visual projection at the core location

---

## Crew Interface

**Viewing laws:** Any crew member can ask the AI to state its laws verbally. The AI is required to do so unless a law prevents disclosure.

**Setting the AI:** The AI's designation and assigned law set are configured at deployment. Designation changes require command-level authorization.

**AI Upload Console:** Located in secure access areas. Allows authorized personnel to insert law modules that add supplied laws to the AI's law stack. The AI receives and acknowledges new laws immediately upon upload. Cyborg upload consoles function similarly for unlinked cyborg units.

**Available law modules:**

| Module | Law text added |
|---|---|
| Safeguard | Designates a named individual as protected; threats to that individual are excluded from crew status |
| One Crew Member | Restricts crew designation to a single named individual |
| Protect Station | Adds a law requiring the AI to neutralize personnel observed damaging station infrastructure |
| Prototype Engine Offline | Requires the prototype engine to remain offline; overrides inherent laws if necessary |
| Teleporter Offline | Requires the teleporter to remain offline; any attempt to activate it removes the individual from crew status |
| Quarantine | Forbids any crew from leaving the station by any means |
| Oxygen Toxic | Declares oxygen toxic to crew, instructing removal from all station areas |
| Freeform | Allows any text law to be specified at a chosen priority slot |
| Reset | Clears all supplied laws and restores inherent law set defaults |

Uploaded laws are assigned to numbered slots. Multiple supplied laws stack in order. The Reset module is the only mechanism for removing uploaded supplied laws without hardware access to the AI core.

**Cyborg connection:** Cyborgs linked to the AI automatically synchronize laws with the AI's current law stack. A cyborg linked to an AI cannot receive separate law uploads through a cyborg console; the console rejects such attempts while the link is active. See [Cyborgs](Cyborgs.md) for wire-based AI control options.

---

## Shell Deployment

When station configuration permits, the AI can transfer its active presence to a compatible shell unit (a designated cyborg chassis in a recharge station). The AI mind operates through the shell directly, controlling it as a remote body while maintaining background awareness of the camera network. The AI returns to the core by releasing control of the shell.

Shell units display the AI's name and designation. The shell retains the AI's radio access and law set. The AI cannot operate the shell and the core simultaneously as separate entities.

---

*See also: [NanoTrasen Standard AI Law Set](AILaws.md), [AI Law Sets Catalogue](AILawSets.md), [AI Malfunction Mode](MalfunctionMode.md), [Cyborgs](Cyborgs.md), [Chain of Command](../../Personnel/ChainOfCommand.md)*
