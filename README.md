# 📊 Customer Churn Analysis using Python

## 📌 Project Overview

Customer retention is one of the most important challenges faced by telecommunication companies. Acquiring new customers is often more expensive than retaining existing ones, making churn prediction and analysis a critical business objective.

This project analyzes the IBM Telco Customer Churn Dataset to identify the factors influencing customer attrition. The analysis includes data cleaning, exploratory data analysis (EDA), feature engineering, and statistical hypothesis testing to uncover actionable business insights.

---

## 🎯 Objectives

- Assess and improve dataset quality
- Perform Exploratory Data Analysis (EDA)
- Identify key factors influencing customer churn
- Create meaningful features for enhanced analysis
- Validate business assumptions using statistical testing
- Generate actionable recommendations for customer retention

---

## 📂 Dataset Information

**Dataset:** IBM Telco Customer Churn Dataset

| Attribute | Value |
|------------|--------|
| Records | 7,043 Customers |
| Features | 21 Variables |
| Target Variable | Churn |
| Dataset Type | Classification |
| Industry | Telecommunications |

### Key Variables

- Gender
- SeniorCitizen
- Partner
- Dependents
- Tenure
- InternetService
- Contract
- PaymentMethod
- MonthlyCharges
- TotalCharges
- Churn (Target Variable)

---

## 🛠 Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scipy
- Jupyter Notebook

---

## 📈 Exploratory Data Analysis (EDA)

The following analyses were performed:

### Customer Churn Distribution
- Churn Rate: **26.54%**
- Retention Rate: **73.46%**

### Contract Type vs Churn
- Month-to-Month customers exhibit the highest churn rates.
- Two-Year contract customers show the strongest retention.

### Monthly Charges vs Churn
- Customers with higher monthly charges are more likely to churn.

### Customer Tenure vs Churn
- Customers with shorter tenure periods are more likely to leave.

### Internet Service vs Churn
- Fiber Optic customers experience higher churn compared to DSL customers.

---

## 🧹 Data Cleaning

### Missing Values

After converting `TotalCharges` to numeric format:

- Missing Values Found: **11**
- Missing Values Removed: **11**
- Remaining Missing Values: **0**

### Duplicate Records

- Duplicate Records Found: **0**
- Duplicate Records Removed: **0**

### Data Type Corrections

- Converted `TotalCharges` from Object to Numeric format.

---

## ⚙️ Feature Engineering

Several new features were created to improve analysis and future predictive modeling.

### Tenure Group

| Tenure (Months) | Category |
|---------------|----------|
| 0–12 | New |
| 13–24 | Short-Term |
| 25–48 | Medium-Term |
| 49–72 | Long-Term |

### Charge Category

| Monthly Charges | Category |
|----------------|----------|
| Below $35 | Low |
| $35–$70 | Medium |
| Above $70 | High |

### Additional Features

- AvgMonthlySpend
- Churn_Encoded

---

## 🔍 Key Findings

### 1. Customer Churn is Significant
Approximately **26.54%** of customers have discontinued their services.

### 2. Contract Type is the Strongest Churn Driver
Month-to-Month customers show significantly higher churn rates.

### 3. Higher Monthly Charges Increase Churn Risk
Customers paying higher monthly charges are more likely to leave.

### 4. New Customers are More Vulnerable
Short-tenure customers demonstrate higher churn rates.

### 5. Fiber Optic Customers Have Higher Churn
Fiber Optic users show greater attrition compared to DSL customers.

---

## 📊 Statistical Hypothesis Testing

### Selected Hypothesis

**H₀:** There is no significant difference in monthly charges between churned and retained customers.

**H₁:** There is a significant difference in monthly charges between churned and retained customers.

### Test Used

Independent Two-Sample T-Test

### Results

| Metric | Value |
|----------|----------|
| T-Statistic | 16.54 |
| P-Value | 2.706 × 10⁻⁶⁰ |

### Conclusion

Since the p-value is significantly lower than 0.05, the null hypothesis was rejected.

The results confirm that monthly charges have a statistically significant relationship with customer churn.

---

## 💡 Business Recommendations

- Encourage customers to switch to long-term contracts.
- Develop retention programs for Month-to-Month customers.
- Provide incentives for high-paying customers.
- Improve onboarding experiences for new customers.
- Monitor Fiber Optic customers more closely for churn risk.

---

## 🚀 Future Work

- Build machine learning churn prediction models.
- Perform customer segmentation.
- Develop customer risk scoring systems.
- Integrate customer satisfaction metrics.
- Deploy predictive analytics dashboards.

---

## 📁 Project Structure

```text
telco-customer-churn-analysis/
│
├── data/
│   └── WA_Fn-UseC_-Telco-Customer-Churn.csv
│
├── notebooks/
│   └── Customer_Churn_Analysis.ipynb
│
├── report/
│   └── Customer_Churn_Report.pdf
│
├── images/
│   └── charts_and_visualizations
│
└── README.md
```

---

## 📜 License

This project is intended for educational and portfolio purposes.

---

## 👤 Author

**Daksh Rathod**

LinkedIn: *(Add your LinkedIn profile link)*

GitHub: *(Add your GitHub profile link)*

---
⭐ If you found this project useful, consider giving the repository a star.
