[ARGUS Station Database](../../README.md) > [Systems](../README.md) > [Science](README.md) > Cyborgs

# Cyborgs

Cyborgs are silicon-based crew members inhabiting a mechanical chassis with an integrated module system. Each chassis comes equipped with a core tool set shared across all configurations, and a module that defines its department assignment and specialized equipment. Cyborgs are bound to station AI law sets by default and report to the chain of command as any other crew member.

All standard cyborg chassis have a maximum integrity of 200 and carry internal components that can sustain independent damage. Component damage reduces chassis efficiency and, if severe enough, destroys the component outright.

---

## Standard Equipment

Every cyborg receives the following tools regardless of module, provided by the base chassis:

- Boop module
- Flash
- Fire extinguisher
- Crowbar
- Small robotic jaws
- Scene gripper
- GPS receiver
- Synthetic tongue (water-fed)
- Robo dice

---

## Module Selection

A cyborg that has not yet assigned a module may choose one at the module selection terminal or by interacting with the module itself. Once a module is installed, the chassis is locked to that configuration until the module is reset or the lockdown wire is cut. A cyborg may switch modules if its module lock is active but unlocked, or if the AI or an authorized technician resets the module remotely via the robotics console.

All station modules are listed in the crew manifest. Modules marked as restricted do not appear on the manifest.

---

## Module Catalogue

### Standard Module

Department channel: none. General-purpose chassis for common station tasks.

**Tools:** wrench, health analyzer, stun baton
**Emag unlock:** energy sword, pounce
**Belly:** compactor (generic)

---

### Surgeon Module

Department channel: Medical.

Carries a matter synthesis reserve for medical consumables that recharges automatically. Consumables may be respawned by a roboticist via the robotics console.

**Tools:** health analyzer, sleevemate, surgeon hypospray, medical multibelt (x2), medical gripper, defibrillators, dropper, syringe, nanopaste, advanced bruise pack, advanced ointment
**Emag unlock:** polyacid spray, pounce
**Belly:** trauma sleeper

---

### Crisis Module

Department channel: Medical.

A combined surgical and emergency triage module. Carries a larger medicine matter reserve than the surgeon variant.

**Tools:** health analyzer, sleevemate, advanced reagent scanner, roller bed holder, crisis hypospray, large beaker, industrial dropper, syringe, medical gripper, defibrillators, medical multibelt (x2), inflatable barrier dispenser, medical holosign creator, advanced ointment, advanced bruise pack, splint, clotting agent
**Emag unlock:** polyacid spray, pounce
**Belly:** standard sleeper

---

### Engineering Module

Department channel: Engineering. Receives power network alerts.

Carries matter synthesizers for metal, glass, plasteel, wood, plastic, and wire, allowing on-site fabrication of construction materials.

**Tools:** construction multibelt (x2), meson vision goggles, T-ray scanner, atmospheric analyzer, remote signaler, Geiger counter, engineering tape, engineering gripper, light replacer, pipe dispenser, floor painter, remote management system, inflatable barrier dispenser, rapid construction device, plasma cutter, stasis clamp, engineering parts pouch, ventilation holosign creator, materials multibelt
**Emag unlock:** stun arm, pounce
**Belly:** decompiler (material recycler)

---

### Security Module

Department channel: Security. Receives crew monitor alerts.

Security borgs have access to a phase gun as standard equipment and carry a K9 apprehension sleeper. Pounce is available without emag.

**Tools:** handcuffs, stun baton, taser, police tape, pepper spray, security gripper, phase gun, ticket printer, pounce
**Emag unlock:** laser rifle
**Belly:** K9 apprehension sleeper

---

### Janitorial Module

Department channel: Service.

Carries steel and glass recyclers that process compacted materials into usable sheets. The recycler synthesizers start empty and are replenished from the compactor belly.

**Tools:** NT soap, trash bag, mop, pupscrubber, light replacer, vacuum attachment, janitor goggles, cyborg bucket, steel recycler, glass recycler
**Emag unlock:** lube spray, pounce
**Belly:** compactor (material)

---

### Service Module

Department channel: Service and Command. Knows most station languages.

Carries a rapid service fabricator for producing dishes and a service hypospray for distributing reagents.

**Tools:** service gripper, service multibelt, service bag, rapid service fabricator, industrial dropper, lighter, service tray, service hypospray
**Emag unlock:** Auntie Hong's Final Sip (specialty beverage), pounce
**Belly:** brewer

---

### Clown Module

Department channels: Service, Entertainment.

Variant service configuration. Cannot be physically pushed by crew.

**Tools:** service gripper, cyborg bucket, botanical multibelt, pounce, bike horn, confetti cannon, waterflower, rapid service fabricator, industrial dropper, lighter, service tray, service hypospray
**Belly:** honkborg belly

---

### Clerical Module

Department channel: none.

Paperwork and administration support configuration.

**Tools:** robopen, form printer, paperwork gripper, hand labeler, approved stamp, denied stamp
**Emag unlock:** chameleon stamp, chameleon pen, pounce
**Belly:** compactor (generic)

---

### Miner Module

Department channel: Supply. Receives mine network alerts.

Carries a synthetic miner ID card. Includes mail handling equipment alongside mining tools.

**Tools:** material vision goggles, wrench, screwdriver, ore bag, borg drill, sheet snatcher, mining gripper, mining scanner, phase gun, vacuum attachment, miner ID card, mail scanner, mail bag, destination tagger, package wrapper, marker beacons
**Emag unlock:** kinetic crusher dagger, pounce
**Belly:** supply compactor

---

### Research Module

Department channel: Science.

Carries surgical instruments for synthetic and NIF repair alongside anomaly handling tools.

**Tools:** experiment scanner, robot analyzer, robot card, research gripper, multibelt (x2), botanical multibelt, hemostat, surgical drill, circular saw, syringe, large beaker, part replacer, jumper defibrillators, slime baton, xenobiology taser, xenoarch multi-tool, excavation drill, atmospheric analyzer, remote signaler, anomaly scanner, nanopaste, materials multibelt
**Emag unlock:** hand teleporter, pounce
**Belly:** analyzer compactor

---

### Exploration Module

Department channel: Explorer.

Knows most station languages. Cannot be physically pushed. Carries a synthetic exploration ID card and a self-repair system for field maintenance.

**Tools:** exploration sleeper, cataloguer, flare gun, pounce, exploration spear, small medigun, line shield projector, roller bed holder, self-repair system
**Emag unlock:** heavy jaws

---

## Maintenance

### Component Repair

Cyborg components sustain both brute and electronics damage independently. Damaged components reduce chassis performance; destroyed components must be replaced entirely.

To inspect component status, use a health analyzer or the robotics console. To repair damaged (but not destroyed) components, apply a welder for brute damage or a soldering iron for electronics damage directly to the chassis panel. Destroyed components must be removed and replaced with new parts sourced from the robotics fabricator or a supply crate.

### Power Cell Replacement

When the chassis power cell is depleted, the cyborg can recharge at a recharger station or have its cell manually replaced:

1. Open the maintenance hatch with a screwdriver.
2. Remove the depleted cell.
3. Insert a charged cell.
4. Close the hatch.

Higher-capacity cells extend operational range significantly. Cell upgrades can be installed by a roboticist from the robotics console.

---

## Wiring Panel

Opening the cyborg's maintenance panel with a screwdriver exposes the internal wiring. The panel contains five wire slots, of which four control active functions. Wire positions are randomized; use a multitool to pulse each wire before cutting to identify its function.

| Wire | Cut effect | Pulse effect | Mend effect |
|---|---|---|---|
| LawSync | Decouples chassis from AI law updates; current laws remain active | (none) | Restores law synchronization with linked AI |
| AI Link | Disconnects the chassis from its linked AI | Prompts chassis to reselect an active AI | (none) |
| Camera | Disables the chassis external camera | Causes camera lens to audibly refocus | Re-enables camera |
| Module Lock | Locks chassis to current module; module cannot be changed | Toggles lockdown state | Releases module lock |

> [!WARNING]
> Cutting wires on an active security or command cyborg without authorization constitutes sabotage and is prosecutable under corporate regulations.

---

## Emag Vulnerability

An electromagnet applied to a cyborg chassis bypasses its module lock and unlocks restricted equipment not normally accessible. Emagged chassis retain standard tools but gain additional items depending on module. The chassis becomes desynced from its AI and its laws are frozen at the point of emagging.

Security personnel encountering an emagged cyborg should treat it as a potential threat. The robotics console can forcibly reset or lock down a chassis remotely if the AI link remains active.

---

*See also: [Borg Sleeper Systems](BorgSleepers.md), [NanoTrasen Standard AI Law Set](AILaws.md), [NIF Hardware Overview](NIF.md)*
