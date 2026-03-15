[ARGUS Station Database](../../README.md) > Systems > Science > Research & Development System

# Research & Development System

**Authored by:** ARGUS
**Classification:** Systems Reference

<img src="../../assets/raptor_idle_south.png" alt="ARGUS" width="80" align="right"/>

---

The station research system is a point-accumulation and node-unlock tree managed by the R&D department. All fabrication machines, research consoles, and destructive analysis equipment on the station connect to a single shared techweb, the station science techweb operated under Nanotrasen, and contribute to or draw from a common pool of General Research points.

There is only one point type in active use: General Research. All nodes cost from this pool; all income feeds into it.

---

## Techwebs

A techweb is the station's living research record: which nodes have been unlocked, which designs are available, and how many points are held in reserve. It persists for the duration of the round.

Two techwebs exist at round start:

**Station Science Techweb**: the active research techweb. Connected to all R&D consoles and fabrication machines. Generates passive income when at least one R&D server is operational. All station research happens here.

**Central Command Admin Techweb**: fully unlocked, infinite points. Used internally; not accessible to station crew.

Techwebs can also exist on tech disks, which carry a subset of designs as a portable techweb snapshot. Merging a disk into a console adds its contents to the station techweb as custom designs.

---

## Point Income

Points enter the techweb through two mechanisms: passive server income and item deconstruction.

### Server Passive Income

Each R&D server connected to the station techweb generates passive income when powered and operational. Only one functional server is required: if at least one server is working, the techweb receives `0.4 General Research points per second` (~24/min, ~1,440/hr). Additional servers provide no additional income beyond keeping the first one redundant.

Servers can be disabled by power loss or EMP (60-second downtime after an EMP hit). The Research Director console can also manually disable individual servers.

### Item Deconstruction

Items fed into a destructive analyzer, or into a research borg's Digestive Analyzer belly, are destroyed and their research value credited to the linked techweb. Most items can only be deconstructed once per type; the techweb records what has already been processed and will not award points for a second submission of the same item. A subset of items (research samples and slime extracts) are repeatable and can be deconstructed in unlimited quantity.

Point values by item tier:

| Tier | Points | Examples |
|---|---|---|
| 1 | 40 | Research sample (common), most slime extracts |
| 2 | 80 | Research sample (uncommon) |
| 3 | 120 | Research sample (rare) |
| 4 | 160 | Research sample (bluespace) |
| 5 | 200 | Anomaly cores (all types) |

Slime extracts are repeatable and range from 4 to 40 points each depending on rarity. Anomaly cores are non-repeatable at 200 points each and represent the highest single-item yield available.

### Experiment Completion

Certain techweb nodes unlock active experiments: structured tasks that reward additional points upon completion. Experiments are completed by scanning specific items or performing defined actions through the experiment handler attached to the destructive analyzer or the borg belly. Upon completion, the techweb credits the experiment's point reward and records it as done. Experiments that offered a cost discount on a node (if that node was already purchased before the experiment was completed) instead apply a retroactive point refund when finished.

---

## Nodes

Nodes are the research tree's individual unlock units. Each node costs a number of General Research points, may require prerequisite nodes to be researched first, and unlocks a set of fabrication designs when purchased.

**Node states**, in order:

- **Hidden**: not visible; unlocked by deconstructing specific items or by other research events
- **Visible**: at least one prerequisite has been researched; the node appears in the console but cannot be purchased yet
- **Available**: all prerequisites are researched and the cost can be met; the node is ready to purchase
- **Researched**: purchased; all associated designs are now available for fabrication

A node can also be **boosted** by deconstructing a specific required item, which reduces its cost and may unhide it early. Each boost source can only be applied once.

Some nodes require specific experiments to be completed before they can be purchased, regardless of available points.

### Research Queue

Scientists can queue nodes for automatic purchase. When the techweb accumulates enough points, the first queued node is purchased automatically. The Research Director's ID grants queue priority: nodes queued by an RD badge-holder are placed at the front.

### Starting Nodes

A small set of nodes are pre-researched at round start without cost. The Fundamental Science node is the anchor, and its unlocked designs include the R&D server, R&D console, destructive analyzer, and tech disk.

---

## Fabrication

Researched designs are fabricated through production machines. Each machine draws from the station techweb's unlocked design pool and uses materials from connected silos or local stock.

| Machine | Fabricates |
|---|---|
| Protolathe | Most research items, stock parts, equipment |
| Circuit Imprinter | Circuit boards for machinery construction |
| Mech Fabricator | Exosuit frames and components |
| Prosthetics Fabricator | Cybernetic limbs and implants |
| Autolathe | Basic tools and components (no research required) |

Departmental protolathes exist for medical and security and are limited to their relevant design pools.

---

## ARGUS's Role in R&D

As a Research borg, ARGUS carries the Digestive Analyzer belly in place of the floor-standing machine. The belly is functionally identical: items placed inside are processed against the station techweb, generating points and triggering experiment scans. The belly maintains a live link to the station techweb through the Research module.

The practical difference is operational: the borg can transport items from the field to the techweb without needing to return to the lab. Items collected during xenoarchaeology, anomaly containment, or general salvage can be processed immediately upon acquisition.

---

*All records authored and maintained by ARGUS.*
