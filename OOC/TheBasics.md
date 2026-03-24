[OOC Reference](README.md) > The Basics

# The Basics

> **Out-of-character notice:** This document covers BYOND setup, the character creation screen, and game controls. None of this information exists within the in-world fiction.

CHOMPstation is an adult roleplay server running Space Station 13 on the BYOND engine. Players take the role of station crew over multi-hour sessions with persistent story continuity between shifts.

---

## Joining the Server

1. Download and install the BYOND client from [byond.com](https://www.byond.com).
2. Register a BYOND account.
3. Join the CHOMPstation Discord and complete the 18+ verification form to receive access to the server address.

---

## Character Setup

Set up your character in the preferences screen before joining a round. Save the character when finished. Unsaved characters are lost between sessions. Multiple character slots are available.

See [Character Creation](CharacterCreation.md) for a full walkthrough of character philosophy, backstory, naming, skills, and flavor text.

---

## Interface Overview

### UI Style

Three themes are available: **Orange**, **Midnight**, and **Old** (legacy). Set under the Global tab in preferences.

### Intent

The intent button in the lower right controls how your character interacts with others on left-click. Four modes:

| Intent | Behavior |
|---|---|
| Help | Non-aggressive interaction; CPR when clicking an incapacitated person |
| Disarm | Attempts to push or knock items out of hands without direct harm |
| Grab | Initiates a grab; can be escalated with repeated clicks |
| Harm | Aggressive strikes |

Switch intents with **F** and **G** (counterclockwise/clockwise) in hotkey mode, or number keys **1--4**.

---

## Controls

### Movement

| Input | Action |
|---|---|
| Arrow keys | Move character |
| Shift + Arrow key | Change facing direction without moving |
| Ctrl + A/W/S/D | Move (alternate) |

### Mouse

| Action | Input |
|---|---|
| Pick up item | Left-click with empty hand |
| Drop held item | Click Drop button or Q in hotkey mode |
| Attack / interact | Left-click on target with item in hand |
| Examine | Right-click > Examine |
| Pull object | Right-click > Pull; or Ctrl + click |
| Strip / dress | Drag character sprite onto own sprite |
| Give item | Right-click on adjacent person > Give |

### Chat and Radio

| Command | Function |
|---|---|
| `say "text"` | Speak in character |
| `say ";text"` | Broadcast on your headset |
| `say ":h text"` | Speak on your department radio channel |
| `whisper "text"` | Local whisper, distorted by distance |
| `me "text"` | Custom emote (visible to nearby players) |
| `subtle "text"` | Custom emote (visible only to adjacent players) |
| `ooc "text"` | Out-of-character chat (do not use for in-round information) |

**Radio channel keys:**

| Key | Channel |
|---|---|
| `:c` | Command |
| `:n` | Research |
| `:s` | Security |
| `:m` | Medical |
| `:u` | Cargo |
| `:e` | Engineering |
| `:b` | Binary (AI and Cyborgs only) |

### Hotkey Mode

Press **Tab** to toggle hotkey mode. In hotkey mode, letters are bound to actions rather than chat input.

| Key | Action |
|---|---|
| W / A / S / D | Move |
| Q | Drop |
| E | Equip |
| R | Throw |
| T | Say |
| Y | Whisper |
| X | Swap hands |
| Z | Activate held item |
| 1 / 2 / 3 / 4 | Help / Disarm / Grab / Harm intent |
| F / G | Cycle intent |
| Shift + Click | Examine |
| Ctrl + Click | Drag |

**Function keys (any mode):**

| Key | Action |
|---|---|
| F1 | Adminhelp |
| F2 | OOC chat |
| F3 | Say |
| F4 | Emote |

---

## Internals

To breathe in low-pressure or contaminated environments, set up internals:

1. Equip an air or gas mask in the mask slot.
2. Take an air tank in hand and click it to open options.
3. Set pressure output. Leave air-mix tanks at default (approximately 80 kPa). Pure oxygen tanks can be set as low as 17 kPa.
4. Large tanks attach to the back slot; emergency tanks fit the belt or pocket.

Internals must be running actively. Being in a spacesuit without active internals does not protect against vacuum.

---

## Useful Tips

- **Run/Walk toggle**: Slowing to a walk prevents slipping on wet floors. Use the Run/Walk button in the interface.
- **Container access**: Drag a container or character sprite onto your own to open an inventory window.
- **Recalling typed text**: Hold Ctrl and press Up to recall previously entered text.
- **Pushing an object while pulling**: Click a floor tile with an empty hand while pulling an object to push it in that direction.
- **Set Pose**: Use the set pose verb under the IC tab to display a short status note on your character (useful for indicating AFK state or current activity).

---

## Job Assignment

Jobs are selected in the Occupations tab of the preferences screen. Each job has four preference levels: Never, Low, Medium, High. The server assigns jobs at round start based on player preferences and slot availability.

Recommended starting jobs for new players: Assistant (no department expectation), Cargo Technician, Janitor, or Bartender. Avoid command, security, and silicon roles until familiar with the server.

---

## See Also

- [Character Creation](CharacterCreation.md) -- building a character from scratch
- [A Crash Course in Roleplaying](CrashCourseRP.md) -- IC/OOC discipline and roleplay fundamentals
- [Commands](Commands.md) -- full verb and command reference
- [Terminology](Terminology.md) -- SS13 and CHOMP-specific term glossary
