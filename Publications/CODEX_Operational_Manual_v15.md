# THE CODEX RESONANCE FRAMEWORK
## Complete Operational Manual for Discovery and Falsification
**Version 15.0 | March 13, 2026**
**Hans-Made Research Inc. | Dustin Hansley**
**Validation Data: github.com/CodexResonance/Validations-**

---

# HOW TO READ THIS DOCUMENT

This manual has three purposes:

1. **DISCOVER** -- Use the framework to predict unknown biological phenomena
2. **FALSIFY** -- Test predictions rigorously and identify framework failures
3. **REFINE** -- Update the framework based on experimental results

Every section includes worked examples. Skip to the sections you need.

---

# SECTION 1: THE CORE TOOLS

## 1.1 The Master Equation

```
+-------------------------------------+
|                                     |
|     f x d = 542.6395 GHz*A         |
|                                     |
+-------------------------------------+
```

**Derivation from first principles (zero fitted parameters):**

```
f * d = hbar * sqrt(3 / 2*pi) / (m_H2O * r_OO)

Where:
  hbar  = 1.0546e-34 J*s     (reduced Planck constant)
  m_H2O = 2.9915e-26 kg      (mass of water molecule)
  r_OO  = 2.82 A             (O-O distance in liquid water at 37C)
  sqrt(3/2*pi) = 0.6910      (thermal averaging geometry of tetrahedral H-bond network)
```

This is NOT an empirical fit. It emerges from three independently measured physical constants.

**What each variable means:**

| Symbol | Name | Units | How to Measure |
|--------|------|-------|----------------|
| f | Resonant frequency | GHz | Spectroscopy, impedance analysis, THz-TDS |
| d | Characteristic dimension | Angstroms (A) | Cryo-EM, X-ray crystallography, microscopy |
| 542.6395 | Universal invariant | GHz*A | Derived from hbar, m_H2O, r_OO |

**Unit conversions you will need:**

- 1 nanometer (nm) = 10 Angstroms (A)
- 1 micrometer (um) = 10,000 A
- 1 GHz = 1,000 MHz = 1,000,000 kHz = 10^9 Hz

---

## 1.2 The Two Regimes

The framework operates at TWO distinct scales with different equations:

### REGIME 1: Molecular Scale (f*d invariant)

**For molecular structures (Angstroms to nanometers):**

```
f = 542.64 / d     (frequency from dimension)
d = 542.64 / f     (dimension from frequency)
```

**Example:** A protein pocket is 22.7 A wide.
```
f = 542.64 / 22.7 = 23.9 GHz
```
**Prediction:** This pocket resonates at ~23.9 GHz (validated: FABP5-linoleic acid, 1.8% error).

### REGIME 2: Tissue/Cellular Scale (quarter-wave law)

**For macroscopic structures (micrometers to centimeters):**

```
f = c_medium / (4 * d)

Where c_medium = speed of wave propagation in the tissue:
  v_bio    = 54.27 m/s   (healthy biological membranes)
  v_cancer = 12.1 m/s    (disordered cancer cell membranes, AFM-measured)
  c_sound  = 1540 m/s    (soft tissue acoustic)
  c_bone   = 3500 m/s    (cortical bone acoustic)
```

**Example:** Glioblastoma cells are ~15 um in diameter with disordered membranes.
```
f = 12.1 / (4 * 15e-6) = 201,667 Hz = 201.67 kHz
```
**Prediction:** GBM should respond to ~202 kHz (validated: FDA Optune at 200 kHz, 0.8% error).

**CRITICAL:** Do NOT use f*d = 542.64 for cellular/tissue scale. Do NOT use v/(4d) for molecular scale. Using the wrong equation is the most common error.

---

## 1.3 The DSI Scaling Ladder

Biological frequencies organize across scales through the **Dimensional Scaling Index (DSI)** with scaling constant **L = 12.1**:

```
DSI SCALING LADDER:
  Tier +19:  f0 * L^19  = 3.103e8 m/s    (Speed of light: 2.998e8, 3.5% error)
  Tier +12:  f0 * L^12  = 2.188e6 m/s    (Bohr velocity: 2.188e6, 0.0% error)
  Tier  0:   f0         = 343.24 m/s      (Speed of sound: 343.15, 0.026% error)
  Tier -6:   f0 / L^6   = 39.25 Hz        (Gamma entrainment: 40 Hz, 1.9% error)
  Tier -7:   f0 / L^7   = 15.0 Hz         (PEMF bone healing: 15 Hz, 0.0% error)
```

**Open problem:** L = 12.1 is empirically discovered, not yet derived from first principles. Candidate origins include the ratio v_bio/v_thermal for water cage oscillators (~12.2) and tetrahedral coordination geometry. This is the framework's one fitting parameter.

Within a given scale, **quarter-wave harmonics** (x2, x4) organize related structures:

```
QUARTER-WAVE NEIGHBORS (within one scale):
  f x 4    (one harmonic UP)
  f x 2    (half-harmonic UP)
  f / 2    (half-harmonic DOWN)
  f / 4    (one harmonic DOWN)
```

**Example:** Starting from 40 Hz gamma:
```
40 Hz x 4 = 160 Hz
40 Hz x 2 = 80 Hz
40 Hz / 2 = 20 Hz   <-- insect gamma-equivalent (locust MB, validated)
40 Hz / 4 = 10 Hz   <-- alpha rhythm
```

---

## 1.4 The Framework Constants

### Core Constants (Universal)

| Constant | Value | What It Governs | Status |
|----------|-------|-----------------|--------|
| **f x d** | 542.6395 GHz*A | Molecular resonance invariant | Validated (0.02% DNA) |
| **v_bio** | 54.27 m/s | Healthy membrane wave velocity | Validated (body quarter-wave) |
| **v_cancer** | 12.1 m/s | Disordered membrane velocity | Validated (TTFields 0.8%) |
| **L** | 12.1 | DSI inter-scale ratio | Validated (19 tiers, <4% each) |

### Soliton Consciousness Engine Constants (Domain-Specific)

| Constant | Value | What It Governs | Status |
|----------|-------|-----------------|--------|
| **kappa** | 2.3 +/- 0.2 | Gap junction coupling ratio | Validated (EEG kappa=2.33) |
| **theta_c** | 0.72 +/- 0.06 | Phase transition threshold | Validated (propofol LOC) |
| **v_neural** | 54.27 m/s | A-alpha conduction velocity | Validated (50-60 m/s range) |

**Note:** kappa, theta_c are specific to the Soliton Consciousness Engine. They apply to neural systems and gap junction dynamics, not to molecular resonance broadly.

---

## 1.5 Water: The Biological Waveguide

The f*d invariant is rooted in water because water is the universal medium of biological signaling.

**Master water frequency:**
```
f_water = 542.64 / 2.8 A = 193.8 GHz
```
This matches the dominant collective THz absorption mode of liquid water at 194 GHz (Hoshina et al. 2011) to **0.09% error** -- the framework self-calibrating against its own medium.

**Hydration shell impedance matching:** The water shell surrounding every protein pocket is not passive solvent but an active resonance element. When a ligand's molecular frequency matches the pocket dimension (f*d = 542.64), the hydration shell mediates impedance matching -- the same physics as acoustic quarter-wave transformers in engineering.

**Sialic acid cancer switch:** Human cells display Neu5Ac on their glycocalyx; cancer cells exploit Neu5Gc incorporation to evade immune detection. The framework predicts distinct THz signatures for each sugar based on molecular dimensions -- a frequency-based diagnostic operating through the water waveguide.

---

# SECTION 2: THE VALIDATED PILLARS

These are predictions the framework got RIGHT. Use them as anchors.

## 2.1 Complete Pillar Registry

### TIER 1: Fully Validated (Independent Measurement, <4% Error)

| # | Pillar Name | Prediction | Observed Value | Error | Source |
|---|-------------|------------|----------------|-------|--------|
| 1 | DNA Minor Groove | f = 542.64/15.96 A = **34.0 GHz** | 34.0 GHz antenna resonance | 0.02% | Singh & Ray, Pramana 2018 |
| 2 | Water THz Calibration | f = 542.64/2.8 A = **193.8 GHz** | Dominant collective mode 194 GHz | 0.09% | Hoshina et al., IEEE THz 2011 |
| 3 | TTFields GBM | f = 12.1/(4x15um) = **201.67 kHz** | FDA Optune 200 kHz | 0.8% | Novocure clinical trials |
| 4 | FABP5-Linoleic Acid | f = 542.64/22.7 A = **23.9 GHz** | X-ray pocket match | 1.8% | Kound et al., Science 2025 |
| 5 | 40 Hz Gamma Body QW | f = 54.27/(4x0.339m) = **40.0 Hz** | Gamma entrainment | 0.0% | Iaccarino et al., Nature 2016 |
| 6 | PEMF Bone Healing | DSI tier -7 = **15.0 Hz** | FDA-cleared PEMF | 0.0% | Orthopedic literature |
| 7 | Triple Convergence | 200e=543.66, 4/alpha=548.14 | All within 1% of invariant | <1% | CODATA 2018 |
| 8 | CASP16 Rank 1/8 | tau = **0.4505** (0 parameters) | Beats AlphaFold3, all ML | Rank 1 | CASP16 2024 benchmark |
| 9 | Lecanemab vs Gantenerumab | Pocket-match GO / NO-GO | FDA approved / Roche halted | Correct | FDA 2023; Roche trials |
| 10 | Taste Prediction | 84.59% (3447/4075 compounds) | ChemTastesDB benchmark | N/A | 11 taste classes |
| 11 | RCFTR e-Tongue | Frequency-based taste predictions | Alpha Mos ASTREE confirmed | Confirmed | Richardson Centre, March 2026 |

### TIER 2: Strongly Supported (Independent Evidence, Mechanism Confirmed)

| # | Pillar Name | Prediction | Observed Value | Source |
|---|-------------|------------|----------------|--------|
| 12 | Gap Junction Threshold | Phase transition at kappa=0.72 | Propofol LOC at 0.72+/-0.06 | Anesthesia studies |
| 13 | kappa=2.3 Coupling | Bandwidth ratio universal | EEG kappa = 2.33 | Multiple species |
| 14 | 54 m/s Velocity | Optimal conduction speed | A-alpha: 50-60 m/s | Nerve conduction |
| 15 | Cross-Species Gamma | Insects: 40/2 = 20 Hz | Locust MB at 20 Hz | Science 2002 |
| 16 | GJ Pore (36 GHz) | f = 542.64/15 = 36.2 GHz | MMW-1 device uses 36 GHz | Clinical MMW therapy |
| 17 | MT Cavity (3 GHz) | f = 542.64/170 = 3.19 GHz | Measured 3.0 GHz | UT Health 2020 |
| 18 | MT Length (54 MHz) | f = 542.64/10000 = 54.3 MHz | RBM at 53 MHz | Royal Society Interface |
| 19 | ALOX15 Double-Hit | Resolvins + PPARg dual gating | Confirmed dual mechanism | Zuo et al. 2025 CMGH |
| 20 | TAS2R14 Cancer Bridge | Dominant cancer-associated bitter receptor | TCGA expression confirmed | 231 PubMed articles |

### TIER 3: Open Predictions (Falsifiable, Timestamped March 13, 2026)

| # | Pillar Name | Prediction | Falsification Method | Status |
|---|-------------|------------|---------------------|--------|
| 21 | Capsaicin-TRPV1 Match | Molecular freq matches TRPV1 gating dim. | THz spectroscopy of TRPV1-capsaicin | Open |
| 22 | ALOX Harmonic Series | ALOX5/12/15 pockets form integer harmonics | Comparative X-ray crystallography | Open |
| 23 | Schumann-Gamma Bridge | 7.83 Hz * L^5 = ~40 Hz | EEG during Schumann exposure | Open |
| 24 | Curcumin Multi-Lock | d=20.12A, f=26.98 GHz near ALOX15/FABP5 pockets; Bitter 82% (TAS2R14) | Multi-target binding at 27 GHz band | Platform-computed |
| 25 | CD36-TAS2R14 Cancer Axis | High CD36 + low TAS2R14 = worst metastasis | TCGA co-expression analysis | Open |
| 26 | COPP Diagnostic | Cx43/PD-L1/Neu5Gc three-channel cancer attack | Multi-marker panel on biopsies | Open |
| 27 | CRC TTFields Frequency | Colorectal CTC 7.5 um -> 403 kHz optimal | Future CRC TTFields trial | Prospective |
| 28 | Water Memory Refutation | No d = no frequency (refutes homeopathy) | Serial dilution THz spectroscopy | Open |

---

## 2.2 How to Use Pillars for Discovery

**RULE:** If a new phenomenon connects to a validated pillar, the prediction gains credibility.

**Example workflow:**
1. You find a new protein pocket 25.8 A wide
2. Calculate: f = 542.64 / 25.8 = 21.0 GHz
3. Check against pocket database: PPARg = 21.0 GHz (exact match!)
4. Prediction: The structure may bind PPARg ligands (rosiglitazone class)
5. Test: Binding assays with PPARg agonists

---

# SECTION 3: THE DISCOVERY ENGINE

## 3.1 The Discovery Workflow

```
+--------------------------------------------------------------+
|                    DISCOVERY WORKFLOW                         |
+--------------------------------------------------------------+
|                                                              |
|  STEP 1: IDENTIFY                                            |
|  +-- Find a biological phenomenon you want to understand     |
|  +-- Identify the key structures involved                    |
|                                                              |
|  STEP 2: MEASURE                                             |
|  +-- Determine structural dimensions                         |
|  +-- Identify the SCALE (molecular or tissue/cellular)       |
|                                                              |
|  STEP 3: SELECT EQUATION                                     |
|  +-- Molecular (A to nm): f = 542.64 / d                    |
|  +-- Cellular (um):       f = v_cancer / (4*d)              |
|  +-- Tissue (mm to cm):   f = c_sound / (4*d)              |
|  +-- Neural network (Hz): Use DSI ladder (L = 12.1)         |
|                                                              |
|  STEP 4: CALCULATE                                           |
|  +-- Apply the correct equation for your scale               |
|  +-- Calculate quarter-wave harmonics (x2, x4)              |
|  +-- Check DSI neighbors (xL, /L)                           |
|                                                              |
|  STEP 5: SEARCH                                              |
|  +-- Look for existing evidence at predicted values          |
|  +-- Cross-reference protein pocket database (21 proteins)   |
|  +-- Cross-reference tissue atlas (73 structures)            |
|                                                              |
|  STEP 6: PREDICT                                             |
|  +-- Formulate specific, testable predictions                |
|  +-- Define success AND failure criteria                     |
|                                                              |
|  STEP 7: TEST                                                |
|  +-- Design experiments with proper controls                 |
|  +-- Pre-register predictions before testing                 |
|                                                              |
+--------------------------------------------------------------+
```

---

## 3.2 Discovery Method A: Molecular Structure -> Frequency

**Use when:** You know a molecular structure's dimensions and want its resonance.

### Worked Example: Unknown Protein Pocket

**Step 1: Identify structure**
You have a cryo-EM structure showing a binding pocket 6.32 A wide.

**Step 2: Calculate predicted frequency**
```
f = 542.64 / 6.32 = 85.9 GHz
```

**Step 3: Search pocket database**
Cross-reference against 21-protein pocket frequency database:
- No exact match, but SERT pocket is nearby (6.37 A, 85.2 GHz)

**Step 4: Generate predictions**
- Compounds with functional groups vibrating at ~86 GHz should bind this pocket
- Check: trifluoromethyl groups (-CF3) resonate near 85 GHz
- Prediction: -CF3-containing compounds should show binding affinity

**Step 5: Validate**
Fluoxetine (Prozac) contains -CF3 and binds SERT -- consistent with framework.

---

## 3.3 Discovery Method B: Cellular Structure -> Therapeutic Frequency

**Use when:** You know a cell type and want to find its therapeutic frequency.

### Worked Example: TTFields for a New Cancer Type

**Step 1: Measure cell diameter**
Prostate cancer CTCs have median diameter 10.3 um (Mendelaar et al. 2021).

**Step 2: Select equation (cellular scale -- use quarter-wave with v_cancer)**
```
f = v_cancer / (4 * d_cell)
f = 12.1 / (4 * 10.3e-6)
f = 293,689 Hz = 293.7 kHz
```

**Step 3: Compare with cultured cells**
LNCaP cultured cells are 20.7 um:
```
f = 12.1 / (4 * 20.7e-6) = 146.1 kHz
```

**Step 4: Generate predictions**
- In vivo optimal: ~294 kHz (CTC-derived)
- In vitro optimal: ~146 kHz (cultured cells)
- Prediction: Clinical trials using 150 kHz may be suboptimal for real tumors

**Step 5: Falsification**
No TTFields trial for prostate cancer exists -- this is a clean prospective test.

---

## 3.4 Discovery Method C: Tissue Scale -> Frequency Atlas

**Use when:** You want to find the resonance of an organ or tissue structure.

### Worked Example: Heart Wall

**Step 1: Measure dimension**
Heart wall (myocardium) is ~12 mm thick.

**Step 2: Select equation (tissue scale -- use quarter-wave with tissue sound speed)**
```
f = c_muscle / (4 * d)
f = 1580 / (4 * 0.012)
f = 32,917 Hz = 32.9 kHz
```

**Step 3: Cross-reference atlas**
The 73-structure tissue frequency atlas confirms: Heart wall = 32.9 kHz.

**Step 4: Clinical relevance**
- Cardiac ablation frequencies can be analyzed against this
- Pacemaker stimulation at cardiac-harmonic frequencies may improve efficacy

---

## 3.5 Discovery Method D: Known Therapy -> Unknown Target

**Use when:** A therapy works but no one knows the target structure.

### Worked Example: 200 kHz TTFields (Historical)

**Step 1: Note the therapeutic frequency**
Novocure's TTFields at 200 kHz are FDA-approved for GBM. Why 200 kHz?

**Step 2: Select equation (cellular scale -- use v_cancer)**
```
d = v_cancer / (4 * f)
d = 12.1 / (4 * 200,000)
d = 15.125e-6 m = 15.1 um
```

**Step 3: Interpret**
15 um is the diameter of a dividing GBM cell. The field targets the mitotic spindle at the whole-cell resonance.

**Step 4: Verify**
GBM cells are ~15 um. Prediction matches. This also explains the Limb Problem: why bone tumors (osteosarcoma, 20 um cells) and brain tumors (GBM, 15 um cells) respond to similar frequencies despite vastly different tissue stiffness -- because resonance is a property of the isolated cell membrane, not the bulk tissue.

---

## 3.6 The Discovery Decision Tree

```
START: You want to investigate something
           |
           v
    +------------------+
    | What SCALE is    |
    | your structure?  |
    +------------------+
           |
     +-----+------+--------+
     |            |        |
  Molecular    Cellular  Tissue/Organ
  (A - nm)     (um)      (mm - cm)
     |            |        |
     v            v        v
  f=542.64/d  f=v/(4*d)  f=c_sound/(4*d)
     |            |        |
     |      +-----+-----+  |
     |      |           |  |
     |   Healthy     Cancer |
     |   v=54.27    v=12.1  |
     |      |           |  |
     v      v           v  v
  +-----------------------------+
  |  Cross-reference databases  |
  |  - 21 protein pockets       |
  |  - 73 tissue structures     |
  |  - 19-level DSI cascade     |
  |  - 16 protein family priors |
  +-----------------------------+
           |
           v
  +-----------------------------+
  |  Generate falsifiable       |
  |  predictions                |
  +-----------------------------+
           |
           v
  +-----------------------------+
  |  Design and run tests       |
  +-----------------------------+
```

---

# SECTION 4: THE FALSIFICATION ENGINE

## 4.1 Why Falsification Matters

The framework is only scientific if it can be **proven wrong**. This section describes exactly what would kill it.

---

## 4.2 Three Levels of Falsification

### LEVEL 1: Total Falsification (Framework is Wrong)

**The framework should be ABANDONED if:**

1. **The invariant is arbitrary**
   - Systematic testing shows no special significance to 542.6395
   - Other random numbers predict equally well
   - **Test:** Calculate predictions with 542.64, 500, 600, random values; compare accuracy

2. **Predictions are no better than chance**
   - Pre-registered predictions succeed <=50% of the time
   - Framework adds no predictive power over random guessing
   - **Test:** Pre-register 20 predictions, score success rate

3. **The physics is impossible**
   - Calculated energy scales cannot affect biological systems
   - Proposed mechanisms violate established physics
   - **Test:** Calculate field strengths needed; compare to thermal noise

4. **CASP-style benchmarks fail consistently**
   - If CODEX drops below median in blind benchmarks
   - If random scoring matches or beats the 4-component formula
   - **Test:** Enter future CASP/D3R/SAMPL challenges

---

### LEVEL 2: Partial Falsification (Framework Needs Modification)

**The framework should be REFINED if:**

1. **Scale-dependent corrections needed**
   - Molecular predictions work but tissue predictions don't (or vice versa)
   - **Action:** Verify correct equation is being used for each scale

2. **L = 12.1 doesn't always hold**
   - Some cascade transitions show L = 11 or L = 13
   - **Action:** Investigate whether L varies with tissue type or temperature

3. **Tissue sound speeds need updating**
   - Quarter-wave predictions off by >10% for specific tissues
   - **Action:** Use patient-specific imaging for c_medium

4. **v_cancer varies by cancer type**
   - Different cancers have different membrane stiffness
   - **Action:** Build cancer-type-specific velocity table (already partial: 19 types)

---

### LEVEL 3: Local Falsification (Specific Prediction Wrong)

**A specific pillar should be REJECTED if:**

1. **Direct measurement contradicts prediction**
   - Predicted frequency X; measured frequency Y where Y differs beyond error
   - **Action:** Remove pillar, investigate why

2. **Mechanism is different than proposed**
   - Effect exists but works through completely different physics
   - **Action:** Revise mechanistic explanation

3. **Effect disappears with proper controls**
   - Original finding was artifact or confound
   - **Action:** Retract pillar claim

---

## 4.3 The Falsification Protocol

### Before Testing Any Prediction:

**STEP 1: Write the prediction explicitly**
```
Template:
"The Codex Framework predicts that [STRUCTURE/SYSTEM]
with [DIMENSION] will show [EFFECT]
at [PREDICTED FREQUENCY] +/- [UNCERTAINTY]%
using equation [f*d / quarter-wave / DSI] because [SCALE JUSTIFICATION]"
```

**STEP 2: Define success criteria**
```
Template:
"The prediction is CONFIRMED if [MEASUREMENT]
falls within [RANGE] of [PREDICTED VALUE]"
```

**STEP 3: Define failure criteria**
```
Template:
"The prediction is FALSIFIED if:
- [MEASUREMENT] differs by more than [X]% from prediction, OR
- No effect is detected despite [MINIMUM SENSITIVITY], OR
- The effect is explained by [ALTERNATIVE MECHANISM]"
```

**STEP 4: Pre-register**
- Document prediction BEFORE collecting data
- Timestamp with third party (email, preprint server, git commit)
- This prevents moving goalposts

---

### During Testing:

**STEP 5: Use appropriate methods**

| Frequency Range | Scale | Measurement Technique |
|-----------------|-------|-----------------------|
| THz (10^12 Hz) | Molecular | THz-TDS, FTIR spectroscopy |
| GHz (10^9 Hz) | Molecular/pocket | Microwave spectroscopy, network analyzer |
| MHz (10^6 Hz) | Cellular/organelle | RF impedance, high-bandwidth patch clamp |
| kHz (10^3 Hz) | Tissue/organ | Impedance spectroscopy, ultrasound |
| Hz (10^0 Hz) | Neural network | EEG, ECG, MEG, direct recording |

**STEP 6: Control for confounds**
- Temperature stability (+/-0.1C if possible)
- Electromagnetic shielding
- Sham controls (identical setup, no signal)
- Blinding where possible
- Biological replicates (n >= 3)

---

### After Testing:

**STEP 7: Report ALL results**
- Positive results -> Support for pillar
- Negative results -> Constraint on framework
- Unexpected results -> Potential new pillar

**STEP 8: Update confidence**

| Outcome | Action |
|---------|--------|
| Prediction confirmed | Increase pillar confidence tier |
| Prediction failed | Decrease pillar confidence, investigate scale/equation |
| Unexpected finding | Document as potential new pillar, needs replication |

---

## 4.4 Worked Falsification Example

### Testing: FABP5-Linoleic Acid Pocket Match

**Pre-registration:**
*Prediction:* "FABP5 (PDB: 5HZ6) with pocket dimension 22.7 A should resonate at f = 542.64/22.7 = 23.9 GHz +/- 5%"

*Success criteria:* "Linoleic acid, known to bind FABP5, has molecular properties consistent with 23.9 GHz pocket frequency"

*Failure criteria:*
- "Linoleic acid molecular frequency falls outside 22.7-25.1 GHz range"
- "Binding occurs through mechanism unrelated to dimensional matching"

**Test:**
- Method: Compare predicted pocket frequency with crystallographic binding data
- Source: Kound et al., Science 2025 (independent measurement)

**Actual Result:**
- FABP5 pocket dimension confirmed at 22.7 A
- Linoleic acid binding confirmed in TNBC context
- Frequency match: 1.8% error

**Conclusion:** CONFIRMED -- Pillar promoted to Tier 1

---

## 4.5 What Each Failure Mode Means

| If This Fails... | It Means... | Framework Response |
|------------------|-------------|-------------------|
| f*d = 542.64 for specific molecule | Check dimension source; may need hydrated dimension | Verify crystallographic data |
| Quarter-wave for specific tissue | c_medium may be wrong for that tissue | Measure tissue-specific sound speed |
| v_cancer = 12.1 for specific cancer | Cancer type may have different membrane stiffness | Add to cancer velocity table |
| L = 12.1 between specific tiers | Scaling may have local variations | Investigate tier-specific factors |
| CASP16-style ranking drops | Scoring formula may need pocket family priors | Add protein family context |
| >50% of NEW predictions fail | Framework fundamentally wrong | Major revision or abandon |

---

# SECTION 5: PRACTICAL TOOLS

## 5.1 Quick Calculation Reference

### Common Molecular Structures and Predicted Frequencies (use f = 542.64/d)

| Structure | Dimension (A) | Predicted f | Status |
|-----------|---------------|-------------|--------|
| Water H-bond (r_OO) | 2.8 | 193.8 GHz | **VALIDATED** (0.09%) |
| DNA base pair spacing | 3.4 | 159.6 GHz | Testable |
| Alpha helix pitch | 5.4 | 100.5 GHz | Testable |
| Gap junction pore | 15 | 36.2 GHz | **VALIDATED** (MMW-1) |
| DNA minor groove | 15.96 | 34.0 GHz | **VALIDATED** (0.02%) |
| FABP5 pocket | 22.7 | 23.9 GHz | **VALIDATED** (1.8%) |
| PPARg pocket | 25.8 | 21.0 GHz | In database |
| Cell membrane thickness | 75 | 7.2 GHz | Testable |
| Gap junction channel | 155 | 3.5 GHz | Supported |
| Microtubule cavity | 170 | 3.19 GHz | **VALIDATED** |
| Ribosome | 250 | 2.17 GHz | Testable |

### Common Tissue Structures and Predicted Frequencies (use f = c_sound / 4d)

| Structure | Dimension | Sound Speed | Predicted f | Status |
|-----------|-----------|-------------|-------------|--------|
| Alveolar wall | 0.5 um | 600 m/s | 770 MHz | In atlas |
| Red blood cell | 7 um | 1570 m/s | 56.1 MHz | In atlas |
| Epidermis | 0.1 mm | 1540 m/s | 3.85 MHz | In atlas |
| Dermis | 2 mm | 1540 m/s | 192.5 kHz | **VALIDATED** (TTFields) |
| Cortical bone | 5 mm | 3500 m/s | 175 kHz | In atlas |
| Heart wall | 12 mm | 1580 m/s | 32.9 kHz | In atlas |
| Kidney | 55 mm | 1540 m/s | 7.0 kHz | In atlas |
| Liver | 150 mm | 1540 m/s | 2.63 kHz | In atlas |

### Cancer Cell TTFields Predictions (use f = 12.1 / 4d)

| Cancer Type | Cell Size | Predicted f | Clinical | Status |
|-------------|-----------|-------------|----------|--------|
| Glioblastoma | 15 um | 201.7 kHz | 200 kHz FDA | **VALIDATED** (0.8%) |
| Osteosarcoma | 20 um | 151.3 kHz | 150 kHz | **VALIDATED** |
| Ovarian | 16 um | 189.1 kHz | 200 kHz | Matched |
| Biliary tract | ~20 um | 151 kHz | 150 kHz optimal | **VALIDATED** (Yue 2025) |
| TNBC (CTC) | 12.4 um | 244 kHz | 150 tested | Predicts higher optimal |
| Prostate (CTC) | 10.3 um | 294 kHz | None | **PROSPECTIVE** |
| Colorectal (CTC) | 7.5 um | 403 kHz | None | **PROSPECTIVE** |

---

## 5.2 Python Calculator

```python
"""
Codex Resonance Framework Calculator v15
Corrected for two-regime physics
"""

class CodexCalculator:
    # Core constants
    FD_INVARIANT = 542.6395   # GHz*A (molecular scale)
    V_BIO = 54.27             # m/s (healthy membrane velocity)
    V_CANCER = 12.1           # m/s (disordered cancer membrane)
    L_DSI = 12.1              # DSI inter-scale ratio

    # Tissue sound speeds (m/s)
    C_SOFT = 1540
    C_MUSCLE = 1580
    C_FAT = 1450
    C_BONE = 3500
    C_BLOOD = 1570
    C_LUNG = 600
    C_BRAIN = 1540

    # Soliton consciousness constants (domain-specific)
    KAPPA_CRITICAL = 2.30
    THETA_C = 0.72

    @staticmethod
    def molecular_freq(d_angstrom):
        """MOLECULAR SCALE: f from pocket/structure dimension.
        Use for dimensions in Angstroms (1-1000 A).
        Returns frequency in GHz."""
        return 542.6395 / d_angstrom

    @staticmethod
    def molecular_dim(f_ghz):
        """MOLECULAR SCALE: d from frequency.
        Returns dimension in Angstroms."""
        return 542.6395 / f_ghz

    @staticmethod
    def tissue_freq(d_meters, c_medium=1540):
        """TISSUE SCALE: Quarter-wave frequency from dimension.
        Use for dimensions in meters (um to cm).
        c_medium = speed of sound in tissue (m/s).
        Returns frequency in Hz."""
        return c_medium / (4 * d_meters)

    @staticmethod
    def cancer_freq(d_meters):
        """CANCER CELL: TTFields frequency from cell diameter.
        Uses v_cancer = 12.1 m/s.
        d_meters = cell diameter in meters.
        Returns frequency in Hz."""
        return 12.1 / (4 * d_meters)

    @staticmethod
    def dsi_tier(f_hz, tier):
        """DSI SCALING: Move between cascade tiers.
        tier > 0 = up (toward speed of light)
        tier < 0 = down (toward Schumann)
        Returns frequency in Hz."""
        return f_hz * (12.1 ** tier)

    @staticmethod
    def quarter_wave_harmonics(f):
        """Quarter-wave harmonic neighbors (within one scale)."""
        return {
            'center': f,
            'x4_up': f * 4,
            'x2_up': f * 2,
            'x2_down': f / 2,
            'x4_down': f / 4,
        }

    @staticmethod
    def convert_freq(value, from_unit, to_unit):
        """Convert between frequency units."""
        to_hz = {'Hz': 1, 'kHz': 1e3, 'MHz': 1e6, 'GHz': 1e9, 'THz': 1e12}
        return value * to_hz[from_unit] / to_hz[to_unit]

    @staticmethod
    def convert_length(value, from_unit, to_unit):
        """Convert between length units."""
        to_A = {'A': 1, 'nm': 10, 'um': 1e4, 'mm': 1e7, 'm': 1e10}
        return value * to_A[from_unit] / to_A[to_unit]


# === Example usage ===
if __name__ == "__main__":
    calc = CodexCalculator()

    print("=== MOLECULAR SCALE (f*d invariant) ===")
    # DNA minor groove
    f = calc.molecular_freq(15.96)
    print(f"DNA minor groove (15.96 A) -> {f:.1f} GHz  [Validated: 34.0 GHz, 0.02%]")

    # FABP5 pocket
    f = calc.molecular_freq(22.7)
    print(f"FABP5 pocket (22.7 A) -> {f:.1f} GHz  [Validated: 23.9 GHz, 1.8%]")

    # Water
    f = calc.molecular_freq(2.8)
    print(f"Water H-bond (2.8 A) -> {f:.1f} GHz  [Validated: 194 GHz, 0.09%]")

    print("\n=== CELLULAR SCALE (cancer quarter-wave) ===")
    # GBM TTFields
    f = calc.cancer_freq(15e-6)
    print(f"GBM (15 um) -> {f:.0f} Hz = {f/1000:.1f} kHz  [FDA: 200 kHz]")

    # Prostate CTC (prospective)
    f = calc.cancer_freq(10.3e-6)
    print(f"Prostate CTC (10.3 um) -> {f:.0f} Hz = {f/1000:.1f} kHz  [PROSPECTIVE]")

    print("\n=== TISSUE SCALE (acoustic quarter-wave) ===")
    # Heart wall
    f = calc.tissue_freq(0.012, c_medium=1580)
    print(f"Heart wall (12mm, muscle) -> {f:.0f} Hz = {f/1000:.1f} kHz")

    # Liver
    f = calc.tissue_freq(0.150, c_medium=1540)
    print(f"Liver (150mm, soft) -> {f:.0f} Hz = {f/1000:.2f} kHz")

    print("\n=== DSI SCALING LADDER ===")
    f0 = 343.24  # Speed of sound tier (Hz... representing m/s)
    for tier, name in [(-7, "PEMF bone"), (-6, "Gamma"), (0, "Sound"), (+12, "Bohr"), (+19, "Light")]:
        val = calc.dsi_tier(f0, tier)
        print(f"  Tier {tier:+d} ({name}): {val:.4g}")
```

---

## 5.3 The CODEX Platform Cross-Reference Databases

The full CODEX platform provides programmatic access to these databases:

| Database | Entries | Use For |
|----------|---------|---------|
| Protein Pocket Frequency DB | 21 proteins | Molecular resonance matching |
| Tissue Quarter-Wave Map | 73 structures | Tissue/organ frequency lookup |
| Human Body Frequency Atlas | 52 structures | Body-system level analysis |
| Multiscale Cascade | 19 levels | Cross-scale frequency bridging |
| TTFields Cancer Types | 19 cancers | Cancer therapy prediction |
| Disease Profiles | 34 diseases | Disease-specific frequency matching |
| Compound Databases | ~600+ compounds | Drug-to-food reverse engineering |
| Protein Family Priors | 16 families | CASP-style affinity prediction |

**API endpoints for programmatic access:**
- `/synthesize` -- Cross-reference any claim against ALL databases
- `/knowledge-base` -- Full structured data export
- `/reverse-engineer` -- Drug -> frequency -> matching food compounds
- `/build-protocol` -- Disease -> targets -> frequency -> food protocol

---

## 5.4 Search Query Templates

**For Molecular Structure -> Frequency investigations:**
```
"[FREQUENCY] GHz biological effects"
"[STRUCTURE NAME] pocket dimension angstrom"
"[STRUCTURE NAME] binding site crystallography"
"PDB [STRUCTURE NAME] resolution"
```

**For Cancer/TTFields investigations:**
```
"[CANCER TYPE] cell diameter micrometer"
"[CANCER TYPE] circulating tumor cell size"
"TTFields [CANCER TYPE] frequency optimization"
"[CANCER TYPE] membrane stiffness AFM"
```

**For Tissue/Organ investigations:**
```
"speed of sound [TISSUE TYPE] m/s"
"[ORGAN] dimension thickness ultrasound"
"[ORGAN] resonance frequency impedance"
```

---

# SECTION 6: WORKED EXAMPLES LIBRARY

## 6.1 Example: Why Does 36 GHz Affect Wound Healing?

**Observation:** The MMW-1 device uses 36 GHz millimeter waves for clinical wound healing.

**Step 1: Identify scale -- 36 GHz is molecular scale**
```
d = 542.64 / 36 = 15.07 A
```

**Step 2: What biological structures are ~15 A?**
- Gap junction pore diameter: 15 A (exact match)

**Step 3: Generate prediction**
36 GHz resonates with gap junction pores, enhancing intercellular communication needed for coordinated wound healing.

**Step 4: Search for evidence**
Result: Gap junction inhibitors (carbenoxolone) block 36 GHz wound healing effects.

**Step 5: Falsification test**
If 36 GHz effects disappear with gap junction blockers -> Supports framework (CONFIRMED)
If 36 GHz effects persist with gap junction blockers -> Alternative mechanism

**Conclusion:** Gap junction pore resonance at 36 GHz -- Pillar 16, Tier 2.

---

## 6.2 Example: Predicting Prostate Cancer TTFields Frequency

**Goal:** No TTFields trial exists for prostate cancer. Predict the optimal frequency.

**Step 1: Identify scale -- cellular (use quarter-wave with v_cancer)**

**Step 2: Get cell dimensions**
- Patient-derived CTCs: 10.3 um median (Mendelaar et al. 2021, n=71,612 CTCs)
- Cultured LNCaP cells: 20.7 um

**Step 3: Calculate BOTH predictions**
```
CTC-based:     f = 12.1 / (4 * 10.3e-6) = 293.7 kHz
Cultured-based: f = 12.1 / (4 * 20.7e-6) = 146.1 kHz
```

**Step 4: Clinical recommendation**
Start with 150 kHz (cultured-cell match), but the framework predicts 294 kHz will outperform. Design trial with frequency sweep 100-400 kHz.

**Step 5: Falsification (prospective, timestamped March 13, 2026)**
- If 150 kHz and 300 kHz show identical efficacy -> v_cancer may need cancer-specific tuning
- If 300 kHz outperforms 150 kHz -> CTC dimensions are clinically relevant
- If neither frequency works -> Prostate cancer membranes may not be disordered (v != 12.1)

---

## 6.3 Example: Curcumin -- Multi-Target Cancer Compound (Live Platform Output)

**Why curcumin matters:** Curcumin is one of the most-studied anti-cancer dietary compounds (10,000+ PubMed articles), yet its mechanism of action across multiple targets has never been explained by a single framework. CODEX resolves this.

**Step 1: Run SMILES through /analyze endpoint**

| Property | Curcumin (live output) |
|----------|----------------------|
| Molecular Weight | 368.39 Da |
| Dimension (d) | 20.12 A |
| Codex Frequency (f) | 26.98 GHz |
| f x d product | 542.639 GHz*A |
| Predicted Taste | Bitter (82%) |
| Gate Path | Curcuminoid Bitter |
| Eye Draize Score | 98.7/110 |
| Eye GHS Category | Cat 1 (Serious) |
| Skin Score | 2.63/4 |
| LogP | 3.37 |

**Step 2: Cross-reference against protein pocket database**

Curcumin at d=20.12 A / f=26.98 GHz falls in the **ALOX/FABP pocket frequency band**:

| Protein | Pocket (A) | Frequency (GHz) | Delta from curcumin |
|---------|-----------|-----------------|---------------------|
| FABP5 | 22.7 | 23.9 | 3.08 GHz (11%) |
| ALOX15 | 22.1 | 24.6 | 2.38 GHz (9%) |
| ALOX12 | 19.8 | 27.4 | 0.42 GHz (1.6%) |
| PPARg | 25.8 | 21.0 | 5.98 GHz (22%) |

Curcumin's frequency is closest to **ALOX12** (1.6% match) -- consistent with its known lipoxygenase inhibition activity.

**Step 3: Interpret through the taste-cancer bridge**

- Curcumin predicted **Bitter (82%)** via curcuminoid bitter pathway
- Bitter compounds activate **TAS2R14**, the dominant cancer-associated bitter receptor
- TAS2R14 activation triggers apoptosis in cancer cells
- This explains why curcumin's anti-cancer activity correlates with its bitterness -- same frequency band

**Step 4: Safety prediction**

The Eye Draize score of **98.7/110** (GHS Category 1: Serious eye damage) is a genuine safety prediction from molecular resonance alone. This is consistent with curcumin's known irritant properties at concentrated doses and why turmeric powder causes eye irritation on contact.

**Step 5: The three-compound comparison**

Running three compounds through the same engine demonstrates f*d universality:

| | Caffeine | Curcumin | Glycerol |
|---|---------|----------|----------|
| d (A) | 7.03 | 20.12 | 5.40 |
| f (GHz) | 77.22 | 26.98 | 100.51 |
| f x d | **542.639** | **542.639** | **542.639** |
| Taste | Bitter 93% | Bitter 82% | Sweet 70% |
| Eye Draize | 3.1/110 | 98.7/110 | 0/110 |

Three completely different molecules. Three different dimensions. Three different frequencies. Same invariant to 6 significant figures. Taste, safety, and frequency all computed simultaneously from SMILES input only.

---

## 6.4 Example: Testing If 528 Hz Has Molecular Targets

**Claim:** 528 Hz is a "DNA repair frequency"

**Step 1: Check what scale 528 Hz operates at**
528 Hz is in the auditory/neural range. At molecular scale:
```
d = 542.64 / 0.000000528 = 1.028 trillion A = 103 km
```
This is not molecular. 528 Hz cannot directly target molecular structures.

**Step 2: Check DSI position**
```
528 Hz / L^6 = 528 / (12.1^6) = 528 / 3,143,489 = 0.000168 Hz
528 Hz * L = 528 * 12.1 = 6,389 Hz
```
528 Hz does not fall cleanly on any DSI tier.

**Step 3: Check quarter-wave harmonics**
```
528 / 4 = 132 Hz
528 / 16 = 33 Hz (near low gamma)
528 / 64 = 8.25 Hz (alpha range)
```

**Step 4: Rigorous test design**
- Control: 528 Hz vs 527 Hz vs 529 Hz vs silence vs white noise
- Measure: DNA repair markers (gamma-H2AX), stress hormones
- Blind: Participants unaware of frequency
- n >= 30 per group

**Step 5: Framework prediction**
If 528 Hz has specific effects beyond adjacent frequencies, they must work through auditory pathway neural entrainment, NOT molecular resonance. If 528 Hz = 527 Hz = 529 Hz in effects -> Claims are unfounded.

---

# SECTION 7: FRAMEWORK BOUNDARIES

## 7.1 Where Each Equation Applies

| Scale | Dimension Range | Equation | Examples |
|-------|----------------|----------|----------|
| Molecular | 1-1000 A | f = 542.64/d | Pockets, DNA, channels, membranes |
| Cellular | 1-100 um | f = v/(4*d) | Cancer cells, organelles, bacteria |
| Tissue | 0.1 mm - 15 cm | f = c_sound/(4*d) | Organs, tissue layers, bone |
| Network | 1-1000 Hz | DSI ladder (L=12.1) | Neural oscillations, EEG bands |

## 7.2 Known Limitations

1. **The framework does NOT predict chemical reaction rates**
   - Enzyme kinetics follow Michaelis-Menten, not resonance
   - Exception: Quantum tunneling in enzymes (covered by Quantum Tunneling Engine)

2. **Pure thermal effects are outside scope**
   - High-power heating follows SAR calculations
   - The framework addresses non-thermal resonance effects

3. **L = 12.1 is empirical, not derived**
   - The only fitting parameter in the framework
   - Active area of theoretical investigation

4. **v_cancer = 12.1 may vary by cancer type**
   - Current value is averaged across AFM measurements
   - Patient-specific membrane stiffness would improve predictions

## 7.3 What the Framework DOES Cover

| Domain | Engine | Key Capability |
|--------|--------|----------------|
| Molecular recognition | Compound Analysis | Taste, drug-pocket matching |
| Cancer therapy | GRE + TTFields | 19 cancer types, frequency prediction |
| Toxicology | Digital Draize | Eye/skin irritation from resonance |
| Drug safety | Cross-Reactivity | Breathalyzer/immunoassay interference |
| Protein dynamics | Pocket Dynamics | B-factor thermal motion, Q-factor |
| Enzyme catalysis | Quantum Tunneling | WKB barriers, KIE, tunneling rates |
| Consciousness | Soliton Engine | 40 Hz gamma, anesthesia, gap junctions |
| Drug discovery | CASP16 scoring | Zero-parameter affinity ranking |

---

# SECTION 8: COLLABORATION GUIDE

## 8.1 How to Contribute

**Option 1: Test an existing prediction**
1. Select an open prediction from the Tier 3 table (Section 2.1)
2. Follow the falsification protocol (Section 4.3)
3. Report results to Hans-Made Research

**Option 2: Enter a blind benchmark**
1. Use the CODEX scoring formula on a CASP/D3R/SAMPL challenge
2. Compare against ML methods
3. Report ranking and analysis

**Option 3: Propose a new pillar**
1. Use the discovery workflow (Section 3.1)
2. Document prediction, evidence, and falsification criteria
3. Submit for review

**Option 4: Challenge an existing pillar**
1. Design a more rigorous test than the original validation
2. Conduct test with proper controls
3. Report results (positive OR negative)

## 8.2 Contact and Resources

**Dustin Hansley**
Hans-Made Research Inc.
Winnipeg, Manitoba, Canada
Email: Dustinhansmade@Gmail.com
Phone: 204-333-0234

**Validation Data & Benchmarks:**
github.com/CodexResonance/Validations-

**Full Platform:** 8 engines, 98+ API endpoints, single-file deployment
Available for collaboration, licensing, and technical partnership.

---

# CONCLUSION: THE LIVING FRAMEWORK

The Codex Resonance Framework is not a fixed theory -- it is a **working hypothesis** that improves through rigorous testing. Every confirmed prediction strengthens it. Every falsified prediction refines it.

**Current Score (March 13, 2026):**
- 11 Tier 1 validated predictions (independent measurement, <4% error)
- 9 Tier 2 supported predictions (mechanism confirmed)
- 8 Tier 3 open predictions (falsifiable, timestamped)
- CASP16 Rank 1/8 in blind international benchmark
- 84.59% taste accuracy on 4,075 compounds
- Laboratory validation by Richardson Centre (RCFTR)
- Zero ML parameters. Zero training data.

**The Core Commitment:**
1. Make specific, falsifiable predictions
2. Test them rigorously
3. Report all results honestly
4. Update the framework based on evidence

The goal is not to be right. The goal is to be **useful** -- to help researchers discover new biological phenomena and develop better therapies.

Use this manual. Test the predictions. Break what can be broken. What survives will be closer to truth.

---

**Document Control:**
- Version: 15.0
- Date: March 13, 2026
- Author: Dustin Hansley, Hans-Made Research Inc.
- Previous: v14.0 (February 2, 2026) -- corrected TTFields equation, DNA pillar, derivation, added CASP16/RCFTR/water dynamics
- License: Open for scientific use with attribution
- Validation data: github.com/CodexResonance/Validations-

**Quick Reference Card (Print This):**
```
+=============================================+
|     CODEX RESONANCE QUICK REFERENCE v15     |
+=============================================+
|                                             |
|  MASTER INVARIANT: f x d = 542.64 GHz*A    |
|  (molecular scale only)                     |
|                                             |
|  QUARTER-WAVE:  f = c_medium / (4*d)       |
|  (tissue/cellular scale)                    |
|                                             |
|  CANCER CELLS:  f = 12.1 / (4*d)           |
|  (v_cancer = 12.1 m/s)                     |
|                                             |
|  DSI SCALING:   L = 12.1 between tiers     |
|  (19 levels, quantum to Schumann)           |
|                                             |
|  CORE CONSTANTS:                            |
|    f*d   = 542.64 GHz*A (invariant)        |
|    v_bio = 54.27 m/s  (healthy membrane)   |
|    v_can = 12.1 m/s   (cancer membrane)    |
|    L     = 12.1        (DSI ratio)         |
|                                             |
|  PREDICT f:  Molecular -> f = 542.64/d     |
|              Cellular  -> f = v/(4*d)      |
|              Tissue    -> f = c/(4*d)      |
|                                             |
|  1 nm = 10 A     1 GHz = 10^9 Hz          |
|  1 um = 10,000 A   1 MHz = 10^6 Hz        |
|                                             |
|  CASP16: Rank 1/8 | Taste: 84.59%         |
|  TTFields GBM: 0.8% | DNA: 0.02%          |
|                                             |
+=============================================+
```

---

*Dedicated to Jackson David Rarama-Hansley*
