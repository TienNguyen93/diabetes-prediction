# Diabetes Prediction

## Problem Statement
Diabetes is a major public health concern in the United States, ranking as the eighth leading cause of death and impacting millions of Americans annually. According to the CDC, 38.4 million people in the U.S. (11.6% of the population) currently have diabetes, and 97.6 million adults (38% of the adult population) have prediabetes. It is also reported that there is 1 in 5 people with diabetes, and approximately 80% of those with prediabetes, are unaware of their condition. The economic burden of diabetes is equally significant, with total costs estimated at $413 billion in 2022 alone—$307 billion in direct medical expenses and $106 billion in indirect costs. The disease disproportionately affects those with lower socioeconomic status due to factors such as age, education, income, and geographic and racial disparities. As the absolute number of people with diabetes continues to grow, so do healthcare costs, and the economic impact on society underscores the importance of targeted early intervention strategies.

## Goals
(1) Determine key risk factors contributing to diabetes prediction. It is hypothesized that certain features will emerge as strong indicators of diabetes risk, guiding prevention and intervention strategies.

(2) Identify the most effective model for early diabetes screening and an optimal predictive model to assess diabetes risk, selected based on recall performance. It is hypothesized that these models will support different stages of detection and prevention.

## Dataset
[CDC Diabetes Health Indicators dataset](https://archive.ics.uci.edu/dataset/891/cdc+diabetes+health+indicators)

## Approach
### Machine Learning Algorithms
* Support Vector Machine
* Random Forest
* Logistic Regression
* XGBClassifier
* Multi-Layer Perceptrons

### Sampling techniques
* Stratified
* SMOTE (Synthetic Minority Over-sampling Technique)
* Random Under Sampling

### Dimensionality reduction technique
* PCA (Principal Component Analysis)

## Results
* Early Screening: Random Forest with either SMOTE or Random Under Sampling (**recall: ∼0.90**)
* Overall Prediction: XGBoost (**recall: 0.77**, **AUC ROC: 0.8**)
* Key predictors influence predicted results based on SHAP values:
  *  DiffWalk Difficult Walking)
  *  BMI
  *  Age
  *  HighChol (High Cholesterol)
