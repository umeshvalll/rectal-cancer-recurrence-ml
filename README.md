# Machine Learning-Based Rectal Cancer Recurrence Prediction

A machine learning research project focused on predicting recurrence after curative treatment for rectal cancer using clinical, imaging, and pathological variables.

## Research Overview

Recurrence prediction after curative rectal cancer treatment is challenging when relying only on conventional TNM staging. This study evaluated whether machine learning models using a broader set of routinely available patient features could improve recurrence prediction.

The study included **902 patients** treated with curative intent between 2017 and 2019, with a reported recurrence rate of **22.3%**.

## Machine Learning Pipeline

The project included:

- Data preprocessing
- Stratified 80:20 train-test split
- SMOTE-based oversampling for class imbalance
- Feature selection using SelectKBest with ANOVA F-value
- Hyperparameter optimization using GridSearch
- 5-fold cross-validation
- Comparative evaluation of multiple machine learning models

## Models Evaluated

- Logistic Regression
- Support Vector Machine (SVM)
- Random Forest
- XGBoost

## Results

XGBoost achieved the strongest overall performance among the evaluated models using the expanded feature set:

| Model | Accuracy | AUC |
|---|---:|---:|
| Logistic Regression | 0.650 | 0.610 |
| SVM | 0.760 | 0.700 |
| Random Forest | 0.750 | 0.700 |
| XGBoost | **0.796** | **0.705** |

XGBoost also achieved a specificity of **0.943**.

For comparison, models trained using only three TNM-based variables performed substantially lower, with XGBoost achieving an accuracy of **0.464** and AUC of **0.577**.

## My Machine Learning Contribution

My contribution focused on the machine learning component of the research, including data preprocessing, class-imbalance handling using SMOTE, feature selection, machine learning model development, model optimization, and comparative evaluation.

## Technologies

- Python
- Scikit-learn
- XGBoost
- Imbalanced-learn
- Pandas
- NumPy
- Machine Learning
- Statistical Analysis

## Published Research

**Machine learning-based prediction of recurrence after curative treatment for rectal cancer: A multi-model analysis from a tertiary cancer centre**

The published research paper is available in this repository:

[`research-paper/published-research-paper.pdf`](research-paper/published-research-paper.pdf)

## Research Disclaimer

This repository presents a research and machine learning implementation. The models are intended for research purposes and should not be considered a clinical diagnostic or treatment tool.
