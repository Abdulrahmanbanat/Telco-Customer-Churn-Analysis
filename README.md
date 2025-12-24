# Telco Customer Churn Analysis

##  Project Overview
This project analyzes customer churn behavior for a telecommunications company using the **Telco Customer Churn dataset (IBM Sample Dataset)**.  
The goal is to identify the key factors influencing customer churn and provide **data-driven insights and recommendations** to help reduce churn, improve customer retention, and increase revenue.

The project follows a complete analytics workflow:
**Data Cleaning → SQL Analysis → Data Visualization**

---

##  Business Objective
- Identify patterns and drivers of customer churn
- Analyze churn across contracts, services, payment methods, and demographics
- Provide actionable recommendations for retention strategies

---

##  Data Source
- **Dataset:** Telco Customer Churn Dataset  
- **Provider:** IBM Sample Dataset  
- **Platform:** Kaggle  
- **Privacy:** Public dataset with no personally identifiable information (PII)

---

##  Tools & Technologies
- **Excel** – Data cleaning and preprocessing  
- **PostgreSQL** – Data analysis and aggregation  
- **Power BI** – Data visualization and dashboard creation  

---

##  Data Cleaning & Preparation (Excel)
Steps performed:
1. Downloaded the dataset as a CSV file.
2. Opened the CSV file in Excel and saved it as XLSX for easier processing.
3. Converted all columns to appropriate data types (Text / Number).
4. Removed 11 rows with missing `TotalCharges` values related to new customers (`tenure = 0`).
5. Checked for duplicate `customerID` values (none found).
6. Verified that no missing values remained in critical columns.
7. Checked for outliers in `MonthlyCharges` (values were within the expected range).
8. Saved the final clean dataset as **`clean_telco_churn.csv`**.

---

##  Data Analysis (PostgreSQL)
SQL was used to generate structured summary tables for visualization:

### 1️ Churn Overview
- Overall customer distribution by churn status (Yes / No)
- Churn percentage

### 2️ Contract Analysis
- Churn rate by contract type:
  - Month-to-month
  - One year
  - Two year

### 3️ Internet Service Analysis
- Churn behavior by internet service type:
  - DSL
  - Fiber optic
  - No internet

### 4️ Payment Method Analysis
- Churn rate by payment method
- Identification of high-risk payment behaviors

### 5️ Demographics Analysis
- Churn analysis by:
  - Gender
  - SeniorCitizen
  - Partner
  - Dependents

### 6️ Charges & Tenure Analysis
- Average Monthly Charges by Internet Service
- Average Tenure (months) by Internet Service

---

##  Dashboard (Power BI)
The Power BI dashboard visualizes the SQL-generated summary tables to highlight churn patterns across:
- Contract types
- Internet services
- Payment methods
- Customer demographics
- Charges and tenure

The dashboard is designed for **quick business insights and decision-making**.

### Dashboard Previews

### Executive Overview
![Executive Overview](https://raw.githubusercontent.com/Abdulrahmanbanat/Telco-Customer-Churn-Analysis/main/Images/Executive%20Overview.png)


### Contract & Payment Analysis
![Contract & Payment Analysis](https://github.com/Abdulrahmanbanat/Telco-Customer-Churn-Analysis/blob/main/Images/Contract%20%26%20Payment%20Analysis%20Report.png)


---

##  Key Insights & Recommendations

###  Payment Method Optimization
**Insight:**  
Customers using **Electronic Check** have the highest churn rate (~45%).

**Recommendation:**  
Encourage customers to switch to **Credit Card (Automatic)** or **Bank Transfer** by offering small incentives such as discounts or loyalty points.

---

###  Contract Conversion Strategy
**Insight:**  
Month-to-month contracts show significantly higher churn compared to long-term contracts.

**Recommendation:**  
Promote **One-year** and **Two-year** contracts through bundled services or special offers to increase customer commitment.

---

###  Service & Support Synergy
**Insight:**  
Fiber optic users experience higher churn, but churn decreases when **Technical Support** is active.

**Recommendation:**  
Implement proactive technical support programs for fiber optic customers to improve retention in this high-value segment.

---
##  Conclusion
This project demonstrates a full data analytics workflow using real-world data.  
It highlights strong skills in **data cleaning, SQL analysis, and data visualization**, with a clear focus on translating data into actionable business insights.
