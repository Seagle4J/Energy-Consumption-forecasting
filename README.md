# Energy-Consumption-forecasting
Energy consumption forecasting plays a crucial role in efficient power generation, distribution, and demand-side management. Accurate prediction of energy usage helps utilities reduce operational costs, avoid energy wastage, and improve grid reliability.

This project focuses on forecasting total energy consumption using machine learning and ensemble learning techniques. The system leverages historical power consumption data and time-based feature engineering to predict future energy demand.

Project Objectives-

To analyze historical energy consumption data

To perform time-series feature engineering (lags, rolling averages, calendar features)

To build and compare multiple machine learning models

To improve prediction accuracy using ensemble learning techniques

To evaluate models using standard regression metrics

Dataset Description-

Source: Kaggle

File Used: powerconsumption.csv

Features:

Datetime

PowerConsumption_Zone1

PowerConsumption_Zone2

PowerConsumption_Zone3

Target Variable:

TotalConsumption (sum of all three zones)

Technologies Used-

Programming Language: Python

Development Environment: Google Colab / Jupyter Notebook

Libraries:

pandas, numpy

matplotlib

scikit-learn

xgboost

joblib

 Machine Learning Models Implemented-
 
1. Linear Regression

Baseline model

Captures linear relationships

Simple and fast

2. Random Forest Regressor

Ensemble of decision trees

Handles non-linear patterns

Reduces overfitting using bagging

3. XGBoost Regressor

Gradient boosting algorithm

Highly optimized and accurate

Performs exceptionally well on structured data

 Ensemble Learning Techniques-
🔹 Voting Ensemble

Combines predictions from:

Linear Regression

Random Forest

XGBoost

Final prediction is the average of individual predictions

🔹 Stacking Ensemble

Base Models: Linear Regression, Random Forest, XGBoost

Meta-Model: Random Forest Regressor

Learns how to optimally combine base model predictions

Achieves the highest accuracy in this project

 Feature Engineering-

Time-based features:

Hour, Day, Month, Weekday, Weekend indicator

Lag features:

Previous timestep

Hourly, Daily, Weekly lags

Rolling statistics:

Hourly rolling mean

Daily rolling mean

These features help the models capture temporal patterns and seasonality in energy usage.

📈 Model Evaluation Metrics

The models are evaluated using standard regression metrics:

MAE (Mean Absolute Error)

RMSE (Root Mean Square Error)

R² Score (Coefficient of Determination)

Additionally, a combined testing accuracy is computed using:

R²-based accuracy

MAE-based accuracy

RMSE-based accuracy

🚀 How to Run the Project

Upload the dataset to Google Colab

Run the preprocessing and feature engineering blocks

Train all models (LR, RF, XGBoost, Voting, Stacking)

Evaluate performance and generate plots

Run the testing code for unseen data

✅ Results & Conclusion

Ensemble models significantly outperform individual models

Stacking Ensemble achieves the best overall accuracy

XGBoost shows strong performance among individual models

Feature engineering plays a key role in improving prediction quality
