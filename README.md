# Sepsis Prediction – Weill Cornell Medicine

## Overview
This project builds machine learning models to predict sepsis onset using ICU patient time-series data.

Models implemented:
- Decision Tree (Nested 5-fold CV)
- Random Forest (Nested 5-fold CV)

## Methods
Preprocessing:
- Feature aggregation (mean within observation window)
- Outlier capping (1st and 99th percentiles)
- Missing value imputation (median)
- Z-score normalization

Modeling:
- Nested Cross Validation (K=5 outer folds)
- GridSearchCV (scoring='roc_auc')
- Performance metrics: AUC, Precision, Recall, F1

## Results
Random Forest achieved improved stability compared to Decision Tree.
(You can add your final AUC numbers here.)

## Repository Structure
- sepsis_prediction_Student_Facing.ipynb – Full modeling workflow
- sepsis_prediction.docx – Project report
- eDataset_sepsis.zip – Dataset (compressed)

## How to Run
1. Install dependencies:
pip install -r requirements.txt

2. Open notebook:
jupyter notebook
