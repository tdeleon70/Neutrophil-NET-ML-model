# Neutrophil-NET-ML-model

### Enhanced Machine Learning Classification of Neutrophil Subtypes in Flow Cytometry Data

**Author:** Thomas DeLeon
**University of Houston–Downtown – MSDA Capstone Project (October 2025)**

---

## 📘 Overview

This project presents an end-to-end **machine learning pipeline** for classifying **neutrophil subtypes** from imaging flow cytometry data.
It builds upon an earlier proof-of-concept and advances it into a robust, interpretable, and validated analytical workflow.

The study focuses on improving biological data automation and interpretability by applying modern ML best practices to high-dimensional cellular data.

---

## 🧠 Key Features

* **Data Preprocessing Pipeline** — normalization, feature cleaning, and variance filtering
* **Feature Engineering** — biologically meaningful ratios (e.g., DNA intensity vs. nuclear area)
* **SMOTE-Tomek Resampling** — addresses class imbalance across six neutrophil subtypes
* **Model Optimization** — Random Forest tuned via `RandomizedSearchCV` with stratified cross-validation
* **Interpretability with SHAP** — explains feature influence and validates biological relevance
* **Cost-Benefit Analysis** — quantifies operational time and cost savings from automation

---

## 📊 Results Summary

* **Accuracy:** 99.93% (Cross-Validation: 99.977% ± 0.029%)
* **Macro F1 Score:** 99.88%
* **MCC:** 0.9992
* **Biological validity:** Model prioritizes DNA content, nuclear morphology, and scatter parameters — mirroring expert gating decisions.
* **Operational impact:** Estimated **>$150K annual savings** for labs processing ~10,000 samples per year.

---

## 🧩 Files Included

* **Capstone2 (1).ipynb** — Jupyter notebook containing the complete ML pipeline, data preparation, and SHAP analysis.
* **MSDA_Project_2_DELEON.pdf** — Final capstone paper summarizing methodology, analysis, and discussion.

---

## 🧬 Biological Context

Neutrophils, as part of the innate immune system, release **Neutrophil Extracellular Traps (NETs)** to capture pathogens.
Accurate classification of NETosis stages is crucial for studying autoimmune diseases, thrombosis, and inflammation.
This project automates that process using supervised learning to reduce manual gating time while maintaining expert-level accuracy.

---

## 🛠️ Technologies Used

* Python (scikit-learn, pandas, NumPy, matplotlib, seaborn)
* SHAP (Model Explainability)
* SMOTE-Tomek (Imbalanced-learn)
* Jupyter Notebook Environment

---

## 📈 Future Work

* Extend validation across multiple imaging cytometry platforms
* Explore gradient boosting and CNN-based deep learning architectures
* Implement uncertainty quantification and active learning for human-in-the-loop review

---

## 🧾 Citation

If referencing this work:
DeLeon, T. (2025). *Enhanced Machine Learning Classification of Neutrophil Subtypes in Flow Cytometry Data.*
University of Houston–Downtown, Master of Science in Data Analytics (Capstone Project).


