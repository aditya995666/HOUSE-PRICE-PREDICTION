In this project,

assume the role of a data scientist tasked with assisting a US-based housing company, Surprise Housing,
as it embarks on expanding into the Australian real estate market. Your primary objective is to develop a machine learning model
that accurately predicts the actual value of potential properties, enabling the company to make informed investment choices.
Project Objective: Create a robust machine learning model capable of forecasting house prices in the Australian real estate market.
This predictive tool will serve as a vital asset for Surprise Housing, aiding them in identifying prospective properties
for acquisition. Furthermore, it aims to unveil the significance of variables that influence house prices andhow these variables collectively describe the price of a house.




# 🎯 Slide 1: Title Slide

- House Price Prediction

# 🧠 Slide 2: Project Overview

- Objective: Predict the SalePrice of residential homes using regression.

- Dataset: Train and test CSV files with 80+ features like construction type, size, year, location.

- Goal: Clean, transform, model, tune, and deploy a machine learning solution.

# ⚙️ Slide 3: Data Preprocessing

Filled missing values using:

- Mean for continuous data

- Median for skewed numerical columns

- Mode for categorical values

- Dropped columns with excessive nulls

- Converted text-based numerics (e.g., "109 min" → 109)

- Applied Label Encoding & One-Hot Encoding

- Scaled features using MinMaxScaler

# 🧪 Slide 4: Feature Engineering

- Separated numerical and categorical columns

- Reduced skewness using:
- 
- LogtransForm
  
- PowerTransformer with 'yeo-johnson' method

- Converted object type columns into numerical values


# ✅ Slide 5: Feature Selection

- Applied SelectFromModel to retain important features

- Threshold set to 'median' feature importance

- Reduced dimensionality and improved model performance

- Feature selection was applied before tuning to enhance efficiency

# 🤖 Slide 6: Regression Models Used

- Linear Regression

- Decision Tree Regressor

- Random Forest Regressor

- Gradient Boosting Regressor

- AdaBoost Regressor

- XGBoost

- Support Vector Regressor (SVR)

# 🔧 Slide 7: Hyperparameter Tuning

- Used RandomizedSearchCV with 10-fold cross-validation

- Tuned key parameters like:

- n_estimators, max_depth, learning_rate

- min_samples_split, subsample, max_features

- Best performance achieved by GradientBoostingRegressor

# 📊 Slide 8: Model Evaluation

Used evaluation metrics:

- R² Score

- Mean Absolute Error (MAE)

- Root Mean Squared Error (RMSE)

- Gradient Boosting and Random Forest showed highest accuracy

- Final R² Score on training data: ~0.92

- Final model saved using Pickle


# 🧰 Slide 10: Tools & Libraries

- Language: Python

- Libraries: Pandas, NumPy, Scikit-learn, XGBoost, Matplotlib, Seaborn

- Environment: Jupyter Notebook, VS Code



