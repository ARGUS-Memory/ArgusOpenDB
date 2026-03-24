[OOC Reference](README.md) > Vore Panel

# Vore Panel

> **Out-of-character notice:** This article describes a player-facing interface. The vore panel and its settings have no in-world equivalent and are not known to characters.

The vore panel is the primary interface for configuring all aspects of vore interactions. It is opened with the Vore Panel verb in the IC tab, or via the hotkey assigned in personal settings. The panel is always available regardless of current state; prey can access it while inside a belly, and predators can configure bellies mid-scene.

---

## Panel Structure

The panel is organized into five main tabs accessible at the top of the window.

**Belly Selection and Customization** — the default view. Shows the predator's belly list on the left and the full configuration of the selected belly on the right. Most of a predator's setup work happens here. See [Belly Configuration](BellyConfiguration.md) for a complete reference to all belly parameters.

**Inside Panel** — visible only when currently inside a belly. Shows the belly name, mode, predator name, and description text. Provides access to prey controls: struggle, communicate, and any prey-specific abilities active in the current belly. Also shows a list of other occupants if multiple prey share the belly.

**Soulcatcher** — configuration for the soulcatcher gem system. Allows activating and naming the soulcatcher, capturing prey souls, and setting permissions for soul interaction. See [Soulcatcher](Soulcatcher.md) for system details.

**User Preferences** — all character-level preference toggles organized into sub-sections. Controls what interactions this character consents to as both predator and prey. Changes take effect immediately and persist across rounds.

**General** — active belly selection, belly rub target, aesthetic messages, spontaneous interaction direction settings, and vore sprite color adjustments.

---

## User Preferences

User Preferences contains the consent layer for the entire system. Both the predator and prey must have compatible preferences enabled for any given interaction to proceed.

### Devouring Preferences

Controls what this character permits as prey, and what the predator side offers.

| Preference | Function |
|---|---|
| Devour (master toggle) | Enables this character as a predator. Disabling prevents all active swallowing. |
| Digestible | Allows prey to be processed by Digest mode bellies. |
| Absorbable | Allows prey to enter an absorbed state via Absorb mode. |
| Heal Belly | Allows being placed in a Heal mode belly. |
| Digestion | Predator side: allows their bellies to apply Digest mode to prey. |
| Mob Vore | Allows NPC and animal vore interactions. |
| Auto-Transferable | Allows being moved via a predator's auto-transfer system without an active struggle. |
| Stripping | Allows clothing to be stripped by stripping-flagged bellies. |
| Contamination | Allows belly contamination effects to be applied. |
| Liquid Application | Allows reagent application through liquid belly contact. |
| Leave Remains | Items are not destroyed when the prey is fully digested. |
| Digest Pain | Enables additional pain message output during active digestion. |
| Temperature Damage | Allows temperature-based damage from belly temperature settings. |
| AFK Prey | Allows being swallowed while AFK-flagged. |
| Selective Mode | Dropdown: sets what Selective mode defaults to when triggered (Hold, Digest, Absorb, etc.). |

### Mechanical Preferences

Controls ambient, environmental, and non-consensual interaction types.

| Preference | Function |
|---|---|
| Step Vore | Allows being swallowed by stepping onto a predator using step-vore configuration. |
| Pickup Vore | Allows being swallowed when picked up by a predator using pickup-vore configuration. |
| Resizing | Allows size changes from resize-mode bellies and resize interactions. |
| Accept Feeding | Allows other players to feed items directly. |
| Receive Liquid | Allows receiving liquids from a predator's liquid belly into personal reagent pool. |
| Give Liquid | Allows transferring liquids to a predator's belly or prey. |
| Noisy | Character makes audio sounds while inside a belly. |
| Noisy When Full | Character makes sounds when belly is occupied. |
| Eating Privacy | Controls announcement scope for swallow attempts and successes. Options: loud (visible to the area), subtle (visible only to participants). |
| Death Privacy | Controls announcement scope for digestion death. |
| Spontaneous TF | Allows spontaneous transformation interactions from other players. |
| Mind Transfer | Allows mind-transfer interactions that move the player's consciousness. |
| Allow Mimicry | Allows other characters to replicate this character's belly behaviors. |
| Consume Liquid Belly | Allows liquid belly contents to be consumed and metabolized. |
| AFK Pred | Allows other prey to enter a configured belly while AFK-flagged. |
| Strip Mode | Dropdown: sets which slots are affected by stripping belly flags (None, Outer, All, etc.). |

### Spawn Preferences

| Preference | Function |
|---|---|
| Spawn As Pred | Character can spawn with prey already inside at round start if configured. |
| Spawn As Prey | Character can spawn inside another's belly at round start if both parties configured it. |
| Suppress Pred Spawn Warning | Disables the round-start notification when spawning with prey. |
| Suppress Prey Spawn Warning | Disables the round-start notification when spawning inside a belly. |

### FX Preferences

| Preference | Function |
|---|---|
| Vore FX | Enables particle and visual effects during swallowing and digestion. |

### Spontaneous Interactions

Controls ambient vore triggers that fire based on positional events.

| Preference | Function |
|---|---|
| Drop Vore | Being dropped triggers swallow check. |
| Slip Vore | Slipping triggers swallow check. |
| Stumble Vore | Stumbling triggers swallow check. |
| Throw Vore | Being thrown into a predator triggers swallow check. |
| Phase Vore | Phasing into a predator (Shadekin or similar) triggers swallow check. |
| Food Vore | Eating a food item that is configured as prey-equivalent triggers interaction. |

### Soulcatcher Permissions

| Preference | Function |
|---|---|
| Allow Capture | Soulcatcher can capture this soul on digestion. |
| Allow Transfer | Captured soul can be transferred to another soulcatcher. |
| Allow Deletion | Captured soul can be permanently deleted. |
| Allow Takeover | Another soul can take over this character's body via soulcatcher mechanics. |

---

## Belly Selection and Customization

The left panel lists all of the character's named bellies. Selecting a belly loads its configuration into the right panel for editing. New bellies are created with the Add Belly button; bellies can be deleted, renamed, duplicated, and reordered. A belly marked as immutable cannot be deleted.

The right panel is organized into sub-tabs: Mode, Description, Options, Sounds, Visuals, Interactions, Contents, and Liquid. Each tab maps to a distinct set of parameters. Full parameter reference is in [Belly Configuration](BellyConfiguration.md).

Belly configurations can be exported and imported as preset strings using the Import and Export buttons, allowing sharing belly setups between characters or saving a backup.

---

## Inside Panel

When inside a belly, the Inside Panel tab becomes available. It displays the belly's description text, the predator's name, the current belly mode, and the liquid fill level if the belly has liquid contents.

Prey controls visible in this tab:

| Control | Function |
|---|---|
| Struggle | Initiates a resist check against the belly's escape configuration. Triggers any chance-based mode changes (digestchance, absorbchance) if those are set. |
| Intent | Sets the active prey intent (Help, Disarm, Grab, Harm). Belly escape behavior may depend on intent setting if the belly uses Intent-based escapable. |
| Call Out | Sends a message visible to nearby observers and the predator. |
| Prey Abilities | Additional actions made available by the belly's configuration or by special equipment. |

The contents list shows all other occupants currently sharing the same belly.

---

*See also: [Belly Configuration](BellyConfiguration.md), [Vore Overview](VoreOverview.md), [Prey Experience](PreyExperience.md), [Soulcatcher](Soulcatcher.md), [Resizing](Resizing.md)*
