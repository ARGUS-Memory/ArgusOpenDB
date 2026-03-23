[OOC Reference](README.md) > Resizing

# Resizing

The resize system allows crew members to change physical scale, affecting appearance, interactions, and eligibility for predator-prey size-based mechanics. Size is expressed as a multiplier relative to standard (1.0).

---

## Size Tiers

| Name | Multiplier | Notes |
|---|---|---|
| Tiny | Below 0.5 | Very small; can be picked up and swallowed by normal-sized individuals |
| Small | 0.5 | Half standard size |
| Normal | 1.0 | Standard station crew size |
| Big | 1.5 | Larger than standard |
| Macro | 2.0 | Maximum standard size; can swallow normal-sized individuals |

---

## Size Limits

In standard station areas, size ranges from 0.25 (25%) to 2.0 (200%). In designated areas with expanded size permissions (dormitories and certain unrestricted zones), size can range from 0.01 (1%) to 6.0 (600%).

---

## Mechanical Effects

**Swallowing eligibility:** A predator can swallow prey whose effective size is smaller than their own. At standard station size limits, a macro (2.0) can swallow a normal (1.0), and a normal can swallow a small (0.5) or tiny. Size differences within the same tier typically do not allow swallowing.

**Being picked up:** A crew member whose size is 0.5 or less relative to another crew member can be picked up by that individual. The larger crew member scoops the smaller into a carrying position. Both parties must have pickup mechanics preferences enabled.

**Damage scaling in bellies:** Digestion damage within a belly is scaled by the size ratio between predator and prey. Larger predators process smaller prey more efficiently per tick.

**Sprite scaling:** Visual representation scales proportionally with the size multiplier. Movement animations are scaled accordingly.

**Stepping:** Macro-sized crew may affect smaller crew members through movement (stepped-on mechanics). This requires both parties to have the relevant preferences enabled.

---

## Size Change Mechanics

Size changes are animated over a brief transition (approximately 0.25 seconds per size unit of change). Visual scale is applied through a transform matrix.

If a size change exceeds 0.3 multiplier units in a single step, worn clothing may be stripped as it no longer fits the new dimensions.

Size changes through belly modes (Shrink, Grow, Size Steal) apply incrementally at 1% per tick until the belly's configured target size is reached. Direct resize is instantaneous and applies the full multiplier.

Crew resizing preferences control whether a character can be resized by external means (belly modes, items). Crew who have opted out cannot be resized by others without their preference being changed.

---

## Effective Size Calculation

A crew member's effective size for swallowing and size-comparison purposes is their base size multiplier modified by species-specific offsets if applicable. Species with unusual physical proportions may have a modifier that raises or lowers their effective size relative to their visual scale.

---

*See also: [Vore Overview](VoreOverview.md), [Belly Configuration](BellyConfiguration.md)*
