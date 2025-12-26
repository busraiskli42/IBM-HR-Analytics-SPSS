# 📉 IBM HR Analytics: Predicting Employee Churn with SPSS

![SPSS](https://img.shields.io/badge/Tool-IBM%20SPSS-blue?style=for-the-badge&logo=ibm)
![Status](https://img.shields.io/badge/Status-Completed-success?style=for-the-badge)
![Data](https://img.shields.io/badge/Data-Kaggle-orange?style=for-the-badge)

## 📖 Project Overview (Proje Özeti)
This project analyzes the key drivers of employee attrition (churn) using a hypothetical dataset of 1,470 employees created by IBM data scientists. The goal is to identify **why employees leave** and to build a predictive model using **Logistic Regression**.

**Key Business Question:** What are the most significant factors driving employee turnover?

## 📊 Dataset
* **Source:** [Kaggle - IBM HR Analytics Employee Attrition & Performance](https://www.kaggle.com/pavansubhasht/ibm-hr-analytics-attrition-dataset)
* **File:** `WA_Fn-UseC_-HR-Employee-Attrition.csv`
* **Rows:** 1,470
* **Features:** 35 (Age, Job Satisfaction, OverTime, Monthly Income, etc.)

## 📁 Repository Contents
* **`Untitled2.sav`**: The SPSS data file used for analysis (raw/processed data).
* **`Output1.spv`**: The full statistical output file exported from SPSS.
* **`bar_chart.png`**: Visualization of OverTime impact.
* **`scatter_plot.png`**: Visualization of Age & Income clusters.

## 🛠️ Methodology & Tools
* **Tool:** IBM SPSS Statistics
* **Process:**
    1.  **Data Cleaning:** Checked for missing values and duplicates.
    2.  **Recoding:** Converted categorical variables (Yes/No) into dummy variables (1/0) for regression.
    3.  **Modeling:** Applied **Binary Logistic Regression** to predict 'Attrition'.
    4.  **Hypothesis Testing:** Used statistical significance (p < 0.05) to validate findings.

## 💡 Key Findings (Analiz Sonuçları)

### 1. Burnout is Real (OverTime vs. Attrition)
Employees working **OverTime** are significantly more likely to leave.
* **Statistical Evidence:** The Logistic Regression model shows that OverTime increases the risk of attrition by **4.3 times** ($Exp(B): 4.29$, $p < 0.05$).

![OverTime Chart]("C:\Users\isikl\Desktop\IBM-HR-Analytics-Project\bar_chart.png")
*(Fig 1: Attrition rates significantly higher for employees working overtime)*

### 2. Losing Young Talent (Age & Income vs. Attrition)
The analysis reveals a cluster of attrition among **younger employees with lower income**.
* **Statistical Evidence:** Negative coefficients for `Age` and `MonthlyIncome` indicate that as age and income drop, the probability of leaving rises.

![Scatter Plot]("C:\Users\isikl\Desktop\IBM-HR-Analytics-Project\scatter_plot.png")
*(Fig 2: Red circles (Attrition) are clustered in the "Young & Low Income" section)*

## 🚀 Executive Summary & Recommendation
The analysis proves that attrition is a manageable risk, not a random event.
* **Problem:** High turnover in Gen Z / Junior levels and employees working overtime.
* **Solution:** To retain talent, the company must move beyond just salary increases and focus on a **sustainable work-life balance** (reducing overtime) and structured career paths for young talent.

---

## 👨‍💻 Author & Acknowledgments
**Analyst:** [Büşra Işıklı](https://www.linkedin.com/in/busraiskli/)  
**Program:** NSA Veri Analizi Okulu - Advanced Statistics  
**Instructor:** Zübeyir Nişancı

---
*If you find this analysis helpful, please ⭐ this repository!*
