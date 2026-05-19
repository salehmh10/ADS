[README (1).md](https://github.com/user-attachments/files/27978775/README.1.md)
# Loan Dataset - Machine Learning Assignment 2

This repository contains my second Applied Data Science homework.  
The project applies a full machine learning workflow on a loan dataset.

## Main Tasks

- **Regression:** predict `loan_amnt`
- **Binary Classification:** predict `loan_status`
- **Multiclass Classification:** predict `loan_intent`

## Files

```text
HW2.ipynb       # Main notebook
loan_data.csv   # Dataset
README.md       # Project summary
```

## Workflow

### 1. Data Cleaning and Preprocessing

- Loaded and inspected the dataset.
- Checked missing values, duplicates, and invalid values.
- Removed invalid or unrealistic records.
- Encoded categorical columns.
- Scaled features when needed.
- Used train/test split for model evaluation.

### 2. Exploratory Data Analysis

- Checked target distributions.
- Used histograms, boxplots, pairplots, and heatmaps.
- Studied relationships between loan, income, credit score, and target variables.
- Checked class imbalance and possible outliers.

### 3. Feature Engineering

Created new useful features such as:

- `loan_to_income_ratio`
- `interest_burden`
- `income_per_age`
- `credit_strength`
- `credit_start_age`
- `default_interest_interaction`
- high/low risk flag features

## Models Used

### Regression Models

- Linear Regression
- Ridge Regression
- LASSO Regression
- Kernel Regression
- Polynomial Ridge
- Elastic Net
- SVR
- Decision Tree Regressor
- XGBoost Regressor
- ExtraTrees Regressor

Main regression metric: **MAE**

### Binary Classification Models

- Logistic Regression
- Linear SVM
- Kernel SVM
- KNN
- Decision Tree
- Random Forest
- LDA

Main binary classification metric: **F1 Score**

### Multiclass Classification Models

- Multiclass SVM
- Logistic Regression OVR
- Multinomial Logistic Regression
- KNN with K tuning
- Decision Tree
- XGBoost
- LightGBM
- AdaBoost
- CatBoost
- Random Forest
- Kernel SVM with OVO

Main multiclass metric: **Macro F1**

## Hyperparameter Tuning

Several hyperparameters were tested using lists of values.

Examples:

- `K` in KNN
- `C` and `gamma` in SVM
- `max_depth` in Decision Trees
- `n_estimators` and `learning_rate` in boosting models
- `alpha` in Ridge and LASSO

Both train and test results were compared to check overfitting.

## Evaluation

The notebook reports different metrics depending on the task.

Regression:

- MAE
- MSE
- MAPE
- R² Score

Classification:

- Accuracy
- Precision
- Recall
- F1 Score
- ROC AUC
- Macro / Micro / Weighted F1
- Log Loss
- Confusion Matrix

## Explainability

The notebook includes simple model interpretation:

- Linear model coefficients
- Top 10 feature weights
- Tree-based feature importance
- Permutation importance
- Confusion matrix analysis

## Bonus Questions

The notebook also answers bonus theory questions about:

- Bias-variance trade-off
- L1 vs L2 regularization
- MAPE problems
- Outliers
- Class imbalance
- Decision boundaries
- KNN and Decision Trees
- Micro, Macro, and Weighted F1
- Multiclass vs Multilabel classification
- ROC vs PR curves

## Main Takeaways

- Data cleaning and feature engineering were important before modeling.
- Scaling helped linear and distance-based models.
- Tree-based models performed well on this tabular dataset.
- F1 Score and Macro F1 were better than accuracy for classification tasks.
- Feature importance helped explain model behavior.

## How to Run

1. Clone the repository.
2. Put `loan_data.csv` next to `HW2.ipynb`.
3. Install the required libraries.
4. Run the notebook from top to bottom.

```bash
pip install pandas numpy matplotlib seaborn scikit-learn xgboost lightgbm catboost
```
