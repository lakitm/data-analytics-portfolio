# Dirty Housing Data: Cleaning & Linear Regression Workflow

## Overview

This project demonstrates an end-to-end machine learning workflow for a messy housing-price dataset. It focuses on practical data preparation, preprocessing, regression modeling, and evaluation.

Rather than presenting a polished dataset only, this project highlights a common analytics scenario: starting with inconsistent, incomplete, and mixed-type data, then building a clean modeling pipeline.

## Workflow

1. Inspect dataset shape, columns, summary statistics, and data types.
2. Identify missing values, duplicate rows, and inconsistent placeholders.
3. Standardize column names.
4. Replace invalid placeholder values with proper missing values.
5. Remove duplicate rows.
6. Detect or define the target column.
7. Clean numeric target values with symbols or commas.
8. Split features and target.
9. Convert numeric-looking text columns into numeric values.
10. Apply preprocessing:
    - median imputation for numeric columns;
    - most-frequent imputation for categorical columns;
    - one-hot encoding for categorical features.
11. Train a Linear Regression model.
12. Evaluate using MAE, MSE, and R².
13. Visualize actual vs. predicted values and residual distribution.

## Skills Demonstrated

- Data cleaning with Pandas
- Handling missing and inconsistent values
- Feature preparation for mixed numeric/categorical data
- Scikit-learn pipelines
- Regression modeling
- Model evaluation and visualization
- Clear technical interpretation for non-technical audiences

## Portfolio Positioning

This project is useful for entry-level data analyst, risk analyst, inventory analyst, compliance analyst, and junior data scientist roles because it demonstrates practical cleaning and modeling discipline. Many real datasets are not clean; this project shows the process of making them usable.
