
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
  - `experience` (numerical)
  - `education` (categorical)
  - `job_title` (categorical)
  - `location` (categorical)
  - `gender` (categorical)
  - `salary` (target variable, numerical)

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

```python
sample_input = {
    'age': 25,
    'workclass': 'Private',
    'fnlwgt': 226802, # Added fnlwgt
    'educational-num': 13,
    'marital-status':'Married-civ-spouse',
    'occupation':'Exec-managerial',
    'relationship':'Husband',
    'race':'White',
    'gender':'Male',
    'capital-gain': 0,
    'capital-loss': 0,
    'hours-per-week': 40,
    'native-country': 'United-States'
}

# Predicted Output
Predicted Salary: <50 USD$
