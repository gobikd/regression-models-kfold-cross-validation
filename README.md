# Regression Models with K-Fold Cross-Validation

This repository contains Python implementations of multiple regression algorithms evaluated using K-Fold Cross-Validation.

The project was developed as part of my machine learning journey with Hope AI. It demonstrates how different regression models can be validated using multiple folds rather than relying on a single train-test split.

---

## Project Objectives

- Apply K-Fold Cross-Validation to regression algorithms.
- Compare model performance using R² scores.
- Evaluate model stability across validation folds.
- Visualise actual versus predicted values.
- Analyse residuals and feature importance.
- Use proper dataset paths and repository organisation.
- Practice reproducible machine learning workflows.

---

## Regression Algorithms Included

| No. | Algorithm | Notebook |
|---|---|---|
| 1 | Simple Linear Regression | `01_simple_linear_regression_kfold.ipynb` |
| 2 | Multiple Linear Regression | `02_multiple_linear_regression_kfold.ipynb` |
| 3 | Support Vector Regression with StandardScaler | `04_svr_standardscaler_kfold.ipynb` |
| 4 | Decision Tree Regression | `05_decision_tree_regression_kfold.ipynb` |
| 5 | Random Forest Regression | `06_random_forest_regression_kfold.ipynb` |
| 6 | AdaBoost Regression | `07_adaboost_regression_kfold.ipynb` |
| 7 | LightGBM Regression | `08_lightgbm_regression_kfold.ipynb` |
| 8 | XGBoost Regression | `09_xgboost_regression_kfold.ipynb` |

> Note: An unscaled SVR notebook can be added later as `03_svr_kfold.ipynb` for comparison with the StandardScaler version.

---

## Datasets

| Dataset | Purpose |
|---|---|
| `Salary_Data.csv` | Simple Linear Regression |
| `50_Startups.csv` | Multiple Linear Regression |
| `insurance_pre.csv` | SVR, Decision Tree, Random Forest, AdaBoost, LightGBM and XGBoost |

The datasets are stored in the `data/` folder.

---

## Repository Structure

```text
regression-models-kfold-cross-validation/
│
├── data/
│   ├── Salary_Data.csv
│   ├── 50_Startups.csv
│   └── insurance_pre.csv
│
├── notebooks/
│   ├── 01_simple_linear_regression_kfold.ipynb
│   ├── 02_multiple_linear_regression_kfold.ipynb
│   ├── 04_svr_standardscaler_kfold.ipynb
│   ├── 05_decision_tree_regression_kfold.ipynb
│   ├── 06_random_forest_regression_kfold.ipynb
│   ├── 07_adaboost_regression_kfold.ipynb
│   ├── 08_lightgbm_regression_kfold.ipynb
│   └── 09_xgboost_regression_kfold.ipynb
│
└── README.md
