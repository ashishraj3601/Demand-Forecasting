# 🏪 Inventory Demand Forecasting using Machine Learning

This project focuses on building a **demand forecasting model** for inventory management using multiple regression techniques, including **Linear Regression, Ridge, Lasso**, and **XGBoost Regressor**.  
The objective is to predict future demand based on historical sales and time-related features, helping businesses optimize stock levels and avoid over/under-stocking.

---

## 📘 Project Overview

Inventory demand forecasting is a critical task in supply chain and retail analytics.  
This notebook demonstrates the full process — from **data preprocessing** and **feature engineering** to **model training** and **evaluation**.

### 🔍 Key Steps:
1. **Data Preprocessing**
   - Date conversion and extraction of `year`, `month`, `day`, `day_of_week`
   - Creation of **cyclical time features** (`sin`, `cos`) for month and day of week  
   - Handling categorical and numerical variables

2. **Feature Engineering**
   - Added cyclic encodings for temporal features to capture seasonality  
   - Optional handling of holidays and weekends for demand spikes

3. **Model Building**
   - Linear Regression  
   - Ridge Regression  
   - Lasso Regression  
   - XGBoost Regressor

4. **Evaluation**
   - Compared models using **Training** and **Validation Errors**
   - Selected the best-performing model for forecasting

---

## 🧠 Models & Performance

| Model | Training Error | Validation Error |
|:------|----------------:|-----------------:|
| **Linear Regression** | 20.90 | 20.97 |
| **XGBoost Regressor** | **6.91** | **6.92** |
| **Lasso Regression** | 21.02 | 21.07 |
| **Ridge Regression** | 20.90 | 20.97 |

### 🏁 Key Insight
- **XGBoost Regressor** achieved the lowest error, effectively capturing non-linear and seasonal patterns.
- Linear, Ridge, and Lasso models performed similarly, suggesting limited linearity in the data.

---

## 📈 Results & Insights

- ✅ **Best Model:** XGBoost Regressor  
- ⚡ **Error Gap:** Minimal between training and validation → No overfitting  
- 📅 **Feature Impact:** Cyclic month and day-of-week encodings helped capture seasonality  
- 💡 **Next Steps:**  
  - Hyperparameter tuning for XGBoost  
  - Incorporate lag/rolling features  
  - Deploy model as an API or Power BI dashboard for business usage  

---

## 🧩 Technologies Used

- **Python 3.10+**
- **Pandas**, **NumPy** — Data processing  
- **Scikit-learn** — Regression models & evaluation  
- **XGBoost** — Gradient boosting model  
- **Matplotlib / Seaborn** — Visualization  
- **Jupyter Notebook** — Development environment  

---
