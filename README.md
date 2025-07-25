# 📊 Loan Amount Prediction using Linear Regression

This project predicts the loan amount sanctioned to users using **Linear Regression** on historical loan application data. It covers data preprocessing, exploratory data analysis (EDA), model training using Scikit-learn, and evaluation using standard metrics.

---

## 🧠 Objective

- Build a Linear Regression model to predict loan amount.
- Perform data cleaning, encoding, scaling.
- Visualize trends and correlations.
- Evaluate model performance statistically and graphically.

---

## 🛠️ Libraries Used

- `pandas` – data loading and preprocessing
- `numpy` – numerical operations
- `matplotlib`, `seaborn` – visualizations
- `scikit-learn` – ML models and evaluation metrics

---

## 📁 Dataset

- **Source**: `train.csv` located in Google Drive
- **Steps Taken**:
  - Removed columns: `Customer ID`, `Name`, `Property ID`
  - Dropped rows with missing values
  - Encoded categorical variables using one-hot encoding
  - Scaled numerical features using `StandardScaler`

---

## 📊 Exploratory Data Analysis (EDA)

- **Loan Amount Distribution**:
  Visualized with histogram and KDE

- **Correlation Heatmap**:
  Shows relationship between numerical features

---

## ⚙️ Model Building

Steps followed:

1. Train-test split (80/20)
2. Model: `LinearRegression()` from scikit-learn
3. Fit the model on training data
4. Predict on test data

### 🔍 Evaluation Metrics

| Metric       | Value            |
|--------------|------------------|
| MAE          | 25,323.79        |
| MSE          | 1,195,267,145.51 |
| RMSE         | 34,572.63        |
| R² Score     | 0.4751           |
| Adjusted R²  | 0.4737           |

---

## 📌 Visualizations

- **Actual vs Predicted** Scatter Plot
- **Residual Plot**
- **Feature Coefficients** Bar Chart

---

## 📚 Theoretical Background

The Linear Regression model assumes a relationship of the form:

y = β₀ + β₁x₁ + β₂x₂ + ... + βₙxₙ + ε


Where:
- `y` = Loan amount (target)
- `xᵢ` = Feature variables (income, credit score, etc.)
- `βᵢ` = Model coefficients
- `ε` = Error term (residual)

---

## 🏁 Conclusion

The model provides a moderate R² score (~47%), indicating potential for improvement. Advanced models or better feature engineering could enhance performance.

---
