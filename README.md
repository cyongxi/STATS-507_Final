# STATS 507 Final Project  
**AG News Text Classification: TF-IDF vs Head-Only DistilBERT**

## 1. Project Overview

This project evaluates and compares two text classification approaches for the **AG News** dataset:

1. **TF-IDF + LinearSVC baseline**
2. **DistilBERT with a frozen encoder (head-only training)**

The goal is to understand performance differences between traditional bag-of-words methods and modern transformer-based models under **resource-constrained settings**.

The project includes:
- Exploratory data analysis (EDA)
- Baseline model with TF-IDF features
- Learning curve analysis
- Experiments with DistilBERT (varying max_length, training steps)
- Error and confusion matrix analysis  
- Final report summarizing findings  

The full write-up is available in:  
**`STAT507_Final_Report.pdf`**

---

## 2. Repository Structure

```text
.
├── notebooks/
│   ├── 01_eda.ipynb                  # Exploratory data analysis
│   ├── 02_tfidf_baseline_and_lc.ipynb# TF-IDF baseline + learning curves
│   └── 03_distilbert_head.ipynb      # DistilBERT (head-only) experiments
│
├── results/                          # Plots and evaluation results
│   ├── Confusion Matrix — TF-IDF.png
│   ├── Confusion Matrix — DistilBERT v1.png
│   ├── Confusion Matrix — DistilBERT v2.png
│   ├── Learning curve — TF-IDF (Accuracy).png
│   └── Learning curve — TF-IDF (Macro-F1).png
│
├── STAT507_Final_Report.pdf          # Final two-page report (IEEE format)
├── requirements.txt                  # Python dependencies
└── README.md
