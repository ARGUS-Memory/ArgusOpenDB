[OOC Reference](README.md) > Prey Experience

# Prey Experience

What prey experience inside a belly, how struggle and escape work, and the message system used for belly interactions.

---

## Inside the Belly

Once swallowed, prey are inside the predator's active belly. They can observe their environment through a fullscreen overlay and receive a continuous stream of ambient messages from the belly. The specific messages depend on the belly's mode, the active message list configured by the predator, and periodic emote triggers.

Prey retain access to all standard communication (in-character speech, radio) unless the belly has sound-muffling flags active. Items in inventory remain accessible. Prey can observe other occupants of the same belly.

Damage from Digest mode is applied each tick to the prey's health pool across the configured damage types. In Hold mode, no damage occurs. The prey can monitor their own health through standard means.

---

## Struggle and Escape

Prey can struggle against confinement at any time. The outcome depends on the belly's escape configuration.

**No escape setting:** Prey cannot force release through struggle. Struggle still produces ambient messages and may trigger secondary events (belching, mode changes) at the predator's configured chances.

**Standard escape:** Any struggle attempt triggers an escape chance check. If the check succeeds, prey begins climbing out. The exit process takes time (configured by escapetime) and produces messages to both predator and nearby observers.

**Intent-based escape:** The outcome of struggle depends on the prey's active physical intent at the moment of each struggle:

| Intent | Behavior |
|---|---|
| Help | Triggers standard escape chance check |
| Hurt | Triggers standard escape chance check |
| Disarm | Triggers primary transfer chance check |
| Grab | Triggers absorb, digest, and selective mode change chances |

**Struggle outcomes (any mode):** Beyond escape, each struggle attempt can independently trigger:
- Transfer to a different belly (based on transferchance and transferchance_secondary)
- Absorption activation (absorbchance)
- Digest mode activation (digestchance)
- Mode switch to Selective (selectchance)
- Predator belch (belchchance)

**Absorbed state:** Prey in an absorbed state use a separate set of struggle messages and a separate escape chance value (escapechance_absorbed). Normal digest mechanics do not apply to absorbed prey.

---

## Message System

Belly messages use a templating system with dynamic substitutions. Predators write custom messages using pattern keywords that the system replaces with contextual values at runtime.

**Pattern substitutions:**

| Pattern | Replaced with |
|---|---|
| %belly | The belly's name |
| %pred | The predator's name |
| %prey | The current prey's name |
| %count / %countprey | Number of prey in the belly |
| %countghosts | Number of observers in the belly |
| %digestedprey | Number of fully digested prey |
| %item | Name of an item in the belly |
| %dest | Destination belly name (for transfer messages) |
| %goo | Random word from the texture word bank |
| %happybelly | Random belly sound word |
| %fat | Random body softness word |
| %grip | Random grip word |
| %cozy | Random comfort word |
| %angry | Random discomfort word |
| %acid | Random acid/liquid word |
| %snack | Random food-framing word |
| %hot | Random heat word |
| %snake | Random tube/constriction word |

These substitutions allow message text to vary naturally between triggers without repeating identical phrasing.

**Emote intervals:** Automatic belly emotes fire every 60 seconds by default (configurable). They select from the belly's configured emote list for the active mode and substitute dynamic patterns before display.

---

## Examine Messages

Observers examining a predator with occupants see contextual examine text. For normal prey above the configured bulge size threshold (default 0.25 size multiplier), the examine text notes visible fullness. For absorbed prey, the description changes to reflect a more diffuse fullness profile. Predators with the DM_FLAG_THICKBELLY flag active display reduced information to outside observers.

---

## Escape Messages

Standard system messages for escape events:

- Attempt: "%prey is attempting to free themselves from your %belly!"
- Attempt (to prey): "You start to climb out of %pred's %belly."
- Success (to pred): "%prey climbs out of your %belly!"
- Success (to prey): "You climb out of %pred's %belly!"
- Failure (to pred): "%prey's attempt to escape from your %belly has failed!"
- Failure (to prey): "Your attempt to escape from %pred's %belly has failed!"
- Outside observer: "%pred's %belly wobbles with a squirming meal."

---

## Digestion Messages

Representative examples of Digest mode messages (exact text varies by belly configuration):

- "You feel %prey's body succumb to your digestive system, which breaks it apart into soft slurry."
- "You hear a lewd glorp as your %belly muscles grind %prey into a warm pulp."
- "Your %belly lets out a rumble as it melts %prey into %goo."

---

## Absorption Messages

- To predator: "You feel %prey becoming part of you."
- To prey: "You feel yourself becoming part of %pred's %belly!"
- To absorbed prey on struggle: "You try and resist %pred's %belly, but only cause it to jiggle slightly."

---

*See also: [Vore Overview](VoreOverview.md), [Belly Configuration](BellyConfiguration.md), [Resizing](Resizing.md)*
