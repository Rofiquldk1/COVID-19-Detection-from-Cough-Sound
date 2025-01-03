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

### Key Metrics
| Dataset               | AUC  | Precision | Recall | F1-Score | Specificity |
|-----------------------|------|-----------|--------|----------|-------------|
| Cambridge             | 0.97 | 1         | -      | -        | -           |
| Coswara               | 0.98 | 1         | -      | -        | -           |
| COUGHVID              | 0.92 | 0.72      | -      | -        | -           |
| Virufy                | 0.93 | 0.93      | -      | -        | -           |
| Combined Dataset      | 0.99 | 1         | -      | -        | -           |

#### Combined Dataset Summary
- **Accuracy:** 0.97
- **AUC:** 0.97
- **Precision:** 0.95
- **Recall:** 0.96
- **F1-Score:** 0.96
- **Specificity:** 0.97

---

## Cross-Dataset Analysis
- **Observations:**
  - Highlights demographic and geographic differences in COVID-19 cough characteristics.
  - Underlines challenges in feature transferability across datasets.
  - Demonstrates improved model generalizability through dataset integration.

---

## Comparative Analysis
| Dataset Category     | Method                                      | AUC  | Precision | Recall |
|----------------------|---------------------------------------------|------|-----------|--------|
| **Cambridge (Asymptomatic)** | Brown et al. [9]      | 0.80 | 0.72      | 0.69   |
| | Dentamaro et al. [124]| 0.83 | 0.80      | 0.80   |
| | Chowdhury et al. [111]| 0.88 | 0.75      | 0.81   |
| | Proposed (DNDT+RFECV+BO+SMOTE+TM)| 0.95 | 0.92      | 0.95   |
| | Proposed (DNDF+RFECV+BO+SMOTE+TM)| 0.97 | 1         | 0.94   |
| **Cambridge (Symptomatic)** | Brown et al. [9]      | 0.87 | 0.70      | 0.90   |
| | Chowdhury et al. [33] | -    | 0.87      | 0.82   |
| | Dentamaro et al. [124]| 0.93 | 0.89      | 0.93   |
| | Chowdhury et al. [111]| 0.95 | 1         | 0.91   |
| | Aytekin et al. [83]   | 0.98 | 0.94      | 0.93   |
| | Proposed (DNDT+RFECV+BO+SMOTE+TM)| 0.97 | 1         | 0.93   |
| | Proposed (DNDF+RFECV+BO+SMOTE+TM)| 0.98 | 1         | 0.97   |
| **Coswara**           |
| Chowdhury et al. [111]| 0.66 | 0.76      | 0.47   |
| Proposed (DNDT+RFECV+BO+SMOTE+TM)| 0.84 | 0.52      | 0.80   |
| Proposed (DNDF+RFECV+BO+SMOTE+TM)| 0.92 | 0.72      | 0.93   |
| **COUGHVID**          |
| Pavel and Ciocoiu [84]| 0.76 | 0.69      | 0.68   |
| Proposed (DNDT+RFECV+BO+SMOTE+TM)| 0.81 | 0.83      | 0.79   |
| Proposed (DNDF+RFECV+BO+SMOTE+TM)| 0.93 | 0.93      | 0.94   |
| **Virufy**            |
| Soltanian and Borna [57]| -  | 1         | 0.95   |
| Islam et al. [60]     | -    | 1         | 0.95   |
| Chowdhury et al. [111]| 0.94 | 0.89      | 0.98   |
| Sobahi et al. [102]   | -    | 0.99      | 0.97   |
| Proposed (DNDT+RFECV+BO+SMOTE+TM)| 0.98 | 1         | 0.96   |
| Proposed (DNDF+RFECV+BO+SMOTE+TM)| 0.99 | 0.98      | 1      |
| **Virufy + NoCoCoDa** |
| Melek [89]            | 0.99 | 0.99      | 0.97   |
| Chowdhury et al. [111]| 0.98 | 0.99      | 0.98   |
| Proposed (DNDT+RFECV+BO+SMOTE+TM)| 0.99 | 1         | 0.99   |
| Proposed (DNDF+RFECV+BO+SMOTE+TM)| 0.99 | 1         | 0.99   |

---

## Conclusion
This research demonstrates the efficacy of deep neural decision trees and forests for COVID-19 detection through audio analysis. The integration of diverse datasets significantly enhances model adaptability and reliability, paving the way for effective diagnostic tools.

-
