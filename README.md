# Machine Learning Regression Validation

This repository contains Python implementations of regression algorithms
evaluated using K-Fold Cross Validation.

The project demonstrates how different regression algorithms perform across
multiple validation folds, rather than relying on a single train-test split.

## Objectives

- Apply K-Fold Cross Validation to regression models.
- Compare model performance using R² scores.
- Evaluate performance consistency across folds.
- Visualise actual versus predicted values.
- Analyse residuals and feature importance.
- Prevent preprocessing leakage using pipelines.

## Regression Models

| No. | Model | Scaling Required | Main Visualisations |
|---|---|---|---|
| 1 | Simple Linear Regression | No | Fold R², actual vs predicted, residuals |
| 2 | Multiple Linear Regression | No | Fold R², coefficients, residuals |
| 3 | Support Vector Regression | Recommended | Fold R², actual vs predicted |
| 4 | SVR with StandardScaler | Yes | Fold R², actual vs predicted, residuals |
| 5 | Decision Tree Regression | No | Tree structure, feature importance |
| 6 | Random Forest Regression | No | Fold R², feature importance, one tree |
| 7 | AdaBoost Regression | No | Fold R², feature importance |
| 8 | LightGBM Regression | No | Fold R², feature importance by gain |
| 9 | XGBoost Regression | No | Fold R², feature importance, tree plot |

## Validation Method

K-Fold Cross Validation divides the dataset into K subsets. The model is
trained on K-1 subsets and validated on the remaining subset. This process is
repeated until every subset has been used for validation.

## Metrics

- R² score for each fold
- Mean R² score
- Standard deviation of R² scores
- Actual versus predicted values
- Residual analysis

## Repository Structure

```text
notebooks/kfold_regression/   Jupyter notebooks
data/                         Dataset files
results/figures/              Exported visualisations
results/model_comparison.csv  Summary of model results
