# Machine Learning Regression Model - CW1

## Project Description
This project is part of a machine learning coursework challenge where the goal is to build the best regression model to predict the outcome variable in a given dataset. The dataset consists of tabular data with both numerical and categorical features.

The objective is to minimize generalization error (measured using R²) on an unseen test set.

---

## Project Structure

- **`notebooks/`**: Jupyter notebooks for exploratory data analysis (EDA) model selection, training , and evaluation.

- **`data/`**: Contains the dataset [CW1_train.csv, CW1_test.csv] (included in the repository).

- **`requirements.txt`**: List of required Python dependencies.

---

## Installation & Setup
**Clone the repository**:
```bash
git clone https://github.kcl.ac.uk/K21184729/MachineLearningCW1.git
cd MachineLearningCW1

**Install dependencies**:
pip install -r requirements.txt

**Run the full pipline**:
Run Notebook Directly

---

## Dataset Information accessed through google drive in the development of the project.
Train File: CW1_train.csv
Test File: CW1_test.csv
Features: Numerical & categorical attributes related to regression modeling.
Target Variable: outcome
Our model is trained to predict the outcome column as accurately as possible.

## Dveleopment of the pipieline was through colab google and later turned into python scripts.
Model Pipeline
The project follows a structured machine learning pipeline:

Data Preprocessing
Handle missing values (median imputation)
One-hot encode categorical variables
Feature selection using Mutual Information
Polynomial feature generation for better non-linearity

Model Training
Train three models: CatBoost, XGBoost, and LightGBM
Hyperparameter tuning using Optuna
Model stacking with an optimized blending approach

Model Evaluation
Compute R² score on training and validation data
Generate scatter plots, residual plots, and box plots
Compare actual vs. predicted values

Results & Performance
Best Model: Stacked ensemble (CatBoost + XGBoost + LightGBM)
Achieved R² Score: 0.4760 on validation data and R² Score: 0.5882 on training data
Feature Importance: Extracted using SHAP values

The model achieved strong generalization while reducing overfitting.

Author: [Maram Talib]
Module: Machine Learning - [King's College London]
Submission Date: [20/02/2025]
