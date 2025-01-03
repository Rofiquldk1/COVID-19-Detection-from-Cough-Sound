# COVID-19 Detection from Cough Sounds

This project presents a robust framework for classifying COVID-19 cough sounds using advanced machine learning techniques. By leveraging deep neural decision trees and forests, the methodology ensures consistent performance across diverse cough sound datasets.

## Key Features
- Comprehensive audio feature extraction for distinguishing COVID-19 positive and negative samples.
- Feature selection through recursive feature elimination and cross-validation.
- Hyper-parameter tuning using Bayesian optimization.
- Balanced training data with synthetic minority over-sampling technique (SMOTE).
- Performance refinement via threshold optimization, maximizing the ROC-AUC score.

## Evaluation Results
The proposed method was evaluated on five datasets:
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

When all datasets were combined, the model achieved the following:
- **Accuracy**: 0.97
- **AUC**: 0.97
- **Precision**: 0.95
- **Recall**: 0.96
- **F1-Score**: 0.96
- **Specificity**: 0.97

## Cross-Dataset Insights
- Demographic and geographic differences in COVID-19-related cough sounds were identified.
- Highlighted challenges in transferring features across datasets.
- Dataset integration improves generalizability and enhances COVID-19 detection from audio signals.

## Conclusion
This research underscores the potential of leveraging advanced machine learning models for COVID-19 detection using cough sounds, offering a path toward more effective and generalized audio-based diagnostic tools.
