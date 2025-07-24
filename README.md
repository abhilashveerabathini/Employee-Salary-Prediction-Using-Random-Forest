
---

## 🎯 Problem Statement

Accurately predicting salaries based on employee profiles is crucial for HR planning, recruitment, and market analysis. Manual estimation methods are inconsistent and lack data-driven insights. This project builds a machine learning model to predict salary with high accuracy using structured employee data.

---

## 🛠️ Technologies & Libraries Used

- **Python** (Google Colab)
- **pandas**, **numpy** — data manipulation
- **scikit-learn** — machine learning models
- **matplotlib**, **seaborn** — data visualization
- **LabelEncoder** — for encoding categorical features
- **RandomForestRegressor** — main prediction algorithm
- **XGBoost, GradientBoosting, KNN, LinearRegression** — for model comparison

---

## 📊 Dataset Overview

- File: `adult3.csv`
- Features:
  - age: Numerical
  - workclass: Categorical
  - fnlwgt: Numerical
  - educational-num: Numerical
  - marital-status: Categorical
  - occupation: Categorical
  - relationship: Categorical
  - race: Categorical
  - gender: Categorical
  - capital-gain: Numerical
  - capital-loss: Numerical
  - hours-per-week: Numerical
  - native-country: Categorical

---

## 🔍 Approach

1. **Load and explore** the dataset
2. **Preprocess** data: handle missing values, encode categorical features
3. **Split** data into training and testing sets
4. **Train models**, starting with Random Forest and compare with others
5. **Evaluate** using R² Score, MAE, and RMSE
6. **Visualize** model performance and feature importance
7. **Predict** salary for new employee profiles

---

## 📈 Model Comparison Results

| Model              | R² Score |
|--------------------|----------|
| Linear Regression  | 0.72     |
| KNN Regressor      | 0.81     |
| Gradient Boosting  | 0.86     |
| **Random Forest**  | **0.87** |
| XGBoost            | 0.88     |

> ✅ **Random Forest** gave one of the best performances in terms of accuracy and generalization.

---

## 💡 Sample Prediction

Features:
  - age: Numerical
  - workclass: Categorical
  - fnlwgt: Numerical
  - educational-num: Numerical
  - marital-status: Categorical
  - occupation: Categorical
  - relationship: Categorical
  - race: Categorical
  - gender: Categorical
  - capital-gain: Numerical
  - capital-loss: Numerical
  - hours-per-week: Numerical
  - native-country: Categorical

Target:
  - income: Categorical (e.g., <=50K, >50K)

