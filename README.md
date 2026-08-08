# Credit Card Financial Dashboard

## Overview
This project analyzes credit card transaction and customer data using SQL, Power Query, and Power BI. The objective was to clean and transform raw transaction and customer data, perform business-focused analysis, and build an interactive two-page dashboard to uncover insights related to customer demographics, spending behavior, card tier performance, and revenue trends.

The project demonstrates an end-to-end analytics workflow:

**Data Cleaning → Data Transformation → SQL/DAX Analysis → Dashboard Development → Business Insights**

---

## Data Cleaning & Feature Engineering

**Age Segmentation**
Created customer age groups (age range 21–73) using bucketed segmentation for demographic analysis:
- 20–30
- 30–40
- 40–50
- 50–60
- 60+

**Card Category Mapping**
Standardized card tiers into consistent categories:
- Blue
- Silver
- Gold
- Platinum

**Risk & Engagement Segmentation**
Classified customers into engagement tiers (Low, Med, High) based on customer acquisition cost and satisfaction score for targeted business strategy analysis.

**Revenue & Interest Calculation**
Built DAX measures to calculate total revenue, interest earned, transaction amount, and transaction count, aggregated by quarter, gender, card category, and customer job.

---

## Tools & Technologies
- Power BI Desktop
- Power BI Service
- Power Query (M Query)
- DAX
- SQL
- Advanced Excel

---

## Dataset Information
The dataset contains credit card transaction and customer records across three linked tables:

**Transaction Data (cc_add.csv)**
- Client_Num
- Card_Category
- Annual_Fees
- Activation_30_Days
- Customer_Acq_Cost
- Week_Start_Date
- Week_Num
- Qtr
- Current_Year
- Credit_Limit
- Total_Revolving_Bal
- Total_Trans_Amt
- Total_Trans_Ct
- Avg_Utilization_Ratio
- Use_Chip
- Exp_Type
- Interest_Earned
- Delinquent_Acc

**Customer Data (customer.csv / cust_add.csv)**
- Client_Num
- Customer_Age
- Gender
- Dependent_Count
- Education_Level
- Marital_Status
- State_Cd
- Zipcode
- Car_Owner
- House_Owner
- Personal_Loan
- Contact
- Customer_Job
- Income
- Cust_Satisfaction_Score

---

## Key Insights
- Overall revenue is ₹57M with ₹8M total interest earned and ₹46M in transaction amount across 667K transactions
- Blue card holders are the primary revenue driver, contributing 83% of total revenue
- Male customers (₹31M) outperform female customers (₹26M) in overall revenue contribution
- Age group 40–50 is the strongest revenue segment across both genders
- Chip and swipe transactions account for 93% of all activity, far outweighing online transactions (7%)
- TX, NY, and CA are the top-performing states, contributing the majority of transaction volume
- Graduate-level education customers drive the highest revenue among education segments

---

## Dashboard Preview
Includes KPI cards (Total Revenue, Total Interest, Transaction Amount, Transaction Count), quarterly revenue trends, card category breakdowns, customer demographic analysis, and interactive slicers for card category, gender, quarter, and risk segment.
