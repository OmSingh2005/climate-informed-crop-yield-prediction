# climate-informed-crop-yield-prediction
Machine learning–based crop yield prediction using global climate data, with SHAP-based explainability and time-aware evaluation.

📌 Project Overview

This project explores machine learning approaches for predicting annual crop yield using publicly available global climate data.
Tree-based models (XGBoost, LightGBM) are evaluated under a strict temporal train–test split, and SHAP is used to interpret feature contributions.

📊 Dataset

FAOSTAT crop yield data (country-level)

NASA POWER climate variables

Crops: Wheat, Rice, Maize, Sugarcane

Time span: 2001–2023

Features include temperature, precipitation, radiation, humidity, and lagged yield

(No need to mention “103 countries” in README unless you want — CV will handle that)

🧠 Models

Linear Regression (baseline)

XGBoost

LightGBM

🔍 Explainability

SHAP summary plots

Feature dependence analysis

Interpretation of lagged yield and climate variables

🧪 Evaluation

Time-based split (no data leakage)

Metrics: RMSE, R²

Separate holdout year evaluation

⚠️ Notes

This repository focuses on modeling and interpretability rather than deployment or productionization.
