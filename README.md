# Time Series Group Project

This repository contains the TSAC group project for time series classification of household appliance power consumption.

## Project goal
- Classify the type of appliance based on its electricity consumption time series.
- Analyze a small multivariate time series dataset and prepare it for modeling.

## Contents
- `study.ipynb` — main notebook containing:
  - dataset loading and overview
  - exploratory data analysis (EDA)
  - multivariate time series reshaping and channel analysis
  - class distribution and feature interpretation
- `data/` — dataset files used for analysis and submission
- `best_model.joblib`, `loocv_scor.joblib` — saved model and validation score artifacts

## Dataset overview
- 100 samples total
- 10 appliance classes
- 4-channel time series format inferred from 1460 measurements per sample
- Each sample appears to represent 4 distinct electrical signal channels over 365 time steps

## Key findings
- The dataset is balanced with 10 samples per class.
- One channel (`Ch2`) appears most discriminative for appliance classification.
- The data size is very small, so cross-validation and simple models are important to avoid overfitting.

## How to use
1. Open `study.ipynb` in Jupyter or VS Code.
2. Run the notebook cells sequentially to reproduce the EDA and preprocessing steps.
3. Inspect the saved artifacts if needed for model performance and submission.

