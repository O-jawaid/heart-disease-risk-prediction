# Heart Disease Risk Prediction

A machine learning project that predicts a patient's risk of heart disease from clinical indicators, comparing five classification models to identify the strongest performer.

## Overview

Using a dataset of 302 patient records, I trained and evaluated five classification models, including Logistic Regression, Naive Bayes, Random Forest, SVM, and XGBoost, to predict the presence of heart disease based on clinical measurements such as chest pain type, cholesterol, and maximum heart rate. The goal was to identify not just the best-performing model, but also the clinical features most predictive of risk.

## Results

The **Support Vector Machine (SVM)** model performed best overall:

| Metric | Score |
|---|---|
| Accuracy | 86.9% |
| Precision | 87.9% |
| Recall | 87.9% |
| ROC-AUC | 0.91 |

The strongest predictive features were **chest pain type, maximum heart rate, ST depression, and number of major vessels**, all consistent with established clinical risk indicators for heart disease.

## Approach

- Cleaned and preprocessed the dataset, including handling missing values, one-hot encoding categorical variables, and feature scaling
- Performed exploratory data analysis to understand feature distributions and relationships with the target variable
- Trained and compared five classification models using consistent train/test splits
- Evaluated each model using accuracy, precision, recall, and ROC-AUC to account for both overall performance and class balance
- Analyzed feature importance to identify the clinical factors most associated with heart disease risk

## Tools & Libraries

Python, Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn

## Repository Contents

- [`notebook.ipynb`](./notebook.ipynb) — full analysis and modeling code, viewable directly on GitHub
- [`report.pdf`](./report.pdf) — full written project report
- [`presentation.pdf`](./presentation.pdf) — final presentation summarizing the project and results
- `data/` — dataset used for this analysis ([source noted below](#dataset))

## Dataset

This project uses the [UCI Heart Disease dataset](https://archive.ics.uci.edu/dataset/45/heart+disease), a widely used public dataset for cardiovascular risk prediction research.

## About This Project

This was completed as part of my B.S. in Data Science at the University of North Texas. It reflects my interest in applying machine learning to real-world, high-impact problems, in this case, using clinical data to support earlier identification of heart disease risk.
