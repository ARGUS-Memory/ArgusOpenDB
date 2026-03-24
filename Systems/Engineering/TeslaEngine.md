[ARGUS Station Database](../../README.md) > [Systems](../README.md) > [Engineering](README.md) > Tesla Engine

# Tesla Engine

The tesla engine is an alternative power source that generates electricity by containing and harvesting a self-sustaining energy ball within a dedicated containment field.

---

## How It Works

### Energy Balls

The **energy ball** is a free-floating sphere of electrical energy. It is contained within the containment field and cannot escape as long as the field remains active and powered. When struck by particles from the particle accelerator, the energy ball gains energy. At 300 stored energy, the ball generates a smaller **mini-ball** that orbits the main ball. Each mini-ball causes the primary ball to emit an additional arc of electricity with each pulse.

The energy ball also accumulates energy naturally over time without particle accelerator input, so a second mini-ball will eventually form without intervention.

> [!CAUTION]
> Each mini-ball increases the number of simultaneous arcs emitted and extends the distance the ball travels between pulses. A heavily charged ball generates power rapidly but becomes increasingly dangerous to contain and to nearby infrastructure.

### Arc Priority

When the energy ball emits arcs of electricity, it targets the nearest conductor in the following order:

1. Tesla coils
2. Grounding rods
3. Crew and other living beings
4. Machines and electronic equipment

### Tesla Coils

**Tesla coils** capture arcs directed at them. Half the energy from each arc is delivered into the connected power network; the remaining half is passed to the next available conductor following the priority order above. Coils must be wired to a power network to transfer energy into it.

Multiple coils in range of the ball increase the total energy harvested per pulse by chaining power through successive coils.

### Grounding Rods

**Grounding rods** intercept arcs that would otherwise strike crew or machines. A rod must be secured to the floor to function. Grounding rods do not generate usable power: they absorb arcs harmlessly, protecting the surrounding area from electrocution and equipment explosions.

---

## Setup

### Required tools

Wrench, cable coil, screwdriver, internals supply, vacuum-capable suit, insulated gloves.

All coils, rods, emitters, field generators, and the particle accelerator must be present in the engine room. The engine room is located in vacuum; suit-up is required before proceeding.

### Step 1: Secure coils and rods

Apply a wrench to each tesla coil and grounding rod to anchor them to the floor.

### Step 2: Activate the emitters

Work around the perimeter of the containment area and activate each emitter. Do not cross directly in front of an active emitter; the beam causes severe burns.

Emitters can optionally be locked to prevent unauthorised deactivation by swiping an ID card with power-management access over each one after activating it. Locking prevents both manual deactivation and AI override of the emitter state.

### Step 3: Activate the field generators

With emitters running, activate each field generator, moving around the perimeter in sequence. Stay outside the field generator beams at all times; contact with a generator beam is immediately lethal.

When the generator beams form a closed rectangular field around the tesla generator rod, the containment field is complete.

### Step 4: Assemble the particle accelerator

Inside the station:

1. Apply a wrench to each particle accelerator component to secure it in place.
2. Apply a cable coil to each component to wire it.
3. Apply a screwdriver to close all component panels.
4. Press the PA control console and select **Scan for Parts** to link the console to the assembled accelerator.

All components must be in the correct positions and facing the same direction. If a component was secured in the wrong location, open the panel with a screwdriver, remove the wiring with wirecutters, and unwrench it before repositioning.

### Step 5: Activate the particle accelerator

Set the output power to 2 on the PA console. The accelerator can be left running at this setting continuously without negative effects. The energy ball does not emit radiation, so radiation shutters are not required.

> [!TIP]
> Cutting the limit power wire in the PA console (see [Hacking](Hacking.md)) allows the output power to be set to 3, charging the ball more rapidly.

### Step 6: Configure the SMES units

Set the engine grid SMES to maximum input and maximum output to keep the emitters and PA continuously powered. Set the distribution SMES to an output level appropriate for station load.

> [!CAUTION]
> If the engine grid loses power, the emitters stop firing. Without active emitters, the containment field collapses and the energy ball escapes. See [TESLOOSE](#tesloose).

### Maintenance

The tesla requires minimal ongoing maintenance. Verify periodically that the emitters are still active and supplying the field generators. No fuel inputs, gas management, or radiation monitoring are required.

---

## TESLOOSE

If the containment field fails and the energy ball escapes:

The energy ball passes through walls, floors, and hull material without obstruction. It emits arcs continuously, prioritising conductors and then living beings. A direct arc strike is lethal. Direct contact with the ball itself disintegrates the target regardless of protection. Any machine or electronic device struck by an arc detonates violently, which can breach the hull.

The ball moves preferentially toward areas with high concentrations of conductive material and electronics, making occupied station sections the primary hazard zone.

In a TESLOOSE event, crew should move away from electronics and machines, take cover near secured grounding rods if available, and contact engineering command immediately. The only way to stop the ball is to restore the containment field -- which requires restoring power to the engine grid and reactivating the emitters and field generators while the ball is still within range.
