# 📊 Customer Churn Prediction

## 🔍 Overview

Customer churn is a major challenge for businesses, especially in digital platforms and subscription-based services. This project focuses on predicting customer churn risk using data analysis and machine learning techniques.

The project not only builds a predictive model but also extracts **actionable business insights** from customer behavior.

---

## 🎯 Problem Statement

Identify customers who are likely to churn based on their behavior, activity patterns, and transaction history.

---

## 📁 Project Structure

```
Customer-Churn-Prediction/
│
├── Customer_churn_prediction_project.ipynb   # Complete ML workflow
├── README.md                                # Project documentation
```

---

## 📊 Dataset Description

The dataset contains customer-related features such as:

* Age
* Days since last login
* Average time spent
* Average transaction value
* Points in wallet
* Login frequency
* Customer activity metrics

**Target Variable:**

* `churn_risk_score` → Indicates likelihood of customer churn

---

## 🧠 Project Workflow

### 1️⃣ Data Loading

* Dataset loaded using Pandas
* Initial inspection using `.head()`, `.info()`, `.describe()`

---

### 2️⃣ Data Cleaning & Preprocessing

#### ✅ Handling Missing Values

* Replaced `"?"` and `"Error"` with `NaN`
* Replaced anomalous values like `-999`
* Used:

  * **Mean imputation** (for normal distributions)
  * **Mode imputation** (for features with outliers)

#### ✅ Null Value Strategy

* Calculated percentage of missing values
* Rule used:

  * If >50% → drop (none found)
  * If <50% → impute

---

### 3️⃣ Feature Engineering

* Split features into:

  * **Numerical features**
  * **Categorical features**

* Converted data types where required

* Cleaned invalid values (e.g., negative frequencies)

---

### 4️⃣ Exploratory Data Analysis (EDA)

#### 📌 Key Analyses Performed:

* Null value heatmap visualization
* Distribution plots (before & after imputation)
* Feature vs churn relationships

#### 🔍 Key Insights:

* Most customers are aged **35–40**
* High churn risk observed around:

  * **~13–14 days login gap**
  * **Transaction values around 10K**
* Average usage time is concentrated in lower ranges

---

### 5️⃣ Data Visualization

* Used:

  * **Matplotlib**
  * **Seaborn**
* Created:

  * Histograms
  * Heatmaps
  * Distribution comparisons
  * Feature vs churn plots

---

### 6️⃣ Data Imputation Strategy (Important Highlight)

A custom visualization function was created to compare:

* Before handling missing values
* After handling missing values

This shows **good understanding of data impact**, which is a strong point for interviews.

---

## 📈 Business Insights

* Customers who log in less frequently are more likely to churn
* Engagement drops significantly after ~2 weeks
* Mid-range transaction users show higher churn risk
* Platform optimization should focus on:

  * Increasing login frequency
  * Improving user engagement cycles

---

## ⚙️ Tech Stack

* Python 🐍
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn

---

## ▶️ How to Run

### 1️⃣ Clone the repository

```bash
git clone https://github.com/dileepkumar2626/Customer-Churn-Prediction.git
cd Customer-Churn-Prediction
```

### 2️⃣ Install dependencies

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

### 3️⃣ Run the notebook

```bash
jupyter notebook
```

Open:

```
Customer_churn_prediction_project.ipynb
```

---

## 🚀 Key Strengths of This Project

* Strong **EDA-driven approach**
* Real-world **data cleaning handling (errors, anomalies)**
* Logical **missing value strategy**
* Insight-driven analysis (not just modeling)

---

## 🔮 Future Improvements

* Add machine learning models (if not fully implemented)
* Hyperparameter tuning
* Feature importance analysis
* Model deployment (Flask / Streamlit)
* Real-time churn prediction system

---

## 👤 Author

**Dileep Kumar**
GitHub: https://github.com/dileepkumar2626

---

## ⭐ If you found this project useful, give it a star!
