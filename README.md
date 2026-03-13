# 📉 Telecom Customer Churn Prediction & Analytics
### *End-to-End Data Pipeline: SQL Server → Python (ML) → Power BI*

![Power BI](https://img.shields.io/badge/Power_BI-Dashboard-yellow) ![Python](https://img.shields.io/badge/Python-ML_Model-blue) ![SQL](https://img.shields.io/badge/SQL-Data_Cleaning-orange)

## 🎯 Project Objective
The goal of this project is to identify the root causes of customer attrition and build a **Machine Learning model** to predict which current customers are likely to churn. This allows the business to transition from reactive reporting to **proactive customer retention**.

## 📊 Executive Summary Dashboard
The primary dashboard provides a high-level view of churn drivers across demographics and service types.

![Executive Summary](summary.png)
> *Dashboard Highlight: Identified that Month-to-Month contract holders and Fiber Optic users represent the highest churn risk.*

---

## 📈 Top Business Insights
* **Contractual Risk:** Month-to-Month customers churn at a rate of **46.5%**, compared to just **2.7%** for two-year contracts.
* **Service Issues:** Fiber Optic users show a **41.1%** churn rate, suggesting a potential gap between service pricing and perceived value.
* **Payment Friction:** Customers using mailed checks are significantly more likely to leave than those on automatic bank transfers.

---

## 🔍 Predictive Analytics: Identifying At-Risk Customers
Beyond historical analysis, this project uses a **Random Forest model** to predict future churners. 

![Predictive Table](prediction.png)
> *Actionable Output: The model identified **411 specific customers** currently at high risk of churn, providing the retention team with a targeted "Save List."*

---

## 🛠️ Technology Stack & Methodology
1.  **SQL Server:** Performed data cleaning, handled nulls in `Total Charges`, and created structured views for Power BI.
2.  **Python (Jupyter Notebook):** Conducted EDA and built a classification model to generate churn probabilities.
3.  **Power BI:** Developed an interactive   (Dynamic Titles, Calculated Measures) .

## 📂 Repository Contents
* `customer.pbix`: Interactive Power BI file.
* `Churn Prediction.ipynb`: Python code for the ML model.
* `SQLQuery1.sql`: Data transformation scripts.
* `Predictions.csv`: Final output of the ML model.

---

