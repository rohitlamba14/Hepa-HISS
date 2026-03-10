# Hepa-HISS: Explainable Machine Learning Framework for Hepatitis C Stage Prediction

This repository contains the implementation of the **Hepa-HISS framework**, proposed for accurate and explainable prediction of Hepatitis C disease stages using machine learning.

The framework integrates hybrid feature selection, interaction feature generation, and multiple machine learning classifiers to improve predictive performance and model interpretability.

---


## Framework Overview

The Hepa-HISS pipeline consists of the following stages:

1. Data preprocessing  
2. Feature scaling using StandardScaler  
3. Generation of polynomial interaction features  
4. Feature selection using:
   - ANOVA (SelectKBest)
   - Recursive Feature Elimination (RFE)
5. Handling class imbalance using BorderlineSMOTE  
6. Model training using multiple classifiers
7. Nested Cross-Validation for robust performance evaluation
8. Model explainability using SHAP / ELI5

---

## Machine Learning Models Used

The following classifiers were evaluated:

- Random Forest
- Support Vector Machine (SVM)
- Gradient Boosting
- XGBoost
- LightGBM
- K-Nearest Neighbors

Among these models, **Random Forest achieved the best performance with an accuracy of 96.58%.**

---

## Dataset

The dataset used in this study is related to **Hepatitis C diagnosis and staging** based on clinical biomarkers.

Classes include:

- Blood Donor
- Suspect Blood Donor
- Hepatitis C
- Fibrosis
- Cirrhosis

---

## Repository Structure


Hepa-HISS
│
├── Final Code_Hepa_HISS.ipynb
├── dataset.csv
├── requirements.txt
└── README.md
