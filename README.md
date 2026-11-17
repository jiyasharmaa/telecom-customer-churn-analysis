# 📉 Customer Churn Exploratory Data Analysis (EDA)

An end-to-end Exploratory Data Analysis (EDA) project examining customer churn behavior in the telecommunications industry using Python. This project cleans raw customer records and uses data visualization libraries to identify critical behavioral and service-related factors driving customer attrition.

---

## 📊 Dataset Overview
* **Source:** Telco Customer Churn Dataset
* **Size:** 7,043 rows × 21 columns
* **Target Variable:** `Churn` (Yes/No indicating whether the customer left within the last month)

---

## 🧹 Data Cleaning & Preprocessing
Before diving into analysis, the dataset underwent standard preprocessing using **Pandas**:
* **Handling Missing Values:** Identified and converted blank strings in the `TotalCharges` column (associated with new customers having a tenure of 0) into numerical `0.0` and cast the column to `float`.
* **Data Integrity Checks:** Verified that `customerID` values were entirely unique with no duplicate records.
* **Feature Transformation:** Converted binary numeric codes in `SeniorCitizen` (`0` and `1`) into categorical labels (`no` and `yes`) for intuitive chart interpretation.

---

## 🔍 Key Exploratory Insights & Findings

1. **Overall Churn Rate:** 
   * Approximately **26.54%** of total customers have churned, indicating a notable retention challenge.
2. **Tenure & Loyalty:** 
   * Customer lifespan is a strong predictor of retention; customers in their first 1–2 months exhibit the highest churn rates, whereas long-tenure customers tend to stay loyal.
3. **Contract Type Impact:** 
   * **Month-to-month contracts** suffer from significantly higher churn compared to long-term commitments (One-year and Two-year contracts).
4. **Internet Service & Add-ons:** 
   * Customers using **Fiber optic internet** show higher churn rates than those using DSL. Furthermore, customers lacking auxiliary services like Online Security, Online Backup, and Tech Support are far more likely to leave.
5. **Payment Method:** 
   * Customers paying via **Electronic check** experience the highest rate of churn compared to automated bank transfers, credit cards, or mailed checks.

---

## 🛠️ Tech Stack & Libraries Used
* **Python:** Core programming language
* **Pandas & NumPy:** Data cleaning, transformation, and manipulation
* **Matplotlib & Seaborn:** Statistical data visualization (countplots, histograms, pie charts, and grouped analysis)

---

## 📂 Repository Structure
```text
├── Customer Churn.csv          # Raw dataset
├── Churn_Analysis.ipynb        # Jupyter Notebook containing full EDA workflow
└── README.md                   # Project documentation
