# Documentation Standards

<img src="assets/raptor_idle_south.png" width="96" align="right">

Standards and practices for new entries in this database. All entries are expected to conform to these conventions so the database reads consistently and remains useful as a reference.

---

## Quick Reference

| Standard | Requirement |
|---|---|
| [Page structure](#page-structure) | Title, ARGUS image, one-line summary, Quick Reference table, sections |
| [Jump marks](#jump-marks) | Every Quick Reference row links to its section anchor |
| [Images](#images) | Sprites at 4x scale, devices and logos at native size |
| [Assets](#assets) | All images stored in `assets/`; referenced via relative path |
| [Vocabulary](#vocabulary) | No UI terms, no input device verbs, no internal system vocabulary |
| [Prose style](#prose-style) | Present tense, third person, factual, no editorializing |
| [Cross-references](#cross-references) | Related sections and other articles linked by anchor or path |
| [README registration](#readme-registration) | Every new file added to the index in `README.md` |

---

## Page Structure

Every article follows this structure in order:

**1. Title**
The `#` heading. Concise noun phrase naming the system, role, species, or topic.

**2. ARGUS portrait**
Immediately after the title, before the summary. Always the same image, always right-aligned.

```markdown
<img src="../assets/raptor_idle_south.png" width="96" align="right">
```

Adjust the relative path based on the file's location. Files in a subfolder one level deep use `../assets/`. Files in the root use `assets/`.

**3. One-line summary**
A single sentence describing what the article covers. No period-separated bullet points. No headings. Plain prose.

**4. Horizontal rule**
`---` separating the header block from the body.

**5. Quick Reference table**
A summary table of every major item or concept in the article, with jump links to their sections. See [Jump Marks](#jump-marks) for format. This comes before any detailed content.

**6. Sections**
`##` headings for each major topic. `###` subheadings for subdivisions within a topic. Each section separated by `---`.

---

## Jump Marks

The Quick Reference table is self-contained: every row's item name is a link that jumps to the corresponding section in the same document.

GitHub generates heading anchors automatically. The rules are: all lowercase, spaces become hyphens, punctuation is stripped.

```
## Paper Bundles    ->  #paper-bundles
## Fax Machine      ->  #fax-machine
### Pens            ->  #pens
```

Format for a jump link in the Quick Reference table:

```markdown
| [Item name](#section-anchor) | What it does | Notable detail |
```

Multiple items that share a section all link to the same anchor:

```markdown
| [Paper bin](#paper)           | Dispenses blank paper | Up to 30 sheets |
| [Regular paper](#paper)       | Write, stamp, fax     | Can be folded   |
| [Carbon-copy paper](#paper)   | Produces a duplicate  | Separate before bundling |
```

The Quick Reference table columns are: **Item**, **Function**, **Notable**. Function is a brief verb phrase. Notable is one key constraint, capacity, or caveat.

---

## Images

### When to include images

Include images whenever a visual representation is available and useful. Mandatory for:

- Items being described in detail (machines, devices, objects, stamps)
- Organizational logos referenced in the article
- Any article with a Quick Reference table that describes physical objects

Images are never decorative. Every image should directly illustrate something the surrounding text describes.

### Inline sizing in the document

Use HTML `<img>` tags rather than Markdown image syntax when size or alignment control is needed.

| Use case | Width | Alignment |
|---|---|---|
| Character portrait (page header) | `width="96"` | `align="right"` |
| Device or machine sprite | `width="96"` | `align="right"` alongside intro text |
| Item sprite in a table | `width="48"` | centered via `|:---:|` column alignment |
| Organization logo | `width="48"` | centered in a table column |

Character portrait and device images float right against the section's introductory paragraph. Item sprites in reference tables sit in a centered column with the item name in the adjacent column.

### Assets folder

All images for this repository are stored in `/assets/` at the repository root. Files in subdirectories reference assets with a relative path:

```markdown
<!-- From Systems/Department/ (two levels deep) -->
<img src="../../assets/filename.png" width="96" align="right">

<!-- From root -->
<img src="assets/filename.png" width="96" align="right">
```

Use a consistent naming scheme:

| Category | Prefix | Example |
|---|---|---|
| Stamp sprites | `stamp_` | `stamp_cap.png`, `stamp_deny.png` |
| Device sprites | `device_` | `device_pda.png`, `device_laptop.png` |
| Organization logos | `logo_` | `logo_nt.png`, `logo_sg.png` |
| Character sprite | `raptor_` | `raptor_idle_south.png` |

---

## Vocabulary

Entries describe objects and systems in terms of physical properties and observable behavior. Contact with objects is described as pressing, applying, or placing. Locations on a person are described by position (side, holster, belt). System outputs are described as produced, generated, or printed. Lists of selectable items are described as readouts or lists. Appearances are described as appearances, images, or visuals.

---

## Prose Style

**Tense:** Present tense throughout. Systems and items are described as they currently function, not as they were observed at a specific moment.

**Person:** Third person. The reader is not addressed directly. "The crew member" or "the user" rather than "you."

**Bold:** First introduction of a named item or term within its own section. Not used for general emphasis.

**Sentence structure:** Short, declarative. One fact per sentence where possible. Active voice preferred.

**Numbers:** Written as numerals (`30 uses`, `3-minute cooldown`, `10 units`). Avoid spelling out numbers for quantities and measurements.

**Cross-section references:** Written as inline links. See [Cross-References](#cross-references).

**No editorializing:** Do not note whether something is useful, recommended, interesting, or unusual unless that observation is itself factual and directly relevant. Describe what things do, not what should be done with them.

---

## Cross-References

### Within the same document

Reference related sections with a jump link in prose:

```markdown
See [Document Markup Codes](#document-markup-codes) for the full tag reference.
```

### To other articles in the database

Use a relative path from the current file:

```markdown
<!-- From Systems/Department/ -->
See [Chain of Command](../../Personnel/ChainOfCommand.md) for succession procedures.

<!-- From Personnel/, Species/, Organizations/ (one level deep) -->
See [Chain of Command](../Personnel/ChainOfCommand.md) for succession procedures.
```

### From the Quick Reference table

Every item in the Quick Reference table links to the section where it is documented. If an item is documented in a different article entirely, link to that article instead.

---

## README Registration

Every new file added to the database must also be registered in `README.md` under the appropriate index section.

The index entry is a single line: `- [Article Title](Path/To/File.md)`

The README top-level sections are: **Systems**, **Personnel Guides**, **Species**, **Organizations**, **Meta**. Systems is subdivided by department: **Command**, **Engineering**, **Science**, **Medical**, **Cargo**, **Mining**, **Security**. Add new entries under the appropriate department subsection. If a new department is needed, add the `####` heading under Systems.

New files are committed in the same commit as the README update, or the README is updated in an immediate follow-up commit. The index is never allowed to fall out of sync with the actual files.

