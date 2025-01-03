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
- **Virufy + NoCoCoDa**

### Performance Metrics
| Dataset                | AUC  | Precision | Recall | F1-Score | Specificity |
|------------------------|------|-----------|--------|----------|-------------|
| Cambridge              | 0.97 | 1         | -      | -        | -           |
| Coswara                | 0.98 | 1         | -      | -        | -           |
| COUGHVID               | 0.92 | 0.72      | -      | -        | -           |
| Virufy                 | 0.93 | 0.93      | -      | -        | -           |
| Virufy + NoCoCoDa      | 0.99 | 1         | -      | -        | -           |

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

## Conclusion
This research validates the potential of deep neural decision trees and forests for detecting COVID-19 through audio signals. Integrating diverse datasets enhances the model's reliability and adaptability, paving the way for practical diagnostic tools.

