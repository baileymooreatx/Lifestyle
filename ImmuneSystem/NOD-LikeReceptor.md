<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
**Table of Contents**  *generated with [DocToc](https://github.com/thlorenz/doctoc)*

- [NOD-Like Receptors (NLRs)](#nod-like-receptors-nlrs)
  - [Structure](#structure)
  - [Subfamilies & Key Members](#subfamilies--key-members)
  - [Two Major Signaling Outputs](#two-major-signaling-outputs)
  - [Why It Matters Clinically](#why-it-matters-clinically)
  - [Connection to the Microbiome](#connection-to-the-microbiome)

<!-- END doctoc generated TOC please keep comment here to allow auto update -->

# NOD-Like Receptors (NLRs)

**NLRs** are a family of **[cytosolic](./Cytosol.md) pattern recognition 
receptors** that detect microbial products, pathogen-associated molecular 
Patterns (PAMPs), and host danger signals, damage-associated molecular 
patterns (DAMPs), **inside** the cell, complementing the membrane-bound 
[Toll-like receptors (TLRs)](./Troll-LikeReceptor.md). They are sometimes called 
**NACHT** (Nucleotide-binding domain, domain with **A**mino-acid repeats, 
**C**ysteine-**H**is-**T**hreonine) and **LRR** (Leucine-Rich Repeat) proteins.  

**NOD** stands for "Nucleotide-binding and Oligomerization Domain." It refers to 
the central domain of NLR proteins that binds ATP/GTP and drives ATP-dependent 
**self-oligomerization** — the molecular "switch" that toggles the receptor from 
an inactive monomer to an active oligomer capable of recruiting downstream 
signaling partners (e.g., ASC for inflammasome assembly, or RIP2 for NF-κB 
activation).

The broader structural name for this domain is **NACHT** (NAIP, CIITA, HET-E, 
TP1 — the four founding proteins in which this nucleotide-binding/oligomerization 
motif was first identified). So "NOD domain" and "NACHT domain" are used 
interchangeably.

## Structure

All NLRs share a common three-part architecture:

- **N-terminal effector domain**: determines the signaling output (CARD, PYD,
  BIR, or none)
- **Central NACHT domain**: the nucleotide-binding switch that toggles
  activation
- **C-terminal leucine-rich repeats (LRRs)**: the ligand-sensing region

## Subfamilies & Key Members

| Subfamily               | Key Members               | Primary Function                                           |
|-------------------------|---------------------------|------------------------------------------------------------|
| **NLRP** (Pyrin domain) | **NLRP3**, NLRP1, NLRP12  | Inflammasome formation → caspase-1 activation              |
| **NLRC** (CARD)         | **NOD1**, **NOD2**, NLRC4 | NF-κB/MAPK signaling; NLRC4 also forms inflammasomes       |
| **NLRA**                | CIITA (NLRA1)             | MHC class II gene regulation                               |
| **NLRB**                | NAIP                      | Senses bacterial type-III secretion; partners with NLRC4   |
| **NLRX**                | NLRX1                     | Antiviral; mitochondrial localization; inhibits type I IFN |

## Two Major Signaling Outputs

**1. NF-κB / MAPK pathway** (NOD1, NOD2, NLRC4)

- NOD1 detects **Tri-DAP** (from Gram-negative peptidoglycan); NOD2 detects
  **MDP** (from Gram-positive peptidoglycan)
- Their CARD domains recruit **RIP2** → activates NF-κB and MAPKs →
  transcription of pro-inflammatory cytokines (IL-6, TNF-α, IL-1β *proform*) and
  antimicrobial peptides
- This is the **"priming" signal** — it loads the cell with inactive pro-IL-1β
  and pro-IL-18

**2. Inflammasome assembly** (NLRP3, NLRP1, NLRC4, AIM2)

- The PYD (or CARD) domain of the activated NLR recruits the adaptor **ASC**
  (PYCARD), which in turn recruits **pro-caspase-1**
- Oligomerization of pro-caspase-1 causes its **auto-cleavage into active
  caspase-1**
- Active caspase-1 cleaves pro-IL-1β and pro-IL-18 into their **active, secreted
  forms**
- Caspase-1 also cleaves **gasdermin D** → pore formation → **pyroptosis**
  (lytic, inflammatory cell death)
- This is the **"activation" signal** — it requires a second trigger (K⁺ efflux,
  ROS, ATP, lysosomal damage, etc.)

## Why It Matters Clinically

- **NOD2** mutations → **Crohn's disease**, Blau syndrome
- **NLRP3** mutations → **CAPS** spectrum (Familial Cold Autoinflammatory
  Syndrome, Muckle-Wells, NOMID/CINCA)
- **NLRP1** mutations → autoinflammatory skin disorders
- **NLRC4** mutations → autoinflammatory enterocolitis
- **NLRP3** is a major therapeutic target for **gout**, **atherosclerosis**,
  **obesity-related inflammation**, and **neurodegeneration** (Alzheimer's,
  Parkinson's)

## Connection to the Microbiome

NOD1 and NOD2 are expressed heavily in **intestinal epithelial cells** and
directly sense bacterial peptidoglycan from the [gut lumen](./GutLumen.md), 
making them a key molecular bridge between the microbiome and host immunity. A 
healthy microbiome provides a steady "low-grade" peptidoglycan signal that keeps 
NOD1/2 tone appropriate; dysbiosis (antibiotics, pathogenic overgrowth) disrupts 
this and can drive chronic intestinal inflammation.
