# London Urban Mobility Demand Predictor

📌 **Project Objective:** Build a high-accuracy supervised machine learning pipeline to forecast hourly smart-bike rental demand in London to assist city operations with fleet rebalancing logistics.

## 📈 Model Performance Summary
- **R-squared (R²) Score:** 0.9564 (The model explains 95.6% of demand variances)
- **Mean Absolute Error (MAE):** 123.12 bikes 
- **Root Mean Squared Error (RMSE):** 228.60 bikes

## ⚙️ The Feature Engineering Edge
Rather than utilizing basic out-of-the-box attributes, I engineered a highly targeted domain feature: `is_rush_hour` (isolating non-holiday weekday windows between 7-9 AM and 4-6 PM). 

Upon model training via a **Random Forest Regressor**, feature importance evaluation proved that this custom engineered attribute was the premier driver of model intelligence, capturing **43.17%** of total feature weight.

## 📊 Repository Structure
- `notebooks/`: Contains the complete data inspection, cleaning, and model pipeline notebook.
- `visualizations/`: Contains saved evaluation graphs (`temperature_vs_rentals.png` and `feature_importances.png`).