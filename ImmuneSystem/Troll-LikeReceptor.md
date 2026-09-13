<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
**Table of Contents**  *generated with [DocToc](https://github.com/thlorenz/doctoc)*

- [Toll-Like Receptors (TLRs)](#toll-like-receptors-tlrs)
  - [Structure](#structure)
  - [Family Members & Ligands](#family-members--ligands)
  - [Two Signaling Pathways](#two-signaling-pathways)
  - [Key Functional Outputs](#key-functional-outputs)
  - [Linking Innate to Adaptive Immunity](#linking-innate-to-adaptive-immunity)
  - [Clinical & Therapeutic Relevance](#clinical--therapeutic-relevance)
  - [Relationship to NOD-Like Receptors (NLRs)](#relationship-to-nod-like-receptors-nlrs)

<!-- END doctoc generated TOC please keep comment here to allow auto update -->

# Toll-Like Receptors (TLRs)

Toll-Like Receptors (TLRs) are a family of **type I transmembrane [pattern
recognition receptors](./PatternRecognitionReceptor.md)** that detect 
pathogen-associated Molecular Patterns (PAMPs) and damage-associated Molecular 
Patterns (DAMPs) at the **cell surface** or within **endosomes/lysosomes**. 
They are the membrane-level complement to the [cytosolic](Cytosol.md) 
[NOD-Like Receptors (NLRs)](./NOD-LikeReceptor.md). 
  
They were first identified in *Drosophila* (fruit flies) as regulators of 
embryonic polarity and later linked to antifungal immunity; the mammalian family 
was characterized in the late 1990s (Medzhitov, Janeway, and others).

## Structure

All TLRs share a three-part architecture:

| Domain                                       | Location      | Function                                                                              |
|----------------------------------------------|---------------|---------------------------------------------------------------------------------------|
| **LRR ectodomain**                           | Extracellular | Horseshoe-shaped, composed of tandem leucine-rich repeats; mediates PAMP/DAMP binding |
| **Transmembrane helix**                      | Membrane      | Anchors the receptor                                                                  |
| **TIR domain** (Toll/IL-1 Receptor homology) | Cytoplasmic   | Recruits adaptor proteins to initiate signaling                                       |

TLRs typically function as **dimers** — either homodimers (TLR4, TLR3) or
heterodimers (TLR2/1, TLR2/6, TLR2/10) — with each dimer having distinct ligand
specificity.

## Family Members & Ligands

A ligand (from Latin ligare, "to bind") is any molecule that binds to a specific 
partner molecule, usually a protein, to form a complex and trigger a biological 
effect.  

**10 in humans** (TLR1–TLR10); **12 in mice** (adds TLR11, TLR12, TLR13).

| TLR   | Localization | Key Pattern Recognition Receptors                          | Source                              |
|-------|--------------|------------------------------------------------------------|-------------------------------------|
| TLR1  | Cell surface | Triacyl lipoproteins (with TLR2)                           | Bacteria                            |
| TLR2  | Cell surface | Diacyl lipoproteins, LTA, PGN, zymosan, mannan, tGPI-mucin | Bacteria, fungi, parasites, viruses |
| TLR3  | Endosome     | Double-stranded RNA (dsRNA)                                | Viruses                             |
| TLR4  | Cell surface | **LPS** (lipopolysaccharide), envelope proteins            | Gram⁻ bacteria, viruses             |
| TLR5  | Cell surface | Flagellin                                                  | Bacteria                            |
| TLR6  | Cell surface | Diacyl lipoproteins (co-receptor with TLR2)                | Bacteria                            |
| TLR7  | Endosome     | Single-stranded RNA (ssRNA)                                | RNA viruses                         |
| TLR8  | Endosome     | ssRNA (human-specific)                                     | RNA viruses                         |
| TLR9  | Endosome     | Unmethylated CpG DNA                                       | Bacteria, DNA viruses, parasites    |
| TLR10 | Cell surface | PAM₃CSK₄ (synthetic); role still debated                   | —                                   |

**Damage-associated molecular patterns (DAMPs)** also activate TLRs — notably
TLR2 and TLR4 respond to heat-shock proteins, HMGB-1, histones, S100 proteins,
and extracellular DNA/RNA, linking sterile inflammation to TLR signaling.

## Two Signaling Pathways

**1. MyD88-dependent pathway** (all TLRs except TLR3; TLR4 uses it partially)

```
Ligand → TLR dimerization → TIRAP/MAL → MyD88 → IRAK4/IRAK1 → TRAF6
  → IKK complex → NF-κB (p65/p50) + MAPKs (p38, JNK, ERK)
  → Transcription: IL-6, TNF-α, IL-1β (proform), chemokines, co-stimulatory molecules
```

- Fast (minutes); dominant at the cell surface
- TIRAP (MAL) is the bridging adaptor for TLR2/1, TLR2/6, and TLR4 at the plasma
  membrane

**2. TRIF-dependent pathway** (TLR3 exclusively; TLR4 partially)

```
Ligand → TLR dimer (endosome) → TRAM → TRIF → TBK1 → IRF3/IRF7
  → Type I interferons (IFN-α/β)
TRIF → RIP1 → RIP2 → TAK1 → NF-κB
  → Additional inflammatory cytokines
```

- Slower (hours); occurs in endosomes after TLR internalization
- TLR3 is the **sole** TRIF-dependent TLR — critical for antiviral responses
- TLR4 is unique in using **both** pathways (MyD88 at the surface, TRIF in
  endosomes)

## Key Functional Outputs

| Output                                              | Pathway       | Consequence                                       |
|-----------------------------------------------------|---------------|---------------------------------------------------|
| **Pro-inflammatory cytokines** (TNF-α, IL-6, IL-1β) | MyD88 → NF-κB | Acute inflammation, fever, sepsis risk            |
| **Type I interferons** (IFN-α/β)                    | TRIF → IRF3/7 | Antiviral state, dendritic cell maturation        |
| **Co-stimulatory molecules** (CD80, CD86)           | Both          | Bridging to adaptive immunity (T cell activation) |
| **Chemokines**                                      | Both          | Recruitment of additional immune cells            |

## Linking Innate to Adaptive Immunity

TLRs are expressed on **dendritic cells**, **macrophages**, and **[B cells](./B-Cell.md)**, 
the key antigen-presenting cells. Upon TLR activation:

1. APCs upregulate MHC and co-stimulatory molecules
2. Cytokine milieu (IL-12, type I IFN, IL-6) directs **naïve T cell polarization
   ** (Th1, Th2, Th17, Treg)
3. B cells receive TLR-derived signals that promote class-switch recombination
   and antibody production

This is why TLRs are sometimes called the **"bridge"** between innate and
adaptive immunity.

## Clinical & Therapeutic Relevance

- **Sepsis / endotoxemia:** TLR4–LPS axis is the primary driver; anti-TLR4
  strategies are under investigation
- **Autoimmune diseases:** TLR7 (SLE — anti-dsRNA autoantibodies + TLR7), TLR9 (
  RA, SLE — CpG DNA), TLR4 (atherosclerosis)
- **Vaccines:** TLR agonists as **adjuvants** — CpG ODN (TLR9),
  imiquimod/resiquimod (TLR7/8), R848 (TLR7), monophosphoryl lipid A (TLR4)
- **Cancer:** TLR agonists (CpG, imiquimod) used topically and in adjuvant
  settings; TLR4 inhibitors explored for tumor-associated inflammation
- **Genetic defects:** TLR4 knockout mice are resistant to LPS but susceptible
  to Gram⁻ bacteria; MyD88 deficiency in humans → recurrent pyogenic infections
  with paradoxically low autoimmunity risk

## Relationship to NOD-Like Receptors (NLRs)


| Feature     | TLRs                                            | NLRs                                                           |
|-------------|-------------------------------------------------|----------------------------------------------------------------|
| Location    | Membrane (surface or endosomal)                 | Cytosol                                                        |
| Ligands     | PAMPs + DAMPs (lipids, proteins, nucleic acids) | PAMPs + DAMPs (peptidoglycan, flagellin, K⁺ efflux, ROS)       |
| Adaptors    | MyD88, TIRAP, TRIF, TRAM                        | ASC, RIP2                                                      |
| Key outputs | NF-κB, IRFs, MAPKs → cytokines, IFNs            | NF-κB (NOD1/2), inflammasome → IL-1β/IL-18, pyroptosis (NLRP3) |
| Timing      | First wave (surface sensing)                    | Second wave (cytosolic confirmation)                           |

Together, TLRs and NLRs form a **two-compartment surveillance system**: TLRs
sound the initial alarm at the membrane, and NLRs confirm the threat
intracellularly before triggering the full inflammatory cascade (including the
inflammasome). This redundancy ensures robust pathogen detection while limiting
false-positive autoinflammation.
