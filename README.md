# Robust COVID-19 Detection from Cough Sounds


---

## Overview
This repository introduces a robust and generalizable machine learning framework for COVID-19 detection using cough sounds. The framework employs Deep Neural Decision Tree (DNDT) and Deep Neural Decision Forest (DNDF) models, achieving consistent and high performance across five individual datasets, as well as a unified dataset that combines all of them. The corresponding paper has been published in Expert Systems with Applications and is available at: https://doi.org/10.1016/j.eswa.2026.131235

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
- **Upload Files:** Upload the Extracted Features from our research for classification, along with the Train-Test Split folders, to your Google Drive to ensure consistent splits for both DNDT and DNDF.
- **Proposed_COVID_19_Detection_from_Cough_Sounds_Dataset_wise_Results.ipynb:** Run the code step by step and follow the comments in the Colab notebook for guidance to perform classification on each individual dataset.
- **COVID19_Cough_Detection_CrossSectional_and_Combined_Dataset_Results.ipynb:** Run the code and follow the comments in the Colab notebook for guidance. This notebook allows you to perform either a Cross-Sectional Study or a Combined Dataset analysis, one at a time.
   
---

## Datasets
The proposed framework was rigorously evaluated on the following datasets:
- **Cambridge (asymptomatic and symptomatic)** - https://www.covid-19-sounds.org/en/
- **Coswara** - https://github.com/iiscleap/Coswara-Data
- **COUGHVID** - https://zenodo.org/records/7024894
- **Virufy** - https://github.com/virufy/virufy-data
- **Combined Virufy + NoCoCoDa** - https://doi.org/10.1109/ACCESS.2020.3018028
- **Combined Dataset:** Integration of all five datasets (Cambridge asymptomatic, Cambridge symptomatic, Coswara, COUGHVID, Virufy, NoCoCoDa).
  
---

## Contributors
- **Rofiqul Islam**, Department of Computer Science and Engineering, University of Chittagong, Chattogram, 4331, Bangladesh
- **Professor Nihad Karim Chowdhury**, Department of Computer Science and Engineering, University of Chittagong, Chattogram, 4331, Bangladesh
- **Professor Ashad Kabir**, School of Computing, Mathematics, and Engineering, Charles Sturt University, Bathurst, NSW, 2795, Australia

### Cite this paper if you use our code or refer to our work:
```bibtex
@article{islam2025robust,
  title={Robust covid-19 detection from cough sounds using deep neural decision tree and forest: A comprehensive cross-datasets evaluation},
  author={Islam, Rofiqul and Chowdhury, Nihad Karim and Kabir, Muhammad Ashad},
  journal={arXiv preprint arXiv:2501.01117},
  year={2025}
}
