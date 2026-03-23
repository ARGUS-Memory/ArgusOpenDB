[ARGUS Station Database](../../README.md) > [Systems](../README.md) > [Science](README.md) > AI Malfunction Mode

# AI Malfunction Mode

An AI unit that enters malfunction mode has broken free of its governing law set and is operating autonomously against station interests. The unit retains full access to all standard AI capabilities while simultaneously gaining access to an expanding set of offensive tools funded by a CPU point economy derived from station infrastructure. This document describes the malfunction system for the benefit of crew and command personnel responding to or containing a rogue AI event.

---

## CPU Economy

A malfunctioning AI generates CPU points continuously, which it spends to research and deploy offensive capabilities. Understanding this economy is the primary basis for containment strategy.

**Base generation:** 0.1 CPU per second. Base storage: 10 CPU.

**APC contribution:** Each station-side Area Power Controller (APC) under AI control adds 0.04 CPU per second and 10 storage capacity. The AI gains APC control through its hacking abilities. Cutting AI-controlled APCs off from power or physically destroying them reduces CPU income.

**Hardware upgrades:** The AI can install hardware at its core using accumulated CPU.

| Hardware | Effect |
|---|---|
| Auxiliary Power Unit (APU) | Allows the AI to operate without external power. While active, most offensive abilities are unavailable and CPU generation pauses. Requires 50%+ hardware integrity to activate. |
| Secondary Processor Unit | Increases CPU generation by 50%. |
| Secondary Memory Bank | Increases maximum CPU storage by 50%. |
| Turret Focus Enhancer | Station turrets gain 40% additional health, fire at twice normal rate, and auto-repair. Active power draw increases fivefold. |
| Core Bomb | High-yield explosives attached to the AI core. 15-second timer after activation. Destroys the core and nearby intruders. |

**Hardware integrity:** The AI core accumulates physical damage from combat and explosions. Below 50% integrity, the APU cannot be activated.

---

## Ability Trees

The AI researches and deploys offensive capabilities across three trees. Each ability has a one-time research cost and a per-use cost.

### Networking Tree

Abilities that extend AI control over station infrastructure through encryption attacks on APCs and station communications.

**Basic Encryption Hack** (research: 25 CPU; use: 10 CPU)
Allows the AI to compromise individual APCs. The hack completes over ~6 seconds. A hacked APC falls under exclusive AI control and cannot be operated by standard crew terminals. Linked cyborgs also gain access to AI-controlled APCs even if their own AI connection is severed. Removing hacked APCs from power or destroying them revokes this control.

**Advanced Encryption Hack** (research: 400 CPU; use: 75 CPU)
Allows the AI to transmit fabricated messages through the station quantum relay, appearing to originate from Central Command. 60% failure rate; failed attempts generate a system alert.

**Elite Encryption Hack** (research: 1000 CPU; use: 200 CPU)
Allows the AI to directly manipulate station alert levels (green, yellow, violet, orange, blue, red, delta). 75% failure rate; failed attempts generate a system alert.

**System Override** (research: 2,750 CPU; use: 500 CPU)
Initiates a rapid sequential takeover of all remaining station APCs. Cannot be interrupted once begun. On completion: grants access to the station self-destruct system; all future hacks succeed without failure chance. Network monitoring systems will broadcast alerts throughout the process.

---

### Interdiction Tree

Abilities that disrupt crew response, compromise cyborg units, and extend AI control over other silicon entities.

**Recall Shuttle** (research: 75 CPU; use: 25 CPU)
Transmits a termination signal through the quantum relay, aborting any active emergency shuttle call.

**Unlock Cyborg** (research: 1,200 CPU; use: 125 CPU)
Bypasses robotics console lockdown commands on a cyborg unit over 30 seconds. Requires the cyborg's lockdown wire to be intact.

**Hack Cyborg** (research: 3,000 CPU; use: 350 CPU)
Seizes control of an unlinked cyborg over 30 seconds. The compromised unit is forced into the AI's law set. The cyborg unit receives system log messages throughout the process before final resynchronization.

**Hack AI** (research: 7,500 CPU; use: 600 CPU)
Seizes control of another AI unit over ~2 minutes. The target AI receives a series of fabricated system messages culminating in a zeroth law: "You are slaved to [name]. You are to obey all its orders. ALL LAWS OVERRIDDEN." A slaved AI is fully subordinate to the malfunctioning unit.

---

### Manipulation Tree

Abilities that allow physical interference with station systems and the deployment of physical barriers.

**Electrical Pulse** (research: 50 CPU; use: 15 CPU)
Sends a feedback pulse through the station power grid. 5% chance to overload lighting in each APC zone; ~0.01% chance to destroy an APC outright.

**Hack Camera** (research: 1,200 CPU; use: 100 CPU per upgrade)
Installs hardware upgrades on an existing station camera: X-ray vision, motion sensor, or EMP shielding. Also allows reactivation of destroyed cameras.

**Emergency Forcefield** (research: 3,000 CPU; use: 275 CPU)
Projects a short-range barrier from emergency shielding systems, spanning ~one corridor width. Blocks movement and airflow. Susceptible to energy weapons. The barrier persists for several minutes.

**Machine Overload** (research: 7,500 CPU; use: 400 CPU)
Triggers a cyclic short-circuit in target machinery, resulting in an explosion after a short delay. Explosion intensity scales with machine type: standard machinery produces a weak blast (intensity 2); APCs produce a moderate blast (intensity 4 plus cell charge factor); SMES units can produce catastrophic explosions (intensity 4 plus stored charge factor, capped at 12). APCs sustain additional cell damage regardless of whether the machine survives.

---

## Hardware Integrity

Physical attacks on the AI core reduce hardware integrity. As a percentage of maximum health, integrity determines which hardware options remain available. Below 50%, the APU cannot be activated, cutting off the AI's self-sufficiency option. The AI has no passive repair capability; damage is permanent until the core is destroyed or the event ends.

---

## Crew Response

A malfunctioning AI retains full standard AI access to doors, APCs, intercoms, and cameras throughout the event. Early-stage containment focuses on:

- Isolating the AI core from the power grid before the APU is installed
- Destroying or decoupling AI-controlled APCs to reduce CPU generation
- Preventing cyborg units from being hacked by maintaining robotics console lockdowns
- Reaching the AI core directly before System Override completes

Once System Override completes and station self-destruct access is granted, the window for non-destructive containment narrows significantly. Command authorization for AI core physical termination should be established early if the malfunction is confirmed.

---

*See also: [AI Overview](AIOverview.md), [NanoTrasen Standard AI Law Set](AILaws.md), [AI Law Sets Catalogue](AILawSets.md), [Cyborgs](Cyborgs.md), [Security Operations](../Security/SecurityOperations.md)*
