# Robust COVID-19 Detection from Cough Sounds

### Authors
- **Rofiqul Islam**, Department of Computer Science and Engineering, University of Chittagong, Chattogram, 4331, Bangladesh
- **Nihad Karim Chowdhury**, Department of Computer Science and Engineering, University of Chittagong, Chattogram, 4331, Bangladesh
- **Muhammad Ashad Kabir**, School of Computing, Mathematics, and Engineering, Charles Sturt University, Bathurst, NSW, 2795, Australia

---

## Overview
This project introduces an innovative approach to identifying COVID-19 using cough sound analysis with cutting-edge machine learning techniques. The methodology leverages deep neural decision trees (DNDT) and forests (DNDF) to deliver robust and reliable performance across diverse datasets.

### Highlights
- **Feature Extraction:** Comprehensive extraction of audio features to differentiate COVID-19 positive and negative cases.
- **Feature Selection:** Utilization of recursive feature elimination with cross-validation (RFECV) for identifying essential features.
- **Model Optimization:** Implementation of Bayesian optimization to fine-tune DNDT and DNDF hyperparameters for optimal results.
- **Data Balancing:** Application of Synthetic Minority Over-sampling Technique (SMOTE) to ensure balanced training data.
- **Performance Optimization:** Threshold adjustment to maximize ROC-AUC metrics.

---

## Dataset Validation
The proposed solution was rigorously tested on the following datasets:
- **Cambridge (asymptomatic and symptomatic)**
- **Coswara**
- **COUGHVID**
- **Virufy**
- **Combined Virufy + NoCoCoDa**

---

## Cross-Dataset Analysis
- **Observations:**
  - Highlights demographic and geographic differences in COVID-19 cough characteristics.
  - Underlines challenges in feature transferability across datasets.
  - Demonstrates improved model generalizability through dataset integration.

---

## Conclusion
This research demonstrates the efficacy of deep neural decision trees and forests for COVID-19 detection through audio analysis. The integration of diverse datasets significantly enhances model adaptability and reliability, paving the way for effective diagnostic tools.


