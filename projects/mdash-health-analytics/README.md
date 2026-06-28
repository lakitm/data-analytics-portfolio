# MDASH: Health Analytics & Dengue Forecasting Dashboard

## Overview

MDASH, or Malolos Disease Analytics and Surveillance Hub, is a health analytics dashboard designed to support dengue surveillance, short-term forecasting, localized public health awareness, and decision support.

The project combines epidemiological data preparation, climate-based feature engineering, forecasting model comparison, dashboard visualization, health facility mapping, and administrative controls. It was developed as a data-driven response to fragmented local health communication and the need for more interpretable surveillance outputs.

## Problem Framing

Dengue surveillance data can be difficult to interpret when records are fragmented, delayed, or not visualized at the community level. MDASH addresses this by presenting surveillance information through dashboard-ready outputs such as trend charts, forecasts, threshold alerts, and local health-resource references.

## My Contribution

My main contribution focused on the analytics and modeling layer:

- Prepared dengue and climate data for weekly time-series modeling.
- Built lagged features using dengue case counts, rainfall, temperature, and humidity.
- Compared statistical, machine learning, and deep learning forecasting approaches.
- Evaluated model performance using RMSE and rolling validation.
- Supported the selection of Random Forest as the deployment model based on forecasting performance.
- Helped translate model outputs into dashboard-ready indicators and threshold-based alerts.
- Supported data security awareness and backend administration workflows in Supabase.

## Methods Used

The modeling workflow compared the following forecasting approaches:

| Model | Purpose |
|---|---|
| Negative Binomial Regression | Count-data baseline for overdispersed dengue cases |
| XGBoost with Poisson Loss | Nonlinear count-based boosted model |
| Random Forest | Ensemble learning model for robust short-term prediction |
| CNN-LSTM | Deep learning approach for sequential pattern extraction |
| LSTM-XGBoost | Hybrid model combining temporal learning and residual boosting |

The final dashboard used a threshold-based early warning logic based on historical baseline trends.

## Result Summary

Under rolling evaluation, Random Forest achieved the lowest RMSE among the tested models and was selected for deployment in the dashboard logic.

| Model | Rolling RMSE |
|---|---:|
| Random Forest | 7.53 |
| LSTM-XGBoost | 7.59 |
| XGBoost-Poisson | 7.95 |
| CNN-LSTM | 8.66 |
| Negative Binomial Regression | 32.32 |

## Dashboard Capabilities

The system concept included:

- Barangay-level dengue trend visualization
- Short-term dengue forecasting
- Threshold-based alert mechanism
- Health facility mapping
- Emergency hotline access
- Public health advisories and awareness content
- Administrative controls for data, content, analytics, users, and settings

## Technical Stack

- Python
- Pandas, NumPy
- Scikit-learn
- XGBoost
- TensorFlow/Keras
- Statsmodels
- Next.js
- Supabase/PostgreSQL
- Cube.js
- Apache ECharts

## Portfolio Publishing Note

This repository does not include raw dengue records, institutional datasets, full private notebooks, credentials, service keys, or the complete unpublished thesis manuscript. Materials here are limited to a sanitized case study, synthetic schema, model summary, and high-level workflow documentation.
