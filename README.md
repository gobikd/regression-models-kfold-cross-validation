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
---

# Validation Method

This project evaluates regression models using **10-Fold Cross Validation**, which provides a more reliable estimate of model performance than a single train-test split.

The dataset is divided into ten equal folds.

For each iteration:

1. One fold is used as the validation dataset.
2. The remaining nine folds are used for training.
3. The model is trained.
4. The model is evaluated.
5. The process repeats until every fold has been used for validation once.

The final model performance is calculated using the average of all ten validation scores.

---

# Performance Metrics

The following evaluation metrics are demonstrated throughout the notebooks.

- R² Score
- Mean R² Score
- Standard Deviation
- Actual vs Predicted Values
- Residual Analysis

These metrics help evaluate both prediction accuracy and model stability.

---

# Model Visualisations

Each notebook contains visualisations that help interpret model performance.

Depending on the algorithm, the visualisations include:

- K-Fold R² Score
- Actual vs Predicted Plot
- Residual Plot
- Feature Importance
- Decision Tree Visualisation
- Random Forest Individual Tree
- AdaBoost Feature Importance
- LightGBM Feature Importance
- XGBoost Feature Importance

---

# Data Leakage Prevention

For Support Vector Regression, data preprocessing is performed using **StandardScaler**.

To avoid data leakage during K-Fold Cross Validation, scaling is performed only on the training folds.

This ensures the validation fold remains completely unseen during training.

---

# Repository Features

This repository demonstrates:

- Structured project organisation
- Relative dataset paths
- Multiple regression algorithms
- K-Fold Cross Validation
- Feature importance analysis
- Residual analysis
- Reproducible notebooks
- GitHub version control

---

# Technologies Used

- Python
- NumPy
- Pandas
- Matplotlib
- Scikit-learn
- XGBoost
- LightGBM
- Graphviz
- Jupyter Notebook
- GitHub

---

# Installation

Clone the repository

```bash
git clone https://github.com/gobikd/regression-models-kfold-cross-validation.git
```

Move into the project directory

```bash
cd regression-models-kfold-cross-validation
```

Install required packages

```bash
pip install numpy pandas matplotlib scikit-learn lightgbm xgboost graphviz
```

Open Jupyter Notebook

```bash
jupyter notebook
```

Open any notebook inside the **notebooks** folder.

---

# Learning Outcomes

This project demonstrates the practical implementation of:

- Linear Regression
- Multiple Linear Regression
- Support Vector Regression
- Decision Tree Regression
- Random Forest Regression
- AdaBoost Regression
- LightGBM Regression
- XGBoost Regression
- K-Fold Cross Validation
- Machine Learning Model Evaluation

---

# Future Improvements

Future enhancements include:

- Hyperparameter Tuning
- GridSearchCV
- RandomizedSearchCV
- MAE, RMSE and MSE comparison
- SHAP Explainability
- Model Deployment using Pickle
- Streamlit Web Application
- Docker Deployment
- CI/CD using GitHub Actions

---

# About Me

**GK**

Biomedical Engineer | Machine Learning Enthusiast | Artificial Intelligence Researcher

Currently learning:

- Python
- Machine Learning
- Deep Learning
- Natural Language Processing
- AI Agents

Research Interests:

- ECG Signal Processing
- Cardiovascular Disease Prediction
- Explainable AI
- Medical Artificial Intelligence

---

# Acknowledgement

This project was developed as part of my learning journey with **Hope AI**.

Special thanks to the Hope AI instructors and community for providing practical machine learning guidance and real-world implementation examples.

---

# License

This repository is intended for educational purposes.

Feel free to fork the project, learn from it, and suggest improvements.
