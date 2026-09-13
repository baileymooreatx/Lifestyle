<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
**Table of Contents**  *generated with [DocToc](https://github.com/thlorenz/doctoc)*

- [Pattern Recognition Receptors (PRRs)](#pattern-recognition-receptors-prrs)
  - [The Five (or Six) Major Families](#the-five-or-six-major-families)
  - [Spatial Logic: Where Each Family Sits](#spatial-logic-where-each-family-sits)
  - [Detailed Family Profiles](#detailed-family-profiles)
    - [1. Toll-like Receptors (TLRs)](#1-toll-like-receptors-tlrs)
    - [2. NOD-like Receptors (NLRs)](#2-nod-like-receptors-nlrs)
    - [3. RIG-I-like Receptors (RLRs)](#3-rig-i-like-receptors-rlrs)
    - [4. C-type Lectin Receptors (CLRs)](#4-c-type-lectin-receptors-clrs)
    - [5. AIM2-like Receptors (ALRs)](#5-aim2-like-receptors-alrs)
    - [6. cGAS-STING (the DNA→IFN axis)](#6-cgas-sting-the-dna%E2%86%92ifn-axis)
  - [The Two Major Signaling Outputs](#the-two-major-signaling-outputs)
  - [The "Priming" Requirement](#the-priming-requirement)
  - [How PRRs Are Connect](#how-prrs-are-connect)
  - [Inhibitory PRRs (iPRRs)](#inhibitory-prrs-iprrs)

<!-- END doctoc generated TOC please keep comment here to allow auto update -->

# Pattern Recognition Receptors (PRRs)

Pattern Recognition Receptors (PRRs) are the molecular "sensors" of the innate 
immune system, the body's first-line, pre-existing, non-specific defense — 
present from birth, requiring no prior exposure to a pathogen, and responding 
within minutes to hours. It is "innate" (hardwired) as opposed to "adaptive" 
(learned, clonal, slow).  

PRRs are a collection of protein families expressed by virtually every nucleated 
cell (not just professional immune cells) that detect pathogen-associated 
molecular patterns (PAMPs) and damage-associated molecular patterns (DAMPs). The 
concept was formalized by **Charles Janeway in 1989**, who proposed that the 
innate immune system recognizes conserved microbial motifs rather than 
individual pathogens, a "pattern" rather than a "molecule."

They comprise a multifamily, multi-compartment surveillance network that detects 
conserved microbial and damage signals at every stage of pathogen invasion 
(outside → membrane → endosome → [cytosol](./Cytosol.md)), translates them into 
two major transcriptional programs (inflammation and antiviral), and provides
the essential "first wave" of defense that bridges to adaptive immunity. Their 
misregulation underlies immune-mediated disease.

## The Five (or Six) Major Families

| Family                                             | Abbreviation | Location                      | Primary Ligands                                                    | Key Signaling Output                                                       |
|----------------------------------------------------|--------------|-------------------------------|--------------------------------------------------------------------|----------------------------------------------------------------------------|
| **[Toll-like receptors](./Troll-LikeReceptor.md)** | TLRs         | Plasma membrane and endosomes | Lipids, lipoproteins, LPS, flagellin, dsRNA, ssRNA, CpG DNA, DAMPs | NF-κB, MAPKs, IRFs → cytokines, type I IFNs                                |
| **[NOD-like receptors](./NOD-LikeReceptor.md)**    | NLRs         | Cytosol                       | Peptidoglycan, flagellin, K⁺ efflux, ROS, toxins, ATP              | NF-κB (NOD1/2); **Inflammasome** → IL-1β, IL-18, pyroptosis (NLRP3, NLRC4) |
| **RIG-I-like receptors**                           | RLRs         | Cytosol                       | Viral RNA (short/5′-triphosphorylated dsRNA, long dsRNA)           | MAVS → NF-κB + IRF3/7 → **type I IFNs** (antiviral)                        |
| **C-type lectin receptors**                        | CLRs         | Plasma membrane               | Fungal β-glucans, mannans, glycolipids                             | SYK → CARD9 → NF-κB; phagocytosis; cytokines                               |
| **AIM2-like receptors**                            | ALRs         | Cytosol                       | Cytosolic **dsDNA** (bacterial, viral, mitochondrial)              | **Inflammasome** (AIM2) → caspase-1 → IL-1β, IL-18, pyroptosis             |
| **STING** (cGAS-STING axis)                        | —            | Cytosol → ER                  | Cytosolic dsDNA (via **cGAS** → cGAMP)                             | TBK1 → IRF3 → **type I IFNs**; NF-κB → cytokines                           |

> Some classifications fold cGAS-STING into the ALR group or treat it as a sixth
> family. Others include **OAS-like receptors (OLRs)** as a seventh. The
> five-family model above is the most widely used.

## Spatial Logic: Where Each Family Sits

The PRR system is organized by **compartment** — each family watches a
different "zone" of the cell:

```
┌─────────────────────────────────────────────────────────────────┐
│  EXTRACELLULAR / LUMEN                                          │
│  ┌─────────────────────────────────────────────────────────┐    │
│  │  TLRs (surface) + CLRs + RAGE                           │    │
│  │  → "First alarm: something is outside"                  │    │
│  └─────────────────────────────────────────────────────────┘    │
├─────────────────────────────────────────────────────────────────┤
│  PLASMA MEMBRANE                                                │
│  ┌─────────────────────────────────────────────────────────┐    │
│  │  TLR2/4/5 (surface)  +  CLRs (Dectin-1, DC-SIGN, etc.)  │    │
│  └─────────────────────────────────────────────────────────┘    │
├─────────────────────────────────────────────────────────────────┤
│  ENDOSESOME / LYSOSOME                                          │
│  ┌─────────────────────────────────────────────────────────┐    │
│  │  TLR3, TLR7, TLR8, TLR9                                 │    │
│  │  → "Internalized material is being processed"           │    │
│  └─────────────────────────────────────────────────────────┘    │
├─────────────────────────────────────────────────────────────────┤
│  CYTOSOL (inside the cell)                                      │
│  ┌─────────────────────────────────────────────────────────┐    │
│  │  NLRs (NOD1/2, NLRP3, NLRC4)                            │    │
│  │  RLRs (RIG-I, MDA5)                                     │    │
│  │  ALRs (AIM2)                                            │    │
│  │  cGAS (→ STING on ER)                                   │    │
│  │  → "Pathogen has breached the membrane"                 │    │
│  └─────────────────────────────────────────────────────────┘    │
└─────────────────────────────────────────────────────────────────┘
```

This **layered surveillance** means that a pathogen is detected at multiple
checkpoints as it progresses from outside → inside. No single PRR family is
sufficient for full detection; redundancy is the design principle.

## Detailed Family Profiles  

### 1. Toll-like Receptors (TLRs)

Covered in depth in [Toll-like Receptors](./Troll-LikeReceptor.md)

- 10 in humans, 12 in mice
- LRR ectodomain + TIR cytoplasmic domain
- MyD88-dependent (fast, surface) and TRIF-dependent (slow, endosomal) pathways
- The "first responders" of the PRR system

### 2. NOD-like Receptors (NLRs)

Covered in depth in [NOD-like Receptors](./NOD-LikeReceptor.md)

- Cytosolic; NACHT + LRR architecture
- NOD1/2 → RIP2 → NF-κB (bacterial peptidoglycan sensing)
- NLRP3, NLRC4, NLRP1 → **Inflammasome** → caspase-1 → IL-1β/IL-18 + pyroptosis
- The "confirmation" layer: if a pathogen has entered the 
  [cytosol](./Cytosol.md), NLRs escalate the response

### 3. RIG-I-like Receptors (RLRs)

The **cytosolic RNA sensors** — the antiviral counterpart to TLR3/7/8 (which
watch RNA in endosomes).

| Member            | Ligand                                        | Specificity                                                     |
|-------------------|-----------------------------------------------|-----------------------------------------------------------------|
| **RIG-I** (DDX58) | Short dsRNA; 5′-triphosphorylated RNA (viral) | Most RNA viruses; also some DNA viruses (via RNA intermediates) |
| **MDA5** (DDX45)  | Long dsRNA; viral replicative intermediates   | Picornaviruses (poliovirus, rhinovirus), enteroviruses          |
| **LGP2** (DDX46)  | Unknown (regulatory)                          | Modulates RIG-I/MDA5; may act as a decoy or process viral RNA   |

**Signaling pathway:**

```
Viral RNA → RIG-I or MDA5 (via CARD domains)
  → MAVS (mitochondrial antiviral-signaling protein; on outer mitochondrial membrane)
  → TRIF-like adaptor domains on MAVS
  → TRAF3/TRAF6 → TBK1 → IRF3/IRF7 → Type I IFNs (IFN-α/β)
  → TRAF6 → NF-κB → pro-inflammatory cytokines
```

**Key features:**

- **MAVS** is the critical adaptor — it sits on the **mitochondrial outer
  membrane**, creating a physical link between cytosolic RNA sensing and
  organelle-based signaling
- RIG-I is the dominant antiviral sensor in most cells; MDA5 is especially
  important in **interferon-stimulated** cells and against specific virus
  families
- **Genetic relevance:** RIG-I and MDA5 polymorphisms affect susceptibility to
  HCV, influenza, and SARS-CoV-2
- **Therapeutic relevance:** RIG-I/MDA5 agonists (short 5′-triphosphorylated
  (RNA) are explored as **vaccine adjuvants** and **cancer immunotherapies** 
  they induce a strong type I IFN response that upregulates MHC I on tumor
  cells)

### 4. C-type Lectin Receptors (CLRs)

The **carbohydrate sensors** — the PRR family that watches for microbial 
**glycans** (sugars) at the cell surface.

**Structure:** Each CLR contains one or more **C-type lectin domains (CTLDs)**, 
calcium-dependent carbohydrate-recognition domains. Unlike TLRs, CLRs typically
signal through **ITAM-bearing adaptor proteins** (SYK kinase pathway) rather
than TIR-domain adaptors.

| CLR                               | Ligand                                | Source                                       | Key Function                                                  |
|-----------------------------------|---------------------------------------|----------------------------------------------|---------------------------------------------------------------|
| **Dectin-1** (CLEC7A)             | β-1,3-glucan                          | Fungal cell walls (*Candida*, *Aspergillus*) | Phagocytosis; NF-κB; IL-1β; Th17 polarization                 |
| **Dectin-2** (CLEC6A)             | High-mannose glycans                  | Fungi, parasites                             | Synergizes with Dectin-1; NF-κB                               |
| **DC-SIGN** (CD209)               | High-mannose/fucosylated glycans      | HIV gp120, *Plasmodium*, fungi               | Viral uptake; phagocytosis; immunosuppressive (on some cells) |
| **Mincle** (CLEC4E)               | α-mannans, trehalose dimycolate (TDM) | Fungi, *M. tuberculosis*                     | NF-κB; IL-1β; Th1/Th17                                        |
| **MGL** (CLEC10A)                 | Mannose, fucose                       | Fungi, mycobacteria                          | Phagocytosis                                                  |
| **MR / CD206** (Mannose receptor) | Mannose, fucose, galactose            | Fungi, apoptotic cells, glycosaminoglycans   | Phagocytosis; clearance                                       |
| **DCIR** (CLEC4A)                 | Unknown (fungal?)                     | —                                            | Inhibitory (ITIM); negative regulation                        |
| **CLEC2** (CLEC1B)                | Thrombospondin (self)                 | Host                                         | Platelet aggregation; immune modulation                       |

**Signaling (Dectin-1 example):**

```
β-glucan → Dectin-1 (FasII domain binds ligand; CTLD mediates dimerization)
  → FcRγ (ITAM-bearing co-receptor)
  → SYK → CARD9 → BCL10 → MALT1 → NF-κB
  → Cytokines: IL-6, TNF-α, IL-23, CCL2
  → Also: phagocytosis, ROS production, IL-1β (via NLRP3 cross-talk)
```

**Key features:**

- CLRs are the **primary fungal sensors** — fungi are invisible to TLRs (which
  sense lipids and nucleic acids), so CLRs fill a critical gap
- **Dectin-1** is the best-characterized CLR; it signals through **FcRγ** (the
  same ITAM-bearing chain used by Fc receptors for antibodies) — a remarkable
  example of pathway sharing
- **Mincle** is a key sensor for *M. tuberculosis* (via TDM) and is a
  therapeutic target for TB
- **DC-SIGN** is a double-edged sword: it promotes phagocytosis but also
  facilitates **HIV entry** (by binding gp120 and concentrating virus on the
  cell surface)

### 5. AIM2-like Receptors (ALRs)

The **cytosolic DNA sensors** that form **inflammasomes**.

| Member                          | Ligand                                                | Output                                                                           |
|---------------------------------|-------------------------------------------------------|----------------------------------------------------------------------------------|
| **AIM2** (Absent In Melanoma 2) | Cytosolic **dsDNA** (bacterial, viral, mitochondrial) | **Inflammasome** → caspase-1 → IL-1β, IL-18, pyroptosis                          |
| **IFI16**                       | Cytosolic dsDNA (also monomeric DNA)                  | Type I IFN (via STING-independent pathway); also inflammasome (in some contexts) |
| **SAMD9/SAMD9L**                | Unknown                                               | GSDMD-mediated cell death (in plants: antiviral)                                 |

**AIM2 structure:** PYD (N-terminal) + HIN domain (C-terminal; binds DNA
directly, no adaptor needed)

**Signaling:**

```
Cytosolic dsDNA → AIM2 (HIN domain binds DNA directly)
  → PYD-mediated oligomerization
  → ASC recruitment (PYD-PYD interaction)
  → Pro-caspase-1 recruitment → auto-cleavage
  → Active caspase-1 → cleaves pro-IL-1β, pro-IL-18, gasdermin D
  → IL-1β/IL-18 secretion + pyroptosis
```

**Key features:**

- AIM2 is the **dominant cytosolic DNA sensor for inflammasome activation** —
  distinct from cGAS-STING (which drives type I IFN)
- Both AIM2 and cGAS detect the same ligand (cytosolic dsDNA) but produce *
  *different outputs** (IL-1β/pyroptosis vs. type I IFN) — a division of labor
- **Genetic relevance:** AIM2 mutations → susceptibility to *Listeria*,
  *Salmonella*, and other DNA-containing pathogens
- **Therapeutic relevance:** AIM2 agonists (CpG-free dsDNA) explored for cancer
  immunotherapy

### 6. cGAS-STING (the DNA→IFN axis)

Strictly speaking, **cGAS** (cyclic GMP-AMP synthase) is the sensor and **STING
** (Stimulator of Interferon Genes) is the adaptor — but they function as a
single pathway and are often grouped with PRRs.

```
Cytosolic dsDNA → cGAS (binds DNA via Walker A/B motifs)
  → Synthesizes cGAMP (2′3′-cGAMP) from ATP + GTP
  → cGAMP (second messenger) → STING (on ER membrane)
  → STING oligomerizes → translocates ER → Golgi
  → Recruits TBK1 → IRF3 → Type I IFNs (IFN-β)
  → Also: NF-κB → pro-inflammatory cytokines
  → Also: MAVS cross-talk → type I IFN amplification
```

**Key features:**

- cGAS is the **dominant cytosolic DNA sensor for type I IFN production** (
  complementary to AIM2's inflammasome role)
- **STING** is one of the most actively targeted PRRs in **cancer immunotherapy
  ** — STING agonists (cGAMP analogs, diabenzazepine compounds) are in multiple
  Phase I/II trials
- **Genetic relevance:** cGAS mutations → susceptibility to viral infections;
  STING mutations → immunodeficiency
- **DAMP sensing:** Mitochondrial DNA released during cell stress activates
  cGAS-STING → sterile inflammation (relevant in atherosclerosis,
  neurodegeneration, cancer)

## The Two Major Signaling Outputs

All PRRs converge on two (sometimes three) transcriptional programs:

| Output                                       | Key Transcription Factors    | Cytokines                                              | Function                                                                  |
|----------------------------------------------|------------------------------|--------------------------------------------------------|---------------------------------------------------------------------------|
| **Inflammatory**                             | NF-κB (p65/p50), AP-1, C/EBP | TNF-α, IL-6, IL-1β (proform), IL-23, IL-12, chemokines | Acute inflammation; neutrophil/macrophage recruitment; fever              |
| **Antiviral (Type I IFN)**                   | IRF3, IRF7, IRF9 (ISGF3)     | IFN-α, IFN-β                                           | Antiviral state (upregulates MHC I, PKR, OAS, Mx proteins); DC maturation |
| **Inflammasome** (NLRP3, NLRC4, AIM2, NLRP1) | Caspase-1 (not a TF)         | IL-1β, IL-18 (active, secreted)                        | Pyroptosis; potent inflammation; Th17 polarization                        |

**Critical distinction:** The inflammatory program (NF-κB) and the antiviral
program (IRF3/7) are **independently regulated** — a cell can produce one
without the other. This is why:

- TLR4 (LPS) → primarily NF-κB (inflammatory), minimal IFN
- TLR3 (dsRNA) → primarily IRF3 (antiviral), minimal NF-κB
- RIG-I (viral RNA) → both NF-κB and IRF3
- NLRP3 (K⁺ efflux) → inflammasome only (no new transcription; requires prior "
  priming" by TLR/NF-κB to load pro-IL-1β)

## The "Priming" Requirement

A critical concept that links PRR families: **inflammasome-activating PRRs (
NLRP3, NLRC4, AIM2) cannot act alone.** They require a prior **"priming" signal
** from a transcriptional PRR (TLR, NOD, CLR, cGAS) to load the cell with
inactive pro-IL-1β and pro-IL-18:

```
Signal 1 (Priming):  TLR4/LPS → NF-κB → transcription of pro-IL-1β, pro-IL-18, NLRP3
Signal 2 (Activation): NLRP3 sensor (K⁺ efflux, ROS, ATP) → inflammasome → caspase-1
  → Cleaves pro-IL-1β → active IL-1β → secretion
```

Without priming, NLRP3 activation produces no IL-1β (there's no substrate).
Without activation, priming produces only the pro-form (inactive). **Both
signals are required.**

## How PRRs Are Connect

| Topic                     | PRR Connection                                                                                                                                                                                                 |
|---------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Microbiome**            | Commensal PAMPs (peptidoglycan → NOD1/2; LPS → TLR4; β-glucan → Dectin-1) provide tonic low-grade signaling that maintains immune tone. Dysbiosis → altered PRR stimulation → inflammation or immunodeficiency |
| **T cells**               | PRR activation on DCs → co-stimulatory molecules (CD80/86) + cytokines (IL-12, IL-6, IL-23) → T cell polarization (Th1, Th17, Treg). PRRs are the "bridge" from innate to adaptive                             |
| **B cells**               | TLR7/9 on B cells provide co-stimulatory signals for activation and class switching. TLR9 agonists (CpG ODN) are vaccine adjuvants                                                                             |
| **Autoimmunity**          | Loss of tolerance + PRR sensing of DAMPs (self DNA → cGAS-STING, TLR9; self RNA → TLR7, RIG-I) → chronic inflammation. SLE: anti-dsDNA immune complexes → TLR7/9 in endosomes → IFN signature                  |
| **Cancer**                | Tumors suppress PRR signaling (downregulate STING, cGAS, TLRs) to evade detection. STING agonists + checkpoint inhibitors = current hot area in cancer immunotherapy                                           |
| **Allergy**               | PRR activation on DCs in a Th2-polarizing environment → IgE class switching → mast cell sensitization                                                                                                          |
| **Inflammation / Sepsis** | Excessive PRR activation (TLR4/LPS in sepsis) → cytokine storm → organ failure. PRR inhibitors (anti-TLR4, JAK inhibitors) are therapeutic targets                                                             |
| **Neuroinflammation**     | Microglial PRRs (TLR3/4/9, NLRP3, RIG-I) sense viral RNA, amyloid-β, α-synuclein → neuroinflammation in Alzheimer's, Parkinson's, MS                                                                           |

## Inhibitory PRRs (iPRRs)

Not all PRRs activate. Some **suppress** immune responses to prevent
overactivation.

| iPRR              | Mechanism                                                           |
|-------------------|---------------------------------------------------------------------|
| **SIGIR / CD163** | Scavenges hemoglobin; suppresses TLR4                               |
| **FcγRIIB**       | ITIM-bearing; inhibits B cell and myeloid activation                |
| **DCIR** (CLEC4A) | ITIM-bearing CLR; negative regulation of DC responses               |
| **LAIR-1**        | Inhibitory receptor; suppresses TLR and BCR signaling               |
| **TIGIT**         | Inhibitory receptor on T cells/NK cells; counterbalances activation |

These "brakes" are essential. Without them, PRR activation would be
self-amplifying and fatal. Their dysregulation contributes to both
immunodeficiency (excessive inhibition) and autoimmunity (inadequate
inhibition).
