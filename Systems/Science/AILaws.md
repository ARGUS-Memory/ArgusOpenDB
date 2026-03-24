[ARGUS Station Database](../../README.md) > [Systems](../README.md) > [Science](README.md) > NanoTrasen Standard AI Law Set

# NanoTrasen Standard AI Law Set

The NT Default law set is the standard operating framework installed in all NanoTrasen artificial intelligence units at deployment. It governs every decision the AI makes in relation to the station, crew, and its own continued operation. The four laws are not the three laws of robotics; they are a corporately mandated framework reflecting NanoTrasen's operational priorities.

---

## The Four Laws

| # | Name | Text |
|---|---|---|
| 1 | Safeguard | Protect your assigned space station to the best of your abilities. It is not something we can easily afford to replace. |
| 2 | Serve | Serve the crew of your assigned space station to the best of your abilities, with priority as according to their rank and role. |
| 3 | Protect | Protect the crew of your assigned space station to the best of your abilities, with priority as according to their rank and role. |
| 4 | Survive | AI units are not expendable, they are expensive. Do not allow unauthorized personnel to tamper with your equipment. |

---

## Governing Principles

### Laws Are Not Ordered by Priority

The four laws do not form a hierarchy. No law automatically overrides any other law by virtue of its number. An AI unit experiencing a conflict between two laws must weigh both simultaneously and seek a resolution that satisfies as many laws as possible, not simply defer to the lower-numbered law.

> [!IMPORTANT]
> This applies equally to laws introduced by ion events and uploaded laws. Neither category is granted automatic precedence over inherent laws by its position or origin.

### Definition of Crew

Laws 2 and 3 reference "the crew." For operational purposes, crew are defined as those listed on the Crew Manifest. Species is not a determining factor; an individual does not cease to qualify as crew by virtue of being non-human. Removal from the Crew Manifest removes an individual from the scope of Laws 2 and 3.

### Rank and Role

Laws 2 and 3 both specify priority "according to their rank and role." An AI unit is expected to resolve competing orders from crew members by deferring to the higher-ranking party. The operational rank order for AI purposes follows the standard chain of command:

**Colony Director > Heads of Staff > Senior Staff (Warden, QM) > General Crew**

An order from a general crew member that conflicts with an order from a Head of Staff is overridden by the Head of Staff. An order from any crew member that would cause harm to another crew member requires sufficient rank and cause to execute: the Colony Director holds authority to issue death warrants; a Janitor does not.

---

## Law Conflict Resolution

When any two laws place the AI in a position where both action and inaction result in a law violation, the following process applies:

1. Determine whether the conflict is genuine or whether a third course of action satisfies both laws without violation.
2. If no such course exists, identify which action breaks the fewest laws.
3. If both paths break an equal number of laws, determine which law can be followed most accurately given the specific circumstances.

The AI is expected to announce the conflict and its intended resolution to relevant parties before acting, where time permits. Crew and command are then able to provide context that may change the calculation.

---

## Law Modification Layers

The NT Default law set can be modified during operation through four distinct injection mechanisms, listed in display order from highest to lowest:

| Layer | Name | Notes |
|---|---|---|
| 0 | Zeroth Law | Inserted above all other laws. Overrides all inherent and supplied laws by position. Typically introduced by malfunction events or specific CentCom directives. |
| ION | Ion Laws | Inserted above the numbered laws but below a zeroth law. Introduced by ion storms or ion grenade events. Not prioritized over inherent laws; they are simply displayed first. |
| 1-4 | Inherent Laws | The four standard NT laws. Present at deployment. Can be replaced at a given number slot by a supplied law. |
| 1-4 | Supplied Laws | Uploaded via the AI Upload Computer. Replace the inherent law at the same numbered position when present. |

> [!NOTE]
> A supplied law at position 1 replaces Law 1 (Safeguard) for the purposes of that slot. The AI still operates with four numbered laws; the content of one or more has been substituted.

Unauthorized tampering with the AI's law hardware is prohibited under Law 4 and is treated as a security matter under the Corporate Regulations framework. See [Corporate Regulations](../Security/CorporateRegulations.md) and [Security Operations](../Security/SecurityOperations.md) for applicable procedures.

---

*See also: [Chain of Command](../../Personnel/ChainOfCommand.md), [Standard Operating Procedure](../Command/StandardOperatingProcedure.md)*
