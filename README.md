# Robust COVID-19 Detection from Cough Sounds


---

## Overview
This repository provides a robust and generalizable machine learning framework for detecting COVID-19 from cough sounds.
It leverages Deep Neural Decision Tree (DNDT) and Deep Neural Decision Forest (DNDF) models to achieve consistent, high-performing results across five individual datasets as well as a combined dataset integrating all of them. A preprint of the paper is available at: https://arxiv.org/abs/2501.01117

![image](https://github.com/user-attachments/assets/d57a3688-dc49-46d1-8656-b6b1dbbe3586)


### Highlights
- Robust COVID-19 cough classification using Deep Neural Decision Tree (DNDT) and Deep Neural Decision Forest (DNDF).
- Extensive experimentation across five individual datasets and a combined dataset, demonstrating strong performance across diverse sources.
- Cross-dataset analysis reveals demographic variability in COVID-19 cough sounds.
- Optimized Modeling Pipeline: Key features selected via Recursive Feature Elimination with Cross-Validation (RFECV) using Extra Trees Classifier, hyperparameters tuned via Bayesian Optimization, and data balanced using Synthetic Minority Over-sampling Technique (SMOTE).
- Performance enhancement achieved through threshold adjustment.

### Framework
- **Feature Extraction:** Extract acoustic audio features to distinguish COVID-19 positive and negative cases.
- **Feature Selection:** Use RFECV with Extra Trees Classifier to identify the most relevant features.
- **Hyperparameter Tuning:** Optimize DNDT and DNDF hyperparameters using Bayesian Optimization.
- **Data Balancing:** Apply SMOTE to balance positive and negative samples in the training set.
- **Threshold Optimization:** Adjust decision thresholds to maximize ROC-AUC and improve classification performance.

### Workflow Steps
- **Upload Files:** Upload the Extracted Features and Train-Test Split folders to your Google Drive. Open a Colab notebook and sequentially add the .ipynb files from the Codes folder.
- **Prepared Data.ipynb:** Perform data preparation in a format compatible with the models.
- **Bayesian Optimization.ipynb:** Perform Bayesian Optimization to fine-tune the hyper-parameters of the models.
- **Feature Selection (RFECV).ipynb:** Apply Recursive Feature Elimination with Cross-Validation (RFECV) to select the most important features.
- **Models.ipynb:** Prepare the models, including deep neural decision tree (DNDT) and forest (DNDF).
- **Classification.ipynb:** Perform the final classification task, including **Threshold Moving** and **Up-sampling**, and evaluate the models performance.
   
---

## Datasets
The proposed framework was rigorously evaluated on the following datasets:
- **Cambridge (asymptomatic and symptomatic)** - https://www.covid-19-sounds.org/en/
- **Coswara** - https://github.com/iiscleap/Coswara-Data
- **COUGHVID** - https://zenodo.org/records/7024894
- **Virufy** - https://github.com/virufy/virufy-data
- **Combined Virufy + NoCoCoDa** - https://doi.org/10.1109/ACCESS.2020.3018028
- **Combined Dataset:** Integration of all five individual datasets (Cambridge asymptomatic, Cambridge symptomatic, Coswara, COUGHVID, Virufy, NoCoCoDa) for comprehensive evaluation.
  
---

## Contributors
- **Rofiqul Islam**, Department of Computer Science and Engineering, University of Chittagong, Chattogram, 4331, Bangladesh
- **Professor Nihad Karim Chowdhury**, Department of Computer Science and Engineering, University of Chittagong, Chattogram, 4331, Bangladesh
- **Professor Ashad Kabir**, School of Computing, Mathematics, and Engineering, Charles Sturt University, Bathurst, NSW, 2795, Australia

### Cite this paper as
```bibtex
@article{islam2025robust,
  title={Robust covid-19 detection from cough sounds using deep neural decision tree and forest: A comprehensive cross-datasets evaluation},
  author={Islam, Rofiqul and Chowdhury, Nihad Karim and Kabir, Muhammad Ashad},
  journal={arXiv preprint arXiv:2501.01117},
  year={2025}
}
