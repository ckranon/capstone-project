# capstone-project

# Adversarial AI in Financial Management

**A Survey of Data Poisoning Techniques for Evasion Attacks on Financial Dataset**  
*Christian Kyle Ranon*  
Bachelor of Business and Data Analytics  
IE University – School of Science and Technology  
**Supervised by:** Luis Angel Galindo ([lgalindo@faculty.ie.edu](mailto:lgalindo@faculty.ie.edu))  
**Submission Date:** April 30, 2025

---

## 🔍 Overview

This project investigates the vulnerability of machine learning models in the financial domain to **Adversarial Machine Learning (AML)**—specifically, **data poisoning attacks** that occur during the training phase. It aims to showcase how easily predictive performance in risk assessment models can be undermined and offers insights into mitigation and defense strategies.

---

## 📘 Table of Contents

- [Overview](#-overview)  
- [Dataset](#-dataset)  
- [Tools & Technologies](#-tools--technologies)  
- [Methodology](#-methodology)  
- [Results & Discussion](#-results--discussion)  
- [Conclusion](#-conclusion)  
- [Reproducibility](#-reproducibility)  
- [References](#-references)  
- [Contact](#-contact)  

---

## 📊 Dataset

- **Name:** Financial Risk Assessment Dataset  
- **Source:** [Kaggle Dataset Link](https://www.kaggle.com/datasets/preethamgouda/financial-risk)  
- **EDA Report:** [View EDA Report](https://ckranon.github.io/capstone-project-eda/)

---

## 🧠 Tools & Technologies

- **Languages:** Python
- **Libraries:**
  - `scikit-learn`: Preprocessing, modeling
  - `AIJack`: Adversarial simulation (SVM poisoning)
  - `ydata-profiling`: Exploratory Data Analysis
  - `pandas`, `numpy`, `matplotlib`: Data manipulation & visualization

---

## ⚙️ Methodology

1. **Adversarial Model Design**  
   - Based on NIST’s taxonomy (2023), we define the adversary’s goal (availability attack), knowledge (white-box), and capabilities (full data access for simulation).

2. **Algorithm Under Attack**  
   - **Support Vector Machines (SVM)** using a linear kernel.
   - Attacks follow the approach defined in Biggio et al. (2012).

3. **Dataset Processing**  
   - Missing data imputed with `KNNImputer`
   - Categorical data encoded via `OrdinalEncoder` and one-hot encoding
   - Standardized numerical features with `StandardScaler`
   - Class balancing: 1,500 samples each for Low, Medium, and High Risk

---

## 📈 Results & Discussion

The poisoned dataset significantly reduced model performance, demonstrating the fragility of financial classification models under adversarial pressure. The discussion outlines attack effects and highlights potential defenses.

---

## 🧩 Conclusion

The paper argues for greater attention to **adversarial robustness** in the financial industry. It reveals how easy it is to introduce adversarial bias in datasets, especially those relying on tabular data in credit risk scoring.

---
