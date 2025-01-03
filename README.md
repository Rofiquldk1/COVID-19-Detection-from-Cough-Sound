# Robust COVID-19 Detection from Cough Sounds

### Authors
- **Rofiqul Islam**, Department of Computer Science and Engineering, University of Chittagong, Chattogram, 4331, Bangladesh
- **Nihad Karim Chowdhury**, Department of Computer Science and Engineering, University of Chittagong, Chattogram, 4331, Bangladesh
- **Muhammad Ashad Kabir**, School of Computing, Mathematics, and Engineering, Charles Sturt University, Bathurst, NSW, 2795, Australia

---

## Abstract
This study proposes an effective method for identifying COVID-19 from cough sounds using advanced machine learning models. By utilizing deep neural decision trees (DNDT) and deep neural decision forests (DNDF), the approach achieves consistent and reliable performance across multiple datasets.

### Key Contributions
- **Feature Extraction:** Extracts a wide range of audio features to distinguish COVID-19 positive and negative samples.
- **Feature Selection:** Employs recursive feature elimination with cross-validation (RFECV) to pinpoint the most critical features.
- **Hyperparameter Optimization:** Fine-tunes the DNDT and DNDF models using Bayesian optimization for enhanced performance.
- **Balanced Data Training:** Ensures fair representation of positive and negative samples through the Synthetic Minority Over-sampling Technique (SMOTE).
- **Performance Enhancement:** Optimizes model thresholds to maximize the ROC-AUC score.

---

## Dataset Evaluation
The proposed method was extensively validated on the following datasets:
- **Cambridge (asymptomatic and symptomatic)**
- **Coswara**
- **COUGHVID**
- **Virufy**
- **Virufy + NoCoCoDa (combined)**

### Performance Metrics
| Dataset               | AUC  | Precision | Recall | F1-Score | Specificity |
|-----------------------|------|-----------|--------|----------|-------------|
| Cambridge             | 0.97 | 1         | -      | -        | -           |
| Coswara               | 0.98 | 1         | -      | -        | -           |
| COUGHVID              | 0.92 | 0.72      | -      | -        | -           |
| Virufy                | 0.93 | 0.93      | -      | -        | -           |
| Combined Dataset      | 0.99 | 1         | -      | -        | -           |

### Results for Combined Dataset
- **Accuracy:** 0.97
- **AUC:** 0.97
- **Precision:** 0.95
- **Recall:** 0.96
- **F1-Score:** 0.96
- **Specificity:** 0.97

---

## Cross-Dataset Insights
- **Key Findings:**
  - Identifies demographic and geographic variations in COVID-19-related cough patterns.
  - Highlights challenges in transferring learned features across datasets.
  - Demonstrates how integrating datasets improves model generalizability and robustness.

---

## Comparison with State-of-the-Art Methods
| Dataset Category     | Method                                      | AUC  | Precision | Recall |
|----------------------|---------------------------------------------|------|-----------|--------|
| **Cambridge (Asymptomatic)** |
| Brown et al. [9]      | 0.80 | 0.72      | 0.69   |
| Dentamaro et al. [124]| 0.83 | 0.80      | 0.80   |
| Chowdhury et al. [111]| 0.88 | 0.75      | 0.81   |
| Proposed (DNDT+RFECV+BO+SMOTE+TM)| 0.95 | 0.92      | 0.95   |
| Proposed (DNDF+RFECV+BO+SMOTE+TM)| 0.97 | 1         | 0.94   |
| **Cambridge (Symptomatic)** |
| Brown et al. [9]      | 0.87 | 0.70      | 0.90   |
| Chowdhury et al. [33] | -    | 0.87      | 0.82   |
| Dentamaro et al. [124]| 0.93 | 0.89      | 0.93   |
| Chowdhury et al. [111]| 0.95 | 1         | 0.91   |
| Aytekin et al. [83]   | 0.98 | 0.94      | 0.93   |
| Proposed (DNDT+RFECV+BO+SMOTE+TM)| 0.97 | 1         | 0.93   |
| Proposed (DNDF+RFECV+BO+SMOTE+TM)| 0.98 | 1         | 0.97   |
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
This research validates the potential of deep neural decision trees and forests for detecting COVID-19 through audio signals. Integrating diverse datasets enhances the model's reliability and adaptability, paving the way for practical diagnostic tools.


