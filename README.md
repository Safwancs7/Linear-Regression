# 🏠 House Price Prediction using Linear Regression

## 📌 Project Overview
This project implements a **Linear Regression** model to predict house prices based on numerical property features.  
The model’s performance is evaluated using standard regression metrics and visualized through an **Actual vs Predicted** plot.

---

## 📂 Dataset
- **Dataset:** `Real_estate.csv`
- **Target Variable:** `Price`
- **Features Used:**
  - Garage_Size
  - Num_Bathrooms
  - Num_Bedrooms
  - Square_Feet
  - Year_Built

The `ID` column was removed since it has no predictive value.

---

## 📊 Exploratory Data Analysis (EDA)

### 🔹 Summary Statistics
Summary statistics were generated to understand the distribution, scale, and variation of each feature.

### 🔹 Correlation Analysis
A correlation heatmap was created to analyze relationships between features and house prices.

**Key Insights:**
- `Square_Feet` shows a strong positive correlation with `Price`.
- Bathrooms and garage size also contribute moderately to price prediction.

---

## 🧮 Linear Regression Model

### 🔹 Model Explanation
Linear Regression models the relationship between features and the target variable using the equation:

\[
y = m_1x_1 + m_2x_2 + m_3x_3 + \dots + b
\]

Where:
- \( y \) = predicted house price  
- \( x \) = input features  
- \( m \) = coefficients  
- \( b \) = intercept  

The dataset was split into:
- **80% training data**
- **20% testing data**

---

## 📈 Model Evaluation

The model was evaluated using the following metrics:

- **MAE (Mean Absolute Error):** Average absolute difference between actual and predicted prices.
- **MSE (Mean Squared Error):** Penalizes larger errors more heavily.
- **RMSE (Root Mean Squared Error):** Error magnitude in the same unit as house prices.
- **R² Score:** Measures how well the model explains variance in house prices.

---

## 📉 Actual vs Predicted Analysis

An **Actual vs Predicted** scatter plot was used to visually assess model performance.

**Interpretation:**
- Most data points lie close to the reference line.
- This indicates that the model predicts house prices reasonably well.
- Deviations from the line represent prediction errors, which are expected.

---

## 📄 Prediction Output
A CSV file was generated containing actual and predicted values:

- **File:** `actual_vs_predicted_prices.csv`
- **Columns:**
  - `Actual`
  - `Predicted`

---

