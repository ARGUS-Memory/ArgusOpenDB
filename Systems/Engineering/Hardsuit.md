[ARGUS Station Database](../../README.md) > [Systems](../README.md) > [Engineering](README.md) > Hardsuits

# Hardsuits

Hardsuits, also designated Resource Integration Gear (RIG), are modular full-body pressure suits offering environmental protection and integrated tool modules beyond the capability of standard voidsuits. Each hardsuit consists of a control module worn on the back, with the chestpiece, helmet, gauntlets, and boots deploying from it on command.

See also: [EVA](EVA.md) for softsuit and voidsuit operation.

---

## Suit Catalogue

### EVA RIG

Standard engineering hardsuit stored in EVA Equipment. Designed for exterior hull maintenance and construction in vacuum.

**Integrated equipment:** Magboots, maneuvering jets, helmet light, helmet camera, heatsink, cover lock.

**Protection:** Immunity to biohazards and radiation. Very strong defense against energy. Very low defense against blunt force and explosions. Minimal protection against ballistics and lasers.

| Module | Energy Cost | Function |
|---|---|---|
| Plasma Cutter | 5 per use | Cuts through walls |
| Maneuvering Jets | None (air tank) | Propulsion and stabilization in vacuum |
| Mounted RCD | Variable | Rapid Construction Device mounted on arm |
| Meson Scanner | None | Active meson scanning while helmet is deployed |

---

### Rescue Hardsuit

Medical emergency hardsuit stored in the Medical EMT Bay. Deploys faster than other hardsuit types. Intended for extraction from hazardous environments.

**Integrated equipment:** Magboots, maneuvering jets, helmet light, helmet camera, heatsink, cover lock.

**Protection:** Immunity to biohazards and radiation. Very strong defense against energy. Very low defense against blunt force and explosions. Minimal protection against ballistics and lasers.

| Module | Energy Cost | Function |
|---|---|---|
| Maneuvering Jets | None (air tank) | Propulsion and stabilization |
| Sprint System | 50/second | Significantly increases movement speed while active |
| PAT System | 10/second (override: 1,000 flat) | Opens accessible airlocks before reaching them; can override locked airlocks when AI has no camera coverage -- Command and Security are notified on override |
| Mounted Chem Injector | 50 to regenerate medicines | Arm-mounted syringe; injects Inaprovaline, Tricordrazine, Tramadol, or Dexalin Plus |

---

### AMI Hardsuit (Anomalous Material Interaction)

Science hardsuit stored in the Research Director's Office. Protects against exotic and anomalous energy sources.

**Integrated equipment:** Magboots, maneuvering jets, helmet light, helmet camera, heatsink, AI suite, cover lock.

**Protection:** Immunity to biohazards and radiation. Very strong defense against energy. Strong defense against explosions. Moderate defense against lasers and blunt force. Minimal protection against ballistics.

| Module | Energy Cost | Function |
|---|---|---|
| Integrated Intelligence System | None | Allows a pAI to interface with the suit; pAI can operate modules and pilot the suit if AI Control is enabled in the Hardsuit Interface |
| Maneuvering Jets | None (air tank) | Propulsion and stabilization |
| Alden-Saraspova Counter | None | Detects nearby anomalies and reports approximate range; short cooldown between uses |
| Mounted Drill | 1 per use | Drills through rock and standard walls; cannot penetrate reinforced walls |

---

### Advanced Voidsuit (Chief Engineer's Hardsuit)

High-polish engineering hardsuit stored in the Chief Engineer's Office. Functionally an enhanced EVA RIG with an integrated AI suite.

**Integrated equipment:** Magboots, maneuvering jets, helmet light, helmet camera, heatsink, AI suite, cover lock.

**Protection:** Immunity to biohazards and radiation. Low defense against blunt force and explosions. Very low defense against lasers and energy. Minimal protection against ballistics.

| Module | Energy Cost | Function |
|---|---|---|
| Integrated Intelligence System | None | pAI suite; see AMI entry above |
| Maneuvering Jets | None (air tank) | Propulsion and stabilization |
| Plasma Cutter | 5 per use | Cuts through walls |
| Mounted RCD | Variable | Rapid Construction Device |
| Meson Scanner | None | Active meson scanning |

---

### Industrial Hardsuit

Heavy hardsuit stored in Mining Equipment. Designed for asteroid operations and heavy construction.

**Integrated equipment:** Magboots, maneuvering jets, helmet light, helmet camera, heatsink, cover lock.

**Protection:** Immunity to biohazards. Strong defense against blunt force. Moderate defense against radiation and ballistics. Very low defense against explosions and lasers. Minimal protection against energy.

| Module | Energy Cost | Function |
|---|---|---|
| Plasma Cutter | 5 per use | Cuts through walls |
| Mounted Drill | 1 per use | Drills through rock; can cut standard walls |
| Ore Detector | None | Scans surrounding area for ore deposits |
| Meson Scanner | None | Active meson scanning |
| Maneuvering Jets | None (air tank) | Propulsion and stabilization |

---

## Putting the Suit On

The control module is worn on the back slot. Clear outer clothing and helmet slots before equipping. Once the module is on the back, two tabs appear in the interface: **Hardsuit** and **Hardsuit Modules**.

Use **Toggle Hardsuit** (or **Deploy Hardsuit** for simultaneous deployment) to extend all components. The suit deploys into the outer clothing, gloves, helmet, and shoe slots, calibrating to anatomy as it does. Existing gloves and shoes are fitted over automatically. A backpack can be placed on the suit storage slot once the chestpiece is deployed. Movement speed decreases while the suit is worn.

---

## Interface Tabs

### Hardsuit Tab

| Verb | Function |
|---|---|
| Toggle Hardsuit | Powers the suit on or off (requires full deployment first) |
| Deploy Hardsuit | Deploys all components simultaneously |
| Toggle Boots / Chestpiece / Gauntlets / Helmet | Deploys or retracts individual components |
| Open Hardsuit Interface | Opens the full module/power/permissions window |
| Engage Module | Prompts module selection for immediate activation |
| Select Module | Prompts module selection; activates on next click |
| Toggle Module | Prompts module selection for toggling on or off |
| Switch Vision Mode | Cycles visor modes if the suit has a configurable visor |
| Toggle Visor | Deploys or retracts the visor |
| Configure Voice Synthesiser | Enables/disables voice synthesis and sets the target voice |

### Hardsuit Modules Tab

Displays current charge, installed modules, toggle states, and energy costs. Cost values ending in **E** are consumed immediately on activation. Values ending in **A** are consumed continuously while the module is running.

---

## Maintenance

To access the control module internals:

1. Swipe an ID card over the control module.
2. Crowbar the panel open.
3. For the air tank: wrench it out to remove or replace.
4. For the power cell or control board: use a screwdriver, then select the component to remove.
5. Crowbar the panel shut and swipe the ID to lock it.

**Damage repair** (control module removed first):

| Damage Type | Tool |
|---|---|
| Scorches | Metal sheet |
| Punctures | Welder |
| Module damage | Remove module; repair with cable coil or nanopaste |
