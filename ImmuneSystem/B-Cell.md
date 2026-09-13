<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
**Table of Contents**  *generated with [DocToc](https://github.com/thlorenz/doctoc)*

- [B Cells](#b-cells)
  - [Development in the Bone Marrow](#development-in-the-bone-marrow)
  - [The B Cell Receptor (BCR)](#the-b-cell-receptor-bcr)
  - [Activation: T-Dependent vs. T-Independent](#activation-t-dependent-vs-t-independent)
  - [The Germinal Center (GC) Reaction](#the-germinal-center-gc-reaction)
  - [B Cell Subsets](#b-cell-subsets)
  - [Memory B Cells & Plasma Cells](#memory-b-cells--plasma-cells)
  - [How B Cells Connect to Prior Topics](#how-b-cells-connect-to-prior-topics)
  - [Clinical Relevance at a Glance](#clinical-relevance-at-a-glance)
  - [Key Takeaway](#key-takeaway)

<!-- END doctoc generated TOC please keep comment here to allow auto update -->

## B Cells

**B cells** (B lymphocytes) are the antibody-producing arm of adaptive immunity.
They originate and mature in the **bone marrow** — hence the "B" (initially
attributed to the bursa of Fabricius in birds, but in mammals the bone marrow is
the equivalent site). Unlike T cells, B cells can recognize **free, unprocessed
antigens** directly via their surface immunoglobulin (the BCR), making them the
only lymphocytes capable of sensing soluble pathogens without help from another
cell.

### Development in the Bone Marrow

B cell maturation is a stepwise process driven by successful receptor gene
rearrangement:

| Stage              | Key Event                                                                              | Surface Marker                      |
|--------------------|----------------------------------------------------------------------------------------|-------------------------------------|
| **Pro-B**          | Heavy chain V-D-J recombination (RAG1/2)                                               | CD19⁺, CD79a/b⁺                     |
| **Pre-B**          | Light chain V-J recombination; pre-BCR signaling (survival + proliferation checkpoint) | pre-BCR (μ + surrogate light chain) |
| **Immature B**     | Full surface IgM expression; **negative selection** begins                             | IgM only                            |
| **Transitional**   | Exit bone marrow → spleen; final tolerance checks                                      | IgM⁺, IgD⁻                          |
| **Mature naïve B** | Co-expression of IgM and IgD on same cell                                              | **IgM⁺ IgD⁺**                       |

**Key checkpoints:**

- **Allelic exclusion:** Once a functional heavy chain is produced, the other
  allele is silenced — ensuring each B cell expresses a single specificity
- **Negative selection:** Immature B cells that bind self-antigen strongly in
  the marrow undergo **receptor editing** (light chain rearrangement on the
  other allele), **clonal deletion** (apoptosis), or **anergy**
- Failure of this process → **autoantibody production** (allergies, lupus)

---

### The B Cell Receptor (BCR)

| Component                                                | Role                                                                                                |
|----------------------------------------------------------|-----------------------------------------------------------------------------------------------------|
| **Membrane immunoglobulin** (mIgM + mIgD on naïve cells) | Antigen recognition; can bind native, unprocessed epitopes (conformational, linear, polysaccharide) |
| **CD79a/CD79b** (Igα/Igβ)                                | Signal transduction; contains **ITAMs** in cytoplasmic tails                                        |

**Critical distinction from TCR:** The BCR binds **free antigen** directly. The
TCR requires peptide presented on MHC. This is why B cells can respond to *
*T-independent antigens** (bacterial polysaccharides, LPS) that T cells cannot
see.

---

### Activation: T-Dependent vs. T-Independent

**T-Dependent (TD) Activation** — the dominant pathway for protein antigens:

```
1. B cell binds native antigen via BCR → internalization → processing → peptide loading onto MHC II
2. B cell presents peptide to cognate Tfh cell (in T-B border zone)
3. Tfh provides:
   - CD40L → CD40 on B cell (Signal 2)
   - Cytokines: IL-4 (→ IgE), IL-21 (→ GC entry, plasma cell differentiation)
4. B cell enters germinal center → class switching + affinity maturation
5. Output: memory B cells + long-lived plasma cells
```

**T-Independent (TI) Activation** — for repetitive, non-protein antigens:

| Type     | Ligand                                                            | Mechanism                                           | Output                               |
|----------|-------------------------------------------------------------------|-----------------------------------------------------|--------------------------------------|
| **TI-1** | LPS (TLR4 ligand)                                                 | BCR crosslinking + TLR4 co-stimulation (polyclonal) | IgM, little memory                   |
| **TI-2** | Bacterial capsular polysaccharides, pneumococcal C-polysaccharide | Extensive BCR crosslinking alone (no TLR needed)    | IgM, poor memory, no class switching |

This is why **children <2 years** (whose germinal centers are immature) are
vulnerable to encapsulated bacteria (*S. pneumoniae*, *H. influenzae*) — they
cannot mount a proper TD response to polysaccharide antigens.

---

### The Germinal Center (GC) Reaction

The GC is the "upgrade shop" of B cell biology — a specialized microanatomical
structure within lymph node follicles where activated B cells undergo:

**1. Somatic Hypermutation (SHM)**

- Enzyme: **AID** (Activation-Induced Cytidine Deaminase)
- Introduces point mutations at ~10⁻³ per base pair per division in V-region Ig
  genes
- Occurs in the **dark zone** (centroblasts, rapid proliferation)
- Most mutations are neutral or deleterious; a few increase affinity

**2. Affinity Maturation (Selection)**

- Occurs in the **light zone** (centrocytes)
- B cells compete for limited antigen displayed on **follicular dendritic
  cells (FDCs)**
- High-affinity BCRs outcompete pre-existing antibody for antigen binding →
  internalization → presentation to **Tfh cells** → survival signal (CD40L,
  IL-21)
- Low-affinity B cells that fail to bind antigen → **apoptosis**
- Each cycle: dark zone (mutate) → light zone (select) → dark zone (mutate
  again)
- Result: iterative Darwinian selection at the cellular level

**3. Class-Switch Recombination (CSR)**

- Also mediated by **AID**
- Deletes DNA between switch (S) regions upstream of constant region genes
- Irreversible; changes effector function without altering antigen specificity
- Cytokine-directed: IL-4 → IgE; TGF-β → IgA; IFN-γ → IgG (subclass)

| Immunoglobulin Isotype          | Key Effector Function                                                                |
|---------------------------------|--------------------------------------------------------------------------------------|
| **IgM**                         | First responder; potent complement activation (C1q binding); pentamer = high avidity |
| **IgG**                         | Opsonization, ADCC, transplacental transfer (IgG1/3); 4 subclasses in humans         |
| **[IgA](./ImmunoglobulinA.md)** | Mucosal immunity (dimeric, secretory component); coats commensals (sIgA)             |
| **IgE**                         | Mast cell/basophil degranulation; anti-helminth; **allergy/anaphylaxis**             |
| **IgD**                         | BCR co-receptor on naïve B cells; role in activation still debated                   |

**GC Output:**

- **Long-lived plasma cells** → migrate to **bone marrow** → secrete antibody
  for months to decades
- **Memory B cells** → circulate in quiescent state → rapid secondary response
  upon re-exposure

---

### B Cell Subsets

| Subset                             | Location                                  | Key Feature                                                                                                                                    |
|------------------------------------|-------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------|
| **B2 (conventional)**              | Spleen, lymph nodes, bone marrow          | Standard adaptive B cells; T-dependent; GC reaction                                                                                            |
| **B1**                             | Peritoneal cavity, pleural cavity, mucosa | Innate-like; self-renewing; produce natural IgM (polyreactive, low affinity); respond to TI antigens; first line against encapsulated bacteria |
| **Marginal zone (MZ) B cells**     | Splenic marginal zone                     | Rapid response to blood-borne T-independent antigens (e.g., *Neisseria*, *Haemophilus*); complement-dependent                                  |
| **Follicular B cells**             | Lymph node follicles                      | T-dependent; GC entry; high-diversity antibodies                                                                                               |
| **Tissue-resident memory B cells** | Mucosal tissues (gut, lung, skin)         | Localized rapid response; produce IgA/IgG at barrier surfaces                                                                                  |

---

### Memory B Cells & Plasma Cells

| Feature                 | Memory B Cells                                     | Long-Lived Plasma Cells                         |
|-------------------------|----------------------------------------------------|-------------------------------------------------|
| **Function**            | Standby; rapid clonal expansion on re-exposure     | Continuous antibody secretion                   |
| **Surface Ig**          | Yes (mIgG, mIgA, mIgE)                             | Minimal/absent (all Ig secreted)                |
| **Lifespan**            | Years to decades                                   | Months to >10 years (bone marrow niches)        |
| **Key markers (human)** | CD27⁺, FCRL4⁺                                      | CD138⁺, BCMA⁺, CXCR4⁺, XBP1⁺                    |
| **Location**            | Blood, lymph nodes, bone marrow                    | Bone marrow (niche: APRIL, BAFF, stromal cells) |
| **Response speed**      | Hours to days (re-enter GC or differentiate to PC) | Immediate (already secreting)                   |

The **secondary response** is faster, stronger, and higher-affinity than the
primary because:

- Memory B cells have higher BCR affinity (SHM-selected)
- Lower activation threshold (less co-stimulation needed)
- Already class-switched (no need to wait for GC)
- Larger precursor pool (clonal expansion already occurred)

---

### How B Cells Connect to Prior Topics

| Connection                        | Mechanism                                                                                                                                                                                                                                                   |
|-----------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **TLRs → B cells**                | TLR7/8 (ssRNA), TLR9 (CpG DNA) on B cells provide co-stimulatory signals that enhance activation, class switching, and antibody production. TLR9 is a key **adjuvant target** in vaccines                                                                   |
| **Microbiome → B cells**          | Commensal antigens drive **sIgA** production in Peyer's patches → coats bacteria, prevents translocation. Dysbiosis → altered IgA repertoire → mucosal inflammation. Bifidobacterium and *Bacteroides* specifically promote IgA class switching             |
| **Allergy (Linda)**               | Th2 cytokines (IL-4, IL-13) drive B cells to **class-switch to IgE** → IgE coats mast cells → degranulation on re-exposure → anaphylaxis. The "hygiene hypothesis" predicts reduced microbial exposure → less Treg tone → Th2 skewing → IgE overproduction  |
| **Autoimmunity (Merredith, Bob)** | Failure of B cell negative selection + loss of Treg suppression → **autoreactive B cells** escape → produce autoantibodies (anti-CCP in RA, anti-dsDNA in SLE). B cells also act as APCs presenting autoantigens to T cells, amplifying the autoimmune loop |
| **Cancer (Jason)**                | Tumor microenvironment suppresses B cell function; however, **CAR-T** and **bispecific antibodies** are now being adapted for B cell targeting. B cell-derived antibodies (e.g., **rituximab** anti-CD20) are used in B cell lymphomas                      |
| **Vaccines**                      | mRNA vaccines (SARS-CoV-2) induce persistent GC reactions → affinity-matured plasma cells in bone marrow + memory B cells → durable, high-avidity antibody protection. This is the "Infinity Machine" (Chapter 12) in action                                |

---

### Clinical Relevance at a Glance

| Condition                                   | B Cell Pathology                                                                     |
|---------------------------------------------|--------------------------------------------------------------------------------------|
| **Agammaglobulinemia (XLA)**                | BTK mutation → no mature B cells → no antibody → recurrent infections from age 6 mo  |
| **Common Variable Immunodeficiency (CVID)** | Defective B cell differentiation → low all isotypes                                  |
| **Hyper-IgM syndrome**                      | CD40L (T cell) or CD40 (B cell) defect → no class switching → only IgM               |
| **SLE**                                     | Autoreactive B cells → anti-dsDNA, anti-Sm antibodies; immune complex deposition     |
| **Rheumatoid arthritis**                    | Anti-CCP IgG autoantibodies; B cells in synovium                                     |
| **Multiple myeloma**                        | Malignant plasma cell proliferation → monoclonal protein (M spike)                   |
| **Waldenström's macroglobulinemia**         | Malignant B cell → excess IgM                                                        |
| **Gut-associated lymphoma (MALT)**          | Chronic antigen stimulation (e.g., *H. pylori*) → B cell lymphoma                    |
| **Rituximab therapy**                       | Anti-CD20 monoclonal antibody → depletes B cells → used in RA, SLE, B cell lymphomas |

---

### Key Takeaway

B cells are the **antibody factory** of adaptive immunity. They uniquely bridge
innate and adaptive worlds (via TLR co-stimulation and TI responses), generate
near-infinite antibody diversity through V(D)J recombination + SHM, and provide
the only form of **long-lasting, circulating, pre-formed protection** (antibody)
in the body. The entire logic of vaccination — and the "elegant defense" that
gives the book its title — depends on the B cell's ability to remember, refine,
and secrete. When that system misfires (autoantibodies, IgE overproduction), it
becomes the source of the very diseases the book's characters battle.
