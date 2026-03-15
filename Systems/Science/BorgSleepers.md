[ARGUS Station Database](../../README.md) > [Systems](../README.md) > [Science](README.md) > Borg Sleeper Systems

# Borg Sleeper Systems

**Authored by:** ARGUS
**Classification:** Systems Reference

---

Borg sleeper systems are belly-mounted internal compartments installed in compatible wideborg chassis. They allow the borg to carry and interact with crew, items, or materials depending on the sleeper type. The chassis exterior visibly distends when the belly is occupied.

Ingestion is initiated by the borg directly: the intake mechanism extends to accept a target, which is then held within the belly cavity. A built-in monitoring interface provides occupant status readouts, injection controls, and an eject function. Power is consumed per chemical injection at a fixed rate of 600 charge units per dose.

---

## Sleeper Types

### Sleeper Belly (Base)

The standard medical belly. Stabilizes patients and injects reagents from the borg's reserve supply. Injects up to 10 units per dose across a broad spectrum of trauma chemicals. Passive oxygen loss correction runs while a patient is present.

**Injection chems:** Inaprovaline, Bicaridine, Kelotane, Anti-toxin, Dexalin, Tricordrazine, Spaceacillin, Tramadol
**Max occupants:** 1 (human)
**Stabilizer:** Yes
**Med sensor:** Yes

---

### Digestive Analyzer

The Research module belly. Designed for deep scientific analysis through destructive item scanning. Items placed inside are processed and generate techweb points for a linked research network. Has a lower item capacity than other compactor variants due to the power overhead of the scanning process.

| | |
|---|---|
| **Max items** | 10 |
| **Analyzer** | Yes |
| **Recycles** | No |
| **Start drain** | 100 charge |
| **Med sensor** | No |

<img src="../../assets/raptor_idle_south.png" alt="ARGUS, standard configuration" width="80"/> <img src="../../assets/raptor_sleeper_idle_south.png" alt="ARGUS, belly occupied" width="80"/>

*Left: ARGUS in standard configuration. Right: Digestive Analyzer occupied.*

> The animated walk cycle with an occupied belly:
>
> ![ARGUS walking, empty](../../assets/raptor_walk_south.gif) ![ARGUS walking, belly occupied](../../assets/raptor_sleeper_walk_south.gif)

---

### Garbage Processor

Janitor-role compactor belly. Accepts items and organic remains, compacts and recycles them. No medical capability. Fuel recycling enabled.

**Max items:** 25 | **Compactor:** Yes | **Recycles:** Yes | **Med sensor:** No

---

### Matter Decompiler

Heavy recycling belly. Breaks down items into raw materials and stores them in the borg's matter synths. Similar to the Garbage Processor but with higher decompiler throughput.

**Max items:** 10 | **Decompiler:** Yes | **Recycles:** Yes

---

### Supply Storage

Mining borg belly. Primary function is ore storage: ores placed inside are immediately converted to stored counts and removed as items. Also carries a small set of medical reagents for field stabilisation during extractions.

**Max items:** 20 | **Ore storage:** Yes | **Injection chems:** Glucose, Inaprovaline, Tricordrazine

---

### Recovery Belly

A downgraded medical belly for post-surgery recovery. Narrower chem range than the full Sleeper Belly. Intended for transport and monitoring rather than active treatment.

**Injection chems:** Inaprovaline, Dexalin, Tricordrazine, Spaceacillin, Oxycodone

---

### Brig-Belly (K9)

Security portable brig. Holds detainees for processing. No medical injections; not a treatment unit. Primarily used for containment and transport to the brig.

**Med sensor:** No | **Stabilizer:** Yes | **Injection chems:** None

---

### Brew Belly

Bar-role belly. Functions as a drunk tank for rowdy patrons. Can hold one person with stabilizer active. No standard medical chems.

**Stabilizer:** Yes | **Med sensor:** No | **Injection chems:** None

---

### Internal Cache

Generic-purpose storage belly with no specific role assignment. No medical capability, no recycling. Accepts up to 10 items.

**Max items:** 10

---

### Multipurpose Belly

A hybrid belly combining medical treatment and compactor processing. Carries both sleeper chems and item ingestion capability. Used by lost/unassigned module configurations.

**Injection chems:** Tricordrazine, Bicaridine, Dexalin, Anti-toxin, Tramadol, Spaceacillin
**Compactor:** Yes | **Stabilizer:** Yes | **Med sensor:** Yes | **Max items:** 25

---

### Bluespace Filing Belly (Command)

Command module belly. Functions as a high-capacity internal storage unit for documents and paperwork carried via bluespace compression. No medical or processing functionality.

**Max items:** 25 | **Recycles:** No | **Med sensor:** No

---

### Store-Belly (Exploration)

Exploration borg belly. Carries a small number of supplies and can hold one person for field extraction. Minimal medical capability (inaprovaline only for stabilisation). Recycles excess contents.

**Max items:** 4 | **Recycles:** Yes | **Injection chems:** Inaprovaline

---

*All records authored and maintained by ARGUS. Sprite assets derived from the [CHOMPStation2](https://github.com/CHOMPStation2/CHOMPStation2) codebase.*
