In this project,

assume the role of a data scientist tasked with assisting a US-based housing company, Surprise Housing,
as it embarks on expanding into the Australian real estate market. Your primary objective is to develop a machine learning model
that accurately predicts the actual value of potential properties, enabling the company to make informed investment choices.
Project Objective: Create a robust machine learning model capable of forecasting house prices in the Australian real estate market.
This predictive tool will serve as a vital asset for Surprise Housing, aiding them in identifying prospective properties
for acquisition. Furthermore, it aims to unveil the significance of variables that influence house prices andhow these variables collectively describe the price of a house.




🧠 Project Overview
Objective: Predict the selling price (SalePrice) of residential homes using machine learning regression models.

Dataset: Train and test CSV files with 80+ features related to house conditions, construction, location, etc.

Goal: Analyze housing data, clean it, engineer features, build models, tune them, and accurately predict price.

## ⚙️ Technical Workflow
# 1. Data Preprocessing
Handled missing values:

- Used mean/median/mode to fill nulls

- Dropped columns with too many nulls

- Converted text-based numbers like "109 min" → 109

- Encoded categorical variables using Label Encoding and OneHotEncoding

- Scaled data using StandardScaler

## 2. Feature Engineering
- Separated numerical and categorical columns

- Removed skewness using PowerTransformer (Yeo-Johnson)

- Used SelectFromModel for dimensionality reduction

## 3. Modeling
Used various regression algorithms:

- Linear Regression

- Decision Tree Regressor

- Random Forest Regressor

- Gradient Boosting Regressor

- AdaBoost Regressor

- XGBoost

- SVR

## 4. Hyperparameter Tuning
Used RandomizedSearchCV to tune:

- n_estimators, max_depth, min_samples_split

- learning_rate, max_features, subsample

- Tuning done after feature selection to improve performance

## 5. Model Evaluation
Metrics used:

- R² Score

- Mean Absolute Error (MAE)

- Root Mean Squared Error (RMSE)

- Best models: GradientBoostingRegressor and RandomForestRegressor

-  Saved model using pickle


## 🧰 Tools & Libraries
- Python

- Pandas, NumPy, Matplotlib, Seaborn

- Scikit-learn, XGBoost


## ✅ Results
Achieved high accuracy (R² ~ 0.92 in training)

