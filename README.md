# Robust COVID-19 Detection from Cough Sounds


---

## Overview
This study addresses a critical challenge in the field of audio-based health diagnostics: developing robust and generalizable machine-learning models for COVID-19 detection from cough sounds.
It introduces a framework for classifying COVID-19 from cough sound with cutting-edge machine-learning techniques. This framework leverages a deep neural decision tree (DNDT) and forest (DNDF) to deliver robust and reliable performance across five different datasets.

### Highlights
-	Robust COVID-19 cough classification using neural decision tree and forest.
-	Experimentation across five datasets and their merged set highlights dataset diversity.
-	Cross-datasets analyses show demographic variability in COVID-19 cough sounds.
-	RFECV and Bayesian optimization improved feature selection and model performance.
-	SMOTE oversampling and threshold moving enhanced data balance and classification.


### Framework
- **Feature Extraction:** Comprehensive extraction of audio features to differentiate COVID-19 positive and negative cases.
- **Feature Selection:** Utilization of recursive feature elimination with cross-validation (RFECV) for identifying essential features.
- **Model Optimization:** Implementation of Bayesian optimization to fine-tune deep neural decision tree (DNDT) and forest (DNDF) hyperparameters for optimal results.
- **Data Balancing:** Application of Synthetic Minority Over-sampling Technique (SMOTE) to ensure balanced training data.
- **Performance Optimization:** Threshold adjustment to maximize ROC-AUC metrics.

---

## Datasets
The proposed framework was rigorously tested on the following datasets:
- **Cambridge (asymptomatic and symptomatic)**
- **Coswara**
- **COUGHVID**
- **Virufy**
- **Combined Virufy + NoCoCoDa**

---

## Authors
- **Rofiqul Islam**, Department of Computer Science and Engineering, University of Chittagong, Chattogram, 4331, Bangladesh
- **Professor Nihad Karim Chowdhury**, Department of Computer Science and Engineering, University of Chittagong, Chattogram, 4331, Bangladesh
- **Professor Ashad Kabir**, School of Computing, Mathematics, and Engineering, Charles Sturt University, Bathurst, NSW, 2795, Australia



