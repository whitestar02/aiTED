# aiTED: AI-driven Transition-state Enzyme Design

## Overview

**aiTED** is a computational enzyme design framework grounded in the **transition-state (TS) stabilization theory**: enzymes accelerate chemical reactions by forming favorable noncovalent interactions that selectively bind and stabilize high-energy TS species, thereby lowering the overall activation energy barrier.

Inspired by the **conserved oxyanion hole** in proteinases and esterases — which stabilizes negatively charged tetrahedral intermediates via backbone amide hydrogen bonds during peptide and ester hydrolysis — aiTED introduces potential H-bond donors into the oxyanion hole region through rational active-site mutagenesis, lowering the activation energy of rate-limiting transition states.

## General Protocol

1. **TS-complex modeling** — AlphaFold3 is employed to construct TS-like complex models of the wild-type enzyme and each mutant with the substrate.
2. **Rational mutagenesis & validation** — Active-site residues are rationally mutated to introduce potential hydrogen-bond donors into the oxyanion hole region; mutant conformations are validated using AlphaFold3.
3. **nHB comparison** — The difference in the number of hydrogen bonds (nHB) within the oxyanion hole is compared between the wild-type enzyme and each mutant.
4. **Experimental validation** — The reaction rates of the wild-type and each mutant are determined experimentally.
5. **Accuracy evaluation** — The predictive accuracy of aiTED is evaluated by comparing experimentally measured activities with the theoretically predicted changes in nHB.

## Key Features

- 🔬 **TS-centric design** — Explicitly targets transition-state stabilization via oxyanion hole engineering
- 🤖 **AlphaFold3-powered** — Automated TS-complex modeling and mutant conformation validation
- 📊 **nHB-based prediction** — Quantifies H-bond network changes as a proxy for catalytic enhancement
- ⚡ **Experimentally validated** — Predictions benchmarked against measured reaction rates

