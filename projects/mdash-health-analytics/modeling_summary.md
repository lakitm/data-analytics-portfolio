# MDASH Modeling Summary

## Objective

Build a short-term forecasting workflow for weekly dengue incidence using historical case counts and climate-related predictors.

## Data Structure

The modeling workflow used weekly aggregated dengue case counts aligned with weekly climate indicators.

Core variables:

| Variable | Description |
|---|---|
| `date` | Weekly date index |
| `cases` | Weekly dengue case count |
| `avg_temperature_c` | Weekly average temperature |
| `avg_humidity_percent` | Weekly average humidity |
| `total_rainfall_mm` | Weekly total rainfall |

Lagged predictors were generated for the previous four weeks.

## Modeling Steps

1. Load dengue and weather datasets.
2. Convert onset dates and weather dates to datetime.
3. Aggregate dengue records into weekly case counts.
4. Merge weekly cases with weather variables.
5. Generate lagged features for climate variables and dengue counts.
6. Standardize predictors.
7. Train and compare candidate models.
8. Evaluate using offline holdout and rolling validation.
9. Select the model with strongest rolling RMSE.
10. Convert forecasts into dashboard-ready threshold statuses.

## Why This Matters for Analytics Roles

This project demonstrates:

- time-series feature engineering;
- model comparison across statistical, machine learning, and deep learning approaches;
- practical model evaluation for deployment;
- translation of technical outputs into decision-support indicators;
- responsible handling of sensitive data.
