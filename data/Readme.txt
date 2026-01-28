Global Crop Yield Prediction (Explainable ML Project)

This project predicts yearly crop yields for different countries using machine learning and climate data.
The goal is not only to make accurate predictions, but also to explain why the model makes certain decisions.

This README is written in simple language so anyone can understand the project, even without technical background.

What This Project Does

Every year, countries grow major crops such as wheat, rice, maize, and sugarcane.
Their yield depends on many factors, including:

Temperature

Rainfall

Sunlight

Humidity

Previous year’s farming conditions

This project brings these factors together and uses machine learning to predict crop yield.
The model also tells us which factors influence the predictions the most, using SHAP (an explainability tool).

Where the Data Comes From

Two reliable global datasets are used:

1. FAOSTAT (Food and Agriculture Organization)

Provides official crop yield data for each country from 2001 to 2023.

2. NASA POWER

Provides yearly climate data (temperature, rainfall, radiation, humidity) for the same countries and years.

These datasets are merged into one combined dataset used for training the models.

How the Model Works (Simple Explanation)

Collect yield and climate data for each country and year.

Clean and prepare the dataset.

Train machine learning models such as XGBoost and LightGBM.

Split the data by year to avoid future leakage:

Train on earlier years

Test on later years

Use 2023 as a final holdout

Use SHAP to understand why the models make certain predictions.

This ensures the project is transparent and interpretable.

Key Findings

Yield from the previous year is one of the strongest predictors of the next year.

Climate factors like temperature, rainfall, and sunlight influence yield but vary across regions and crops.

Different crops and countries show different patterns, and the model learns these differences.

SHAP provides clear and understandable explanations for the model’s predictions.

Why This Project Matters

Crop yields are important for food supply, planning, and climate-related decision making.
Predicting yields with explainable models helps:

Researchers

Policy makers

Agriculture analysts

Students and educators

The project demonstrates how global datasets and explainable ML techniques can be combined effectively.

Technologies Used

Python

Pandas

NumPy

XGBoost

LightGBM

SHAP

Matplotlib / Seaborn
