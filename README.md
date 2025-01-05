# **Gold Price Prediction using Random Forest Regression**

## 📄 **Overview**
This project involves predicting gold prices using a **Random Forest Regression** model. The dataset contains historical financial data, including gold prices, stock market indices, and currency exchange rates. The primary objective is to build a predictive system with high accuracy.

---

## 🛠️ **Workflow**

### 1. **Data Preprocessing**
- Loaded the dataset (`gld_price_data.csv`) and analyzed its structure.
- Checked for missing values (none were found).
- The dataset includes **2290 samples** with **6 columns**:
  - **Date**
  - **SPX** (S&P 500 Index)
  - **GLD** (Gold ETF price - Target variable)
  - **USO** (Crude Oil price)
  - **SLV** (Silver price)
  - **EUR/USD** (Currency exchange rate).

### 2. **Exploratory Data Analysis**
- Generated statistical summaries using `.describe()`.
- Calculated correlation between features and visualized it using a **heatmap**:
  - **GLD** has the highest correlation with **SLV (Silver Price)**: `0.87`.
  - Weak correlations with **SPX**, **USO**, and **EUR/USD**.

### 3. **Feature Engineering**
- Dropped the **Date** column as it is not relevant for modeling.
- Separated the dataset into:
  - **Features (`X`)**: All columns except `GLD`.
  - **Target (`y`)**: The `GLD` column (Gold price).
- Split the dataset into:
  - **Training set**: 80%
  - **Testing set**: 20%.

### 4. **Model Training**
- Trained a **Random Forest Regressor** model using `scikit-learn`.
- **Achieved:**
  - **R² Score (Test Set):** **0.989**

### 5. **Prediction System**
- Built a prediction pipeline to forecast gold prices.
- Visualized the relationship between **actual vs predicted values** using a scatter plot.

---

## 🧰 **Technologies Used**
- **Programming Language:** Python
- **Key Libraries:**
  - `pandas` for data manipulation.
  - `numpy` for numerical computations.
  - `matplotlib` and `seaborn` for data visualization.
  - `scikit-learn` for model training and evaluation.

---

## 📊 **Results**
- **R² Score (Test Set):** **0.989**
- Scatter plot confirms strong alignment between actual and predicted values.

---

## 🔍 **Key Insights**
- **SLV (Silver Price)** has the strongest positive correlation with **GLD (Gold Price)**.
- Random Forest Regression is highly effective for predicting gold prices, achieving excellent performance with minimal error.
- The predictive model can be extended to include real-time financial data for forecasting.

---

## 📁 **Project Files**
- 📂 **pdf:**- https://github.com/Parththapliyal/Gold-Price-Prediction/blob/main/gold.pdf
- 📂 **Jupyter Notebook:**-https://github.com/Parththapliyal/Gold-Price-Prediction/blob/main/gold%20price%20prediction%20random%20forest%20regression.ipynb 

