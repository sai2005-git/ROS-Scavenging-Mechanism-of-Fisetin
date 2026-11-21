# Computational Investigation of Fisetin

## Overview

This project investigates the structural, electronic, and optical properties of **Fisetin (3,3′,4′,7-tetrahydroxyflavone)** using Density Functional Theory (DFT) and Time-Dependent Density Functional Theory (TD-DFT). The study also describes a molecular docking approach to explore the binding potential of fisetin toward **Glycogen Synthase Kinase-3 beta (GSK3β)**, a key protein associated with the Reperfusion Injury Salvage Kinase (RISK) pathway.

The work aims to understand the electronic properties of fisetin and its potential relevance to cardioprotective research, particularly in the context of myocardial ischemia–reperfusion injury.

## Objectives

- Optimize the molecular geometry of fisetin.
- Investigate frontier molecular orbitals (HOMO and LUMO).
- Evaluate molecular electrostatic potential (MEP) and atomic charge distributions.
- Examine intramolecular charge transfer and donor–acceptor interactions through NBO analysis.
- Study solvent-dependent electronic absorption using TD-DFT.
- Explore fisetin's potential binding interactions with GSK3β through molecular docking.

## Computational Methodology

### 1. Geometry Optimization

- **Method:** Density Functional Theory (DFT)
- **Functional:** B3LYP
- **Basis set:** cc-pVDZ
- **Software:** Gaussian 09
- Frequency calculations were used to verify the optimized structure as a local minimum on the potential energy surface.

### 2. Electronic Structure and Reactivity Analysis

The optimized structure was used for:

- HOMO–LUMO analysis
- Global reactivity descriptors
- Molecular Electrostatic Potential (MEP) mapping
- Mulliken population analysis
- Natural Population Analysis (NPA)
- Natural Bond Orbital (NBO) analysis
- Fukui function analysis (listed in the study)

### 3. Solvent-Dependent UV–Visible Analysis

TD-DFT calculations were performed using the Polarizable Continuum Model (PCM) to investigate the absorption properties of fisetin in:

- Gas phase
- Water
- Ethanol
- Dimethyl sulfoxide (DMSO)
- Chloroform
- Acetonitrile

### 4. Molecular Docking

The study describes docking fisetin against **GSK3β** to investigate its potential binding mode.

- **Protein source:** Protein Data Bank (PDB)
- **Docking software:** AutoDock 4.2
- **Search algorithm:** Lamarckian Genetic Algorithm (LGA)
- **Interaction visualization:** Discovery Studio Visualizer

The docking workflow involves protein and ligand preparation, docking, and analysis of protein–ligand interactions.

## Software and Tools

| Software / Tool | Application |
|---|---|
| Gaussian 09 | DFT geometry optimization and electronic structure calculations |
| GaussView 6.0 | Molecular visualization and orbital/MEP representation |
| AutoDock 4.2 | Molecular docking |
| Discovery Studio Visualizer | Visualization and analysis of protein–ligand interactions |

## Key Findings

### Frontier Molecular Orbitals

- HOMO energy: **−5.962 eV**
- LUMO energy: **−1.967 eV**
- HOMO–LUMO energy gap: **3.995 eV**

The orbital distributions indicate electron donation from hydroxyl-substituted aromatic regions toward the chromone and carbonyl-containing region.

### UV–Visible Absorption

The calculated absorption maxima show a small red shift in solvent environments compared with the gas phase.

| Medium | Absorption maximum (nm) |
|---|---:|
| Gas phase | 364.85 |
| Water | 373.09 |
| Ethanol | 373.47 |
| DMSO | 374.50 |
| Chloroform | 374.35 |
| Acetonitrile | 373.22 |

The dominant electronic transition was assigned primarily to HOMO → LUMO excitation, with contributions of approximately 97% in the gas phase and 98% in solvent environments.

### Molecular Electrostatic Potential and Charge Analysis

The MEP and population analyses indicate that the oxygen-containing functional groups are major electron-rich regions of fisetin. The hydroxyl hydrogen atoms show positive charge character, supporting their potential involvement in hydrogen-bonding interactions.

### Natural Bond Orbital Analysis

NBO calculations indicate substantial donor–acceptor interactions and electron delocalization across the conjugated flavonoid framework. The strongest stabilization interactions reported include:

- LP(O17) → π*(C2–C3): **32.35 kcal/mol**
- LP(O21) → π*(C7–C8): **32.31 kcal/mol**

These interactions highlight the contribution of oxygen lone-pair donation to molecular stabilization.

## Repository Contents

A suggested repository organization is:

```text
Fisetin-Computational-Investigation/
│
├── README.md
├── Fisetin_Script.docx
│
├── Gaussian_Inputs/
│   └── (Gaussian input files)
│
├── Gaussian_Outputs/
│   └── (Gaussian output files)
│
├── Molecular_Visualizations/
│   ├── Optimized_Structure/
│   ├── HOMO_LUMO/
│   └── MEP/
│
├── UV_Visible_Spectra/
│
└── Docking/
    ├── Protein/
    ├── Ligand/
    └── Results/
```

*The folder structure above is a suggested organization. Add only the files and results that are actually available in the repository.*

## Research Significance

The computational results provide molecular-level insight into fisetin's geometry, electronic structure, charge distribution, and solvent-dependent optical behavior. The docking component is intended to explore its interactions with GSK3β in the context of the RISK signaling pathway.

These computational findings provide a basis for further investigation. They do not, by themselves, establish biological efficacy or clinical cardioprotective activity.

## References

- Fisetin (3,3′,4′,7-tetrahydroxyflavone).
- Protein Data Bank (PDB): https://www.rcsb.org/
- Gaussian: https://gaussian.com/
- AutoDock: https://autodock.scripps.edu/

---

**Note:** This README summarizes the computational methods and findings described in the project document. Include the corresponding input files, output files, docking results, and figures in the repository when available.
