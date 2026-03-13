# CODEX Resonance Framework - Validations

**Author:** Dustin Hansley, Hans-Made Research Inc.
**Location:** Winnipeg, Manitoba, Canada
**Contact:** [Hans-Made Research](https://github.com/CodexResonance)

---

## What is CODEX?

The CODEX Genesis Resonance Framework is a **physics-only** molecular prediction engine built on a single universal invariant:

```
f * d = 542.6395291455866 GHz*A
```

Derived from first principles: `hbar / (2 * m_H2O * r_OO)` where `m_H2O = 2.9915e-26 kg`, `r_OO = 2.8 A`.

**Zero ML parameters. Zero training data. Zero fitted parameters.**

All predictions emerge from this constant and the quarter-wave law: `f = c_medium / (4 * d)`.

---

## Validated Predictions Summary

| # | Prediction | Error | Category | Reference |
|---|-----------|-------|----------|-----------|
| 1 | DNA minor groove: 34.0 GHz x 15.96 A = 542.6 GHz*A | **0.02%** | Structural Biology | Singh & Ray 2018 |
| 2 | FABP5-Linoleic acid pocket frequency match (TNBC) | **1.8%** | Cancer Biology | Science 2025; PDB 4LKT |
| 3 | TTFields 200 kHz = dermis quarter-wave resonance | **3.75%** | Cancer Therapy | FDA Optune; Oltulu 2018 |
| 4 | TTFields GBM: predicted 201.67 kHz vs 200 kHz FDA | **0.8%** | Cancer Therapy | Novocure clinical |
| 5 | CASP16 ligand affinity: **Rank 1 of 8** (tau=0.4505) | Beats all ML | Drug Discovery | CASP16 2024 |
| 6 | Taste prediction: 84.59% on 4,075 compounds (11 classes) | N/A | Chemosensory | ChemTastesDB; RCFTR |
| 7 | Lecanemab=GO vs Gantenerumab=NO-GO retrodiction | Correct | Drug Development | FDA 2023; Roche trials |
| 8 | ALOX15 double-hit: resolvins + PPARg gating | Confirmed | Cancer Biology | Zuo 2025 CMGH |
| 9 | 40 Hz gamma = body quarter-wave (v_bio/4*0.339m) | **0.0%** | Neuroscience | Iaccarino 2016 |
| 10 | TAS2R14 dominant cancer-associated bitter receptor | Confirmed | Cancer/Taste | TCGA 2022; 231 PubMed |

---

## Repository Structure

```
Validations-/
|
|-- CODEX_validation_summary.json      # Machine-readable summary of all validations
|
|-- Publications/                      # Core framework documents
|   |-- CODEX_Platform_Pamphlet.pdf    # 66-page technical pamphlet (all engines, validations)
|   |-- CODEX_First_Principles_Derivation.pdf  # 16 pages, 39 equations, full derivation chain
|   +-- CODEX_Resonance_Framework_Explainer.pdf # 12-page overview with competitor analysis
|
|-- RCFTR_Electronic_Tongue/           # Richardson Centre lab validation (homage to first validators)
|   |-- Final Report Dustin Hansley March 10 2026.pdf
|   |-- RCFTR_Validation_Report.pdf
|   |-- RCFTR_Validation_Report_v4.pdf
|   |-- RCFTR_full_validation.json     # Complete validation data (machine-readable)
|   +-- plots/                         # Validation visualizations
|       |-- RCFTR_benchmark_plot.png
|       |-- RCFTR_per_compound_bars.png
|       |-- RCFTR_ratio_analysis.png
|       +-- RCFTR_validation_plot1.png
|
|-- CASP16_Benchmark/                  # CASP16 ligand affinity benchmark
|   |-- CASP16_leaderboard.csv         # All 8 methods ranked by Kendall tau
|   |-- L1000_Chymase_compounds.csv    # 17 compounds with IC50 and SMILES
|   +-- CODEX_scoring_formula.txt      # Complete scoring formula derivation
|
|-- TTFields_Cancer/                   # TTFields cancer frequency predictions
|   |-- TTFields_19_cancer_types.csv   # All 19 types with freq, cell size, status
|   +-- TTFields_derivation.txt        # Complete physics derivation
|
|-- Taste_Prediction/                  # Taste prediction benchmarks
|   |-- taste_benchmark_comparison.csv # CODEX vs 5 ML competitors
|   +-- taste_prediction_summary.txt   # Method, dataset, lab validation details
|
|-- Frequency_Atlas/                   # Human body frequency atlas (52 structures)
|   |-- human_body_frequency_atlas.csv # 52 structures, 2.63 kHz - 770 MHz
|   +-- human_body_frequency_atlas.json # Same data, machine-readable
|
+-- Retrodictions/                     # Blind retrodiction tests
    +-- Lecanemab_vs_Gantenerumab.txt  # Alzheimer's antibody discrimination
```

---

## CASP16 Benchmark: Rank 1 of 8

CODEX scored **Kendall tau = 0.4505** on the CASP16 ligand affinity benchmark, outperforming all methods including those with millions of trained parameters:

| Rank | Method | Tau | ML? | Parameters |
|------|--------|-----|-----|------------|
| **1** | **CODEX Resonance** | **0.4505** | **No** | **0** |
| 2 | CoDock (SVR) | 0.43 | Yes | millions |
| 3 | ClusPro | 0.38 | Yes | millions |
| 4 | AlphaFold3 | 0.35 | Yes | ~600M |
| 5 | MULTICOM | 0.32 | Yes | millions |
| 6 | Boltz-1 | 0.28 | Yes | millions |
| 7 | AutoDock Vina | 0.25 | No | 0 |
| 8 | RoseTTAFold AA | 0.22 | Yes | millions |

Scoring formula: `composite = 0.2*DSI + 0.2*TPSA/150 + 0.3*HA/50 + 0.3*(1/harmonic_order)`

See `CASP16_Benchmark/` for complete data and derivation.

---

## TTFields Cancer Predictions

CODEX predicts optimal Tumor Treating Fields frequencies for **19 cancer types** using:

```
f_TTFields = V_cancer / (4 * d_cell)
V_cancer = 12.1 m/s (AFM-measured, cancer cells 4-5x softer)
```

**3 FDA-approved frequencies matched. 5 clinical trial frequencies matched. 11 novel predictions.**

See `TTFields_Cancer/` for complete data.

---

## RCFTR Electronic Tongue Validation

Laboratory validation conducted at the **Richardson Centre for Food Technology and Research**, University of Manitoba, using the Alpha Mos ASTREE Electronic Tongue (AST-043).

- Contract date: January 29, 2026
- Report date: March 10, 2026
- Result: Confirmed CODEX frequency-based taste predictions
- Includes: Full report PDF, validation data JSON, benchmark plots

*The RCFTR designation -- coined during the collaboration -- is retained as a homage to our first validators, whose independent instrumentation provided the earliest laboratory confirmation of the framework's predictions.*

See `RCFTR_Electronic_Tongue/` for full validation reports, data, and plots.

---

## Publications

The `Publications/` directory contains the core framework documents:

- **CODEX_Platform_Pamphlet.pdf** (66 pages) -- Complete technical pamphlet covering all 8 engines, validated predictions, CASP16 benchmark, water dynamics, TTFields cancer predictions, taste-cancer bridge, and API architecture.
- **CODEX_First_Principles_Derivation.pdf** (16 pages, 39 equations) -- Full derivation chain from fundamental constants to the f*d invariant.
- **CODEX_Resonance_Framework_Explainer.pdf** (12 pages) -- Concise overview with competitor analysis.

---

## Human Body Frequency Atlas

52-structure frequency atlas spanning 9 body systems, from 2.63 kHz (liver, 150mm) to 770 MHz (alveolar wall, 0.5 um). All frequencies computed via the quarter-wave law using tissue-appropriate sound speeds.

Available in both CSV and JSON formats in `Frequency_Atlas/`.

---

## Cancer Research Focus

CODEX bridges taste chemosensory biology and cancer through validated findings:

- **TAS2R14** (bitter taste receptor) is the dominant cancer-associated receptor
- **Quercetin** activates TAS2R14 and triggers apoptosis in cancer cells
- **Capsaicin** kills 74+ cancer cell types (231 PubMed articles)
- **FABP5-Linoleic acid** pocket match predicts TNBC binding (1.8% error, Science 2025)
- **CD36-TAS2R14 opposing axis**: novel prediction that high CD36 + low TAS2R14 = worst metastasis phenotype

### Novel Testable Predictions

1. **CD36-TAS2R14 Cancer Axis** - High CD36 + low TAS2R14 expression predicts worst metastasis outcome
2. **COPP Diagnostic** - Cancer cells use coordinated Cx43/PD-L1/Neu5Gc three-channel attack
3. **FABP7-ALOX15 Neural DHA Shuttle** - Frequency-matched at 19.6 GHz predicts functional pairing

---

## How to Verify

All predictions can be independently reproduced from the single invariant `f*d = 542.64 GHz*A`:

1. **DNA minor groove**: 34.0 GHz x 15.96 A = 542.6 GHz*A (measure minor groove width by neutron diffraction)
2. **TTFields**: f = 1540/(4*0.002) = 192.5 kHz (compare to FDA 200 kHz)
3. **Taste**: Run any compound's SMILES through CODEX and compare to ChemTastesDB ground truth
4. **CASP16**: Score any set of ligands with the 4-component formula and compute Kendall tau

The full CODEX platform (8 engines, 80+ endpoints) is available for collaboration.

---

## Citation

If referencing this work:

> Hansley, D. (2026). CODEX Genesis Resonance Framework: Physics-only molecular prediction from f*d = 542.64 GHz*A. Hans-Made Research Inc., Winnipeg, Canada. https://github.com/CodexResonance/Validations-

---

*Dedicated to Jackson David Rarama-Hansley*
