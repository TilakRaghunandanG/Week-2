⚡ Electric Vehicle Price Prediction — Summary

This project predicts the price range of electric vehicles (EVs) using machine learning, specifically a Random Forest Regressor.

🔹 Key Steps

Data Preparation

Loaded data from cars_data_RAW.csv

Removed duplicates, filled missing values, and cleaned numeric columns (removed units like km/h, sec, etc.)

Encoded categorical variables for model use.

Feature Engineering

Target variable: price-range

Split dataset: 80% training, 20% testing

Standardized numeric features using StandardScaler.

Model Training

Model: RandomForestRegressor(n_estimators=100, random_state=42)

Input features: battery capacity, acceleration, top speed, efficiency, range, etc.

Output: predicted EV price range.

Model Evaluation

R² Score: 0.87 → Model explains 87% of price variation (very good)

MAE: ≈ 1200

RMSE: ≈ 1895

Model Saving

Saved trained model and scaler in the models/ directory as:

ev_price_model.pkl

scaler.pkl
