# 🧠 Causal Feature Extraction for Oxidation–Corrosion Mechanism Discovery
---

# 🔬 Overview 

This repository presents a causal machine learning framework for extracting mechanistically interpretable features governing high-temperature oxidation in complex alloys.

We bridge: Predictive materials modeling → Causal mechanism discovery by integrating: Doubly Robust Learning (DRL) approach, SHAP-based explainability, Conditional feature importance (CSVI) ranking, Multi-condition oxidation modeling

---
# 🧭 Framework Pipeline
<img width="958" height="512" alt="image" src="https://github.com/user-attachments/assets/477d6264-c4d7-4a38-b9b0-032c85867f28" />

```text
Raw Literature Data
        ↓
Curve Digitization (4,680 experiments)
        ↓
Feature Engineering (thermo + composition + physics)
        ↓
ML Models (XGBoost, Random Forest...)
        ↓
SHAP Explanation
        ↓
Conditional Causal Scoring (CSVI)
        ↓
Physical Interpretation High Score Feature
        ↓
Experiment Validation 
```
---
# 🧩 System Architecture
```text

        ┌────────────────────────────┐
        │  Alloy Composition Space   │
        └────────────┬───────────────┘
                     ↓
        ┌────────────────────────────┐
        │   ML Prediction Models     │
        └────────────┬───────────────┘
                     ↓
        ┌────────────────────────────┐
        │   SHAP Attribution Layer   │
        └────────────┬───────────────┘
                     ↓
        ┌────────────────────────────┐
        │   CSVI Causal Scoring      │
        └────────────┬───────────────┘
                     ↓
        ┌────────────────────────────┐
        │ Mechanistic Interpretation │
        └────────────────────────────┘
```
```text
📊 Dataset
📚 786 publications
📈 4,680 oxidation curves
🧪 2,414 unique alloy compositions
🧬 64 elemental species
```

# 📁 Repository Structure
```text
causal-feature-extraction/
│
├── data/
├── Causal_cal.ipynb
└── CSVI_cal.ipynb
```

---
# 📌 Applications
High-temperature alloy design
Oxidation prediction
Mechanism-aware materials discovery
Physics-informed machine learning
HEA (high-entropy alloy) screening

# Disclaimer

This repository features generalized prototypes and architectural workflows related to the manuscript 'A multi-agent large language model framework for mechanistic hypothesis generation in high-temperature alloy design', currently under review at Npj Computational Materials. Core proprietary datasets and specialized weights are withheld pending publication.

The dataset is not publicly available at the current stage due to ongoing peer review. Following publication, the processed data supporting the findings of this study will be released in this repository. Prior to publication, data access may be granted upon reasonable request to the corresponding author, in accordance with institutional and journal data-sharing policies.
