[ARGUS Station Database](../../README.md) > [Systems](../README.md) > [Science](README.md) > Xenobotany

# Xenobotany

The Xenoflora laboratory provides equipment for the study and genetic manipulation of plant species, including exotic off-station specimens. Xenobotanists work to identify the genetic structure of plant varieties, transfer specific traits between species, and produce novel organisms for research or distribution.

Xenobotany shares the fundamental tray mechanics documented in [Hydroponics](../Service/Hydroponics.md) but adds gene-level manipulation tools not available in the standard botany bay.

---

## Plant Genetics

Every plant variety carries 12 genes, each controlling a cluster of related traits. Gene labels are assigned at random each shift; gene F6 on one shift's label scheme might correspond to a different trait than F6 in the next shift's scheme, but within a single shift the same label corresponds to the same trait family across all plant species.

The 12 gene families and the traits each governs:

| Gene Family | Traits Controlled |
|---|---|
| **Biochemistry** | Reagent content of the fruit; gases the plant generates |
| **Hardiness** | Endurance; tolerances to toxins, pests, and weeds |
| **Environment** | Preferred temperature and light level; light tolerance range |
| **Metabolism** | Water and fertiliser requirements; ambient temperature alteration |
| **Appearance** | Visual presentation (currently unused in mechanical terms) |
| **Diet** | Gas consumption; carnivorous and parasite behaviours; water and fertiliser consumption rates |
| **Pigment** | Plant body colour; fruit colour; bioluminescence colour |
| **Output** | Power generation; bioluminescent light production |
| **Atmosphere** | Pressure tolerance; temperature deviation tolerance |
| **Vigour** | Maturation time; production interval; spread behaviour |
| **Fruit** | Juicy flag; sting injection flag |
| **Special** | Teleportation trait |

---

## Lysis-Isolation Centrifuge

The **lysis-isolation centrifuge** extracts the genetic data from a seed or cutting. The process is destructive: the seed is consumed to recover the genetic information.

Operation:

1. Insert a seed packet or cutting into the centrifuge.
2. Trigger the analysis. The centrifuge reads and stores the genetic profile.
3. Insert a flora data disk.
4. Copy the desired gene record onto the disk. One disk holds one gene.
5. Repeat with additional disks for each gene to be preserved.

The stored genetic data in the centrifuge degrades after a limited number of copy operations. Once exhausted, a new seed of the same species must be inserted and analysed to continue.

---

## Bioballistic Delivery System

The **bioballistic delivery system** applies a gene from a flora data disk to a target seed. The gene on the disk overwrites the corresponding gene family on the target seed, replacing whatever that gene controlled in the target species with the version from the source species.

Target seeds can only be overwritten a limited number of times before the seed packet degrades beyond use.

Operation:

1. Load a target seed packet into the bioballistic delivery system.
2. Insert a flora data disk carrying the gene to transfer.
3. Activate the modification. The target seed's corresponding gene is replaced.
4. Eject the seed packet and analyse it with a plant analyser to confirm the change.

---

## Gene Identification Procedure

Gene labels are random, so the identity of each labelled gene must be established each shift through systematic comparison.

1. Select two plant species with different trait profiles. Since standard station seed vendor plants share the same Hardiness, Environment, and Metabolism genes, at least one species should be exotic, mutated, or from off-station stock.
2. Obtain three or four identical seed packets from each species.
3. Using the lysis-isolation centrifuge, analyse a seed from Species A and copy each of its 12 genes onto individual data disks. Label each disk with a temporary identifier.
4. Analyse a seed from Species B with the plant analyser. Record its current traits.
5. Insert a Species B seed into the bioballistic delivery system. Apply one disk from Species A.
6. Eject the modified seed and analyse it again. Whichever trait changed identifies the gene on that disk.
7. Label the disk with the confirmed gene identity.
8. Repeat with remaining disks, switching to a fresh Species B seed when the current one can no longer accept modifications.

If applying a disk produces no observable change, the two species likely share an identical version of that gene.

The **Biochemistry** gene (reagents) has an additive transfer behaviour rather than a replacement: transferring it adds the source plant's reagent profile to the target rather than replacing the target's profile. The target plant produces both fruit types, each carrying reagents from both plants. The tradeoff is reduced vigour and potency.

---

## Dangerous Plants

### Spreading Vines

Vine-type plants carry the **Vigour** gene set for creeping or full spread. Without intervention, a vine planted in a standard tray spreads out of the tray into the surrounding environment and, given open doors, can progressively colonise station sections.

Entangled crew members receive injected reagents from the vine's fruit, which may be hazardous depending on the vine variety. A vine with carnivorous traits set to full can drain blood from captured crew.

Control methods:

- Before planting: transfer the Vigour gene from a non-spreading species into the vine to suppress its spread behaviour.
- Use the isolation trays in the Xenoflora lab for all untested specimens.
- A hatchet removes vines faster than standard tools.
- Plant-B-Gone and other herbicidal compounds kill vines on contact.
- A goat from Cargo consumes vine growth rapidly.

### Gas-Producing Plants

Some exotic species emit gases as part of their metabolic process. These gases may accumulate to hazardous pressures or concentrations before the botanist notices.

Management:

- Plant all unknown exotic seeds in isolation trays with atmospheric ports.
- Monitor the local atmospheric readout via the PDA scanner regularly while tending exotic plants.
- If a plant is confirmed to produce gas, close the isolation tray lid to contain the emissions. Note that the restricted environment may require additional fertiliser input.
- If room-level contamination has already occurred, contact Atmospherics. Phoron gas exposure requires immediate exit, decontamination, and medical evaluation.
