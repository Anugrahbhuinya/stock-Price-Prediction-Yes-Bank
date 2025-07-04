# 📈 Yes Bank Stock Price Prediction

A full-cycle machine learning project to predict the closing prices of Yes Bank stock using data analysis, feature engineering, regression models, and hypothesis testing.

---

## 📂 Project Structure

- ✅ Data Cleaning using **Pandas** & **Excel**
- ✅ Visual EDA with **Matplotlib** & **Seaborn**
- ✅ SQL-based validation
- ✅ Feature Engineering
- ✅ Linear & Ridge Regression Modeling
- ✅ Hyperparameter Tuning with **GridSearchCV**
- ✅ Evaluation using MAE, RMSE, R²
- ✅ Hypothesis Testing (ANOVA, T-Test)

---

## 📊 Dataset

- File: `data_YesBank_StockPrices.csv`
- Contains historical OHLC data with dates
- Columns: `Date`, `Open`, `High`, `Low`, `Close`, `Volume`

---

## 🔍 Exploratory Data Analysis (EDA)

- 📈 Line Plot: Trends in closing price
- 📊 Histogram: Distribution of stock prices
- 📦 Box Plot: Outlier detection
- 📌 Heatmap: Correlation between numerical variables
- 📅 Monthly Aggregation: Avg. monthly closing prices

> 📌 Insight: Strong correlation among price-based columns; evidence of seasonality and volatility over time.

---

## 🧠 Feature Engineering

- `Volatility = High - Low`
- `3-Month Moving Average` of closing price
- Extracted time features: Year, Month

---

## 🧪 Hypothesis Testing

### 1. ANOVA Test (Monthly Price Difference)
- **H₀**: No difference in monthly average prices
- **Result**: p < 0.05 → ✅ Reject H₀ → Price varies significantly across months

### 2. T-Test (2020 vs 2021)
- **H₀**: No difference in yearly average prices
- **Result**: p < 0.05 → ✅ Significant difference observed

> 🧬 Significance: Validates EDA patterns with statistical proof, supporting seasonal modeling.

---

## 🤖 Modeling

### ✅ Linear Regression
- Simple, interpretable baseline
- High R² but risk of overfitting due to multicollinearity

### ✅ Ridge Regression
- Used L2 regularization
- **Hyperparameter tuning** using GridSearchCV
- Best model selected via 5-fold CV

---

## 📊 Model Evaluation

| Model              | MAE   | RMSE  | R² Score |
|-------------------|--------|--------|----------|
| Linear Regression | ~3.1  | ~4.2  | 0.99     |
| Ridge Regression  | ~2.8  | ~4.0  | 0.99 ✅  |

> 🎯 Ridge regression offered improved generalization and reduced error.

---

## 🧪 Tools & Libraries Used

- **Python 3.10+**
- **Pandas**, **NumPy**
- **Matplotlib**, **Seaborn**
- **Scikit-learn**
- **SciPy** (for ANOVA, T-Test)
- **SQL / Excel** for additional insights

---

## 📌 Key Insights

- Closing prices show monthly volatility and trend shifts
- Ridge Regression is ideal for stable prediction
- ANOVA and T-Test confirm seasonal and yearly differences

---


## 🙏 Acknowledgments

- Yes Bank dataset (public)
- scikit-learn documentation
- Inspiration from real-world financial modeling use-cases

---

## 📧 Contact

**Anugrah Bhuinya**  
  


