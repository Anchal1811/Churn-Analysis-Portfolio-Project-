# 📉 Telecom Customer Churn Prediction & Analytics
### *End-to-End Data Pipeline: SQL Server → Python (ML) → Power BI*

![Power BI](https://img.shields.io/badge/Power_BI-Dashboard-yellow) ![Python](https://img.shields.io/badge/Python-ML_Model-blue) ![SQL](https://img.shields.io/badge/SQL-Data_Cleaning-orange)

## 🎯 Business Problem
A telecommunications company is experiencing a loss of customers (churn). The goal of this project is to provide the retention team with **predictive and descriptive analytics** to:
1.  Understand **why** customers left in the past.
2.  Identify **who** is at high risk of leaving now.
3.  Implement data-driven strategies to reduce churn and save revenue.

## 📊 Completed Dashboard
This interactive Power BI dashboard provides an executive overview and deep-dive analysis of all churn metrics.

![Full Dashboard Preview](summary.png)
> *Interactive Power BI dashboard focused on user experience (UX) and clean visual design.*

---

## 📈 Top 5 Strategic Business Insights
The analysis of historical and predicted data yielded the following actionable insights:

1.  **Contract Type & Financial Risk:** Customers on **Month-to-Month contracts** have a churn rate of **46.5%**, while 2-year contracts are under **3%**. This segment represents the single greatest point of failure in retention.
2.  **Service Dissatisfaction:** **Fiber Optic** internet service has a churn rate of **41.1%**, significantly higher than DSL (**19.4%**). This indicates either a massive quality-of-service issue or a mismatch between price and value for this high-speed offering.
3.  **Payment Method Sensitivity:** Customers paying by **Mailed Check** churn at **37.8%**, while **Bank Transfer (Automatic)** is only **14.8%**. Mailed check customers face constant friction (remembering to mail it, delayed payments), making them an easier target for competitor switching.
4.  **Tenure & Revenue Loss:** Churn is most severe among customers who have been with the company for **less than 6 months** (**26.4%**). The company is failing to retain new customers, resulting in a loss of lifetime customer value.
5.  **Targeted Retention List:** Using **Machine Learning**, the dashboard provides a definitive **"Customers at Risk"** list, identifying **378 high-value customers** who require immediate attention from the retention team.

---

## 🛠️ Data Pipeline & Methodology

### 1. Data Cleaning & View Creation (SQL)
* Cleaned a dataset of **6,418 customers** using **SQL Server**.
* Handled missing values in "Total Charges," resolved duplicates, and transformed data types.
* Created **SQL Views** (one for demographic data, one for account info) to ensure a standardized, direct import into Power BI, reducing transformation load in Power Query.

### 2. Machine Learning & Predictive Analytics (Python)
* Performed **EDA** to select top churn predictors.
* Developed a **Random Forest** classification model in a Jupyter Notebook.
* The model generated a **Predictions.csv** file, appending a "Churn Prediction" flag (0 or 1) to all active customer IDs.

### 3. Data Visualization & UI/UX (Power BI)
* Built a single-page, professional dashboard focusing on modern design.
* **DAX Development:** Used advanced DAX to calculate **Total Customers**, **New Joiners**, **Churn Rate**, and a dynamic title measure that combines text with live numbers.
* **Format & Flow:** Applied complex formatting tricks to achieve clean transparency for the summary cards over the main blue background shape.

## 🔍 Predictive Table: The ML Output
This table shows the **378 specific customers** (like `11751-TAM`) the Machine Learning model identified as "High Risk," allowing the retention team to focus their limited resources on the highest-probability save opportunities.

![Customers at Risk Table](predictions_table.png)

## 📂 Repository Structure
* `/SQLQuery1.sql`: SQL scripts for cleaning and view creation.
* `/Churn Prediction.ipynb`: Python Jupyter Notebook for the Random Forest model.
* `/customer.pbix`: The final Power BI Desktop file.
* `/summary.png`: Screenshot of the completed dashboard.
* `/predictions_table.png`: Screenshot of the ML-driven risk table.

---

## 📩 Contact & Portfolio
**Anchal**
[LinkedIn Profile](#) | [Portfolio Website](#) | [GitHub Profile](https://github.com/Anchal1811) | [Email Me](mailto:anchal@example.com)
