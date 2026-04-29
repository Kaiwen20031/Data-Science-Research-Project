# Data-Science-Research-Project

This repository contains the code and intermediate results for **Data Science Research Project – Part A (Progress Report)**.

## Overview

The stage analyses the relationship between COVID-19 policies and protective behaviours using survey data and policy data.  
All modelling and analysis are implemented using **Jupyter Notebook**.

---

## Repository Structure

### Root Directory

- `*.ipynb`  
  Jupyter Notebook files containing the full pipeline:
  - data cleaning
  - preprocessing
  - modelling
  - evaluation
  - feature importance analysis

- `OxCGRT_AUS_latest.csv`  
  Policy dataset used in the analysis.

- `australia.zip`  
  YouGov survey dataset (compressed due to large file size).

- `cleaned_data.csv`  
  Dataset after initial cleaning.

- `cleaned_data_preprocessing.csv`  
  Final dataset after preprocessing and feature engineering.

---

### Folders

- `data/`  
  Contains processed datasets after train-test splitting.

- `results/`  
  Stores model evaluation results and summary outputs.

- `Pictures/`  
  Contains all generated figures (e.g., feature importance plots).

---

## Workflow

The notebooks should be executed in the following order:

1. `clean.ipynb`  
   Data cleaning and preprocessing

2. `datasplit.ipynb`  
   Dataset splitting into training and testing sets

3. `LR.ipynb`  
   Logistic Regression (baseline model)

4. `Decision Tree.ipynb`  
   Decision Tree model with hyperparameter tuning

5. `XGBoost.ipynb`  
   XGBoost model with hyperparameter tuning

6. `RF.ipynb`  
   Random Forest model with hyperparameter tuning

7. `final_model.ipynb`  
   Final model evaluation on test datasets

8. `important_feature.ipynb`  
   Feature importance analysis and visualisation

---

## Notes

- The workflow follows a consistent pipeline across models:
  - stratified splitting
  - optional oversampling
  - cross-validation
  - model evaluation
  - feature importance analysis

- Feature importance is estimated using repeated model training and summarised using median values and interquartile ranges.

---

## Author

Kaiwen Du
