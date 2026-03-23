[OOC Reference](README.md) > Vore Overview

# Vore Overview

The station vore system governs the mechanics of predator-prey interactions between crew members. It covers the swallowing process, belly mechanics, and related features including resizing, soulcatchers, and absorption. Participation in the system is preference-governed on both sides; crew configure their availability through personal preference panels.

---

## Preference System

Both predators and prey must have compatible preferences enabled for an interaction to proceed. A crew member with prey availability disabled cannot be swallowed regardless of predator intent. Similarly, a predator cannot swallow others if their own predator preferences are inactive.

These preferences are configured per individual and persist across interactions. Specific belly modes and interaction types can also be restricted or allowed on a per-character basis.

---

## Swallowing

A predator initiates swallowing by attempting to devour an adjacent target. The system performs sanity checks before allowing the attempt to proceed:

- Both predator and prey must have compatible preferences active
- Neither individual may be in an absorbed state
- The target must be within one tile of the predator
- Standard stomach capacity limits apply

If checks pass, the predator begins the swallow process. Organic targets take approximately 10 seconds to fully swallow; non-humanoid targets or those meeting special conditions may be swallowed in approximately 3 seconds. Once the timer completes, the prey is transferred into the predator's selected belly.

Swallowing sounds and messages are announced to nearby observers. The prey appears inside the belly and immediately begins experiencing whatever the belly's active mode dictates.

---

## Bellies

Each predator character has one or more named belly configurations, each with independently set mode, escape settings, sounds, and behavioral options. When swallowing, the active belly at the time of ingestion determines what happens to the prey.

Belly types are broadly organized by what they do to occupants:

| Category | Modes | Summary |
|---|---|---|
| Holding | Hold | Prey is retained safely; no damage or processing |
| Digestion | Digest | Prey takes damage and is converted to nutrition |
| Nutrition theft | Drain, Absorb | Prey's nutrition is taken without immediate harm; Absorb eventually transforms the prey into an integrated state |
| Transformation | Shrink, Grow, Size Steal | Prey's size changes over time |
| Support | Heal | Predator expends nutrition to heal prey injuries |
| Containment | Egg | Prey is encased in an egg and held until release |
| Conditional | Selective | Mode toggles between the belly's default and Digest based on struggle behavior |

For full configuration parameters for each mode, see [Belly Configuration](BellyConfiguration.md).

---

## Belly Transfer

Prey can be moved between bellies. Transfer may occur through struggle (if the belly is configured with a transfer chance), direct predator action, or auto-transfer settings that fire on a timer. Transferred prey retain their current state (absorbed, normal, etc.) and immediately fall under the destination belly's settings.

Multiple prey can occupy a belly simultaneously. Each occupant is processed independently.

---

## Predator Effects

A predator with prey inside experiences a visible fullness effect proportional to the number and size of occupants. Nutrition is gained from all prey in active digestion or drain modes. Healing mode costs the predator nutrition to sustain.

Certain prey types with parasitic properties can cause the predator damage from inside if the predator's settings permit; this is a niche case and depends on individual configuration.

---

## Soulcatcher

The soulcatcher system captures a consciousness into a contained virtual space, separating it from the physical body. This is treated as a distinct system from standard vore belly mechanics. See [Soulcatcher](Soulcatcher.md).

---

## Resizing

Crew members can change size, affecting their apparent scale, movement, and eligibility for predator-prey interactions. Size changes are governed by the resize system. See [Resizing](Resizing.md).

---

*See also: [Belly Configuration](BellyConfiguration.md), [Prey Experience](PreyExperience.md), [Soulcatcher](Soulcatcher.md), [Resizing](Resizing.md)*
