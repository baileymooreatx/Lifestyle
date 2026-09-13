<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
**Table of Contents**  *generated with [DocToc](https://github.com/thlorenz/doctoc)*

- [Cytosol](#cytosol)
    - [What's in the Cytosol](#whats-in-the-cytosol)
    - [What's *not* Cytosolic](#whats-not-cytosolic)
    - [Why it matters in our discussion](#why-it-matters-in-our-discussion)

<!-- END doctoc generated TOC please keep comment here to allow auto update -->

# Cytosol

The cytosol is the fluid-filled interior of a cell that lies *between* the
plasma membrane and the nucleus, and *around* (but excluding) the organelles. 
**Cytosolic** means **located in the cytosol**.

### What's in the Cytosol

| Component                              | Example                                                                       |
|----------------------------------------|-------------------------------------------------------------------------------|
| **Cytosol** (the aqueous fluid itself) | Water, ions, metabolites, dissolved proteins                                  |
| **Cytoskeleton**                       | Actin filaments, microtubules, intermediate filaments                         |
| **Free ribosomes**                     | Protein synthesis                                                             |
| **Cytosolic proteins**                 | Enzymes, signaling molecules, transcription factors (when not in the nucleus) |

### What's *not* Cytosolic

- **Nucleoplasm** (inside the nuclear envelope)
- **Organelle lumens** (mitochondrial matrix, ER lumen, lysosome interior, etc.)
- **Plasma membrane** (it's a membrane, not a compartment)
- **Extracellular space** (outside the cell)

### Why it matters in our discussion

When we described **NLRs, RLRs (RIG-I, MDA5), AIM2, and cGAS** as "cytosolic
sensors," we meant they sit *in the fluid interior of the cell* and detect
pathogens that have **breached the plasma membrane** — as opposed to TLRs and
CLRs, which watch the cell surface or endosomes. The spatial logic is:

```
Outside cell  →  Surface TLRs / CLRs
Inside membrane (endosome)  →  TLR3/7/8/9
Inside cell (cytosol)  →  NLRs, RLRs, AIM2, cGAS   ← "cytosolic"
```

So "cytosolic" is simply the compartment label: it tells you *where* in the cell
the sensor is stationed, which determines *what stage* of pathogen invasion it
can detect.
