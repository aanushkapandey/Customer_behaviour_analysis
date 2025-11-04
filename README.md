# Customer_behaviour_analysis
🛍️ Customer Shopping Behavior Analysis
📘 Project Overview

The Customer Shopping Behavior Analysis project explores insights from 3,900 customer transactions to understand shopping patterns, product preferences, and subscription trends.
The goal is to uncover actionable insights that help businesses optimize marketing strategies, boost customer retention, and improve revenue performance.

📂 Dataset Summary
Property	Details
Rows	3,900
Columns	18
Missing Data	37 missing values in review_rating
Data Source	Customer transactional and demographic data
Key Features

Demographics: age, gender, location, subscription_status

Purchase Details: item_purchased, category, purchase_amount, season, size, color

Shopping Behavior: discount_applied, promo_code_used, previous_purchases, frequency_of_purchases, review_rating, shipping_type

🧹 Data Cleaning & Preparation (Python)

Performed in Python (pandas, numpy, matplotlib, seaborn):

Data Loading: Imported CSV into pandas.

Exploration: Used df.info(), df.describe(), and visual summaries.

Missing Data: Imputed missing review_rating values with median ratings per product category.

Standardization: Renamed columns to snake_case for readability.

Feature Engineering:

Created age_group column by binning customer ages.

Derived purchase_frequency_days column.

Redundancy Check: Dropped promo_code_used due to overlap with discount_applied.

Database Integration: Loaded cleaned DataFrame into PostgreSQL for further SQL analysis.

🧮 SQL Business Analysis

Performed PostgreSQL queries to answer business-critical questions:

#	Analysis	Objective
1	Revenue by Gender	Compare total revenue between male and female customers.
2	High-Spending Discount Users	Identify customers using discounts but spending above average.
3	Top 5 Products by Rating	Find products with highest average review ratings.
4	Shipping Type Comparison	Compare average spend between Standard vs. Express shipping.
5	Subscribers vs. Non-Subscribers	Analyze revenue differences based on subscription.
6	Discount-Dependent Products	Identify products with high percentage of discounted purchases.
7	Customer Segmentation	Categorize customers as New, Returning, Loyal.
8	Top 3 Products per Category	Find most purchased items within each category.
9	Repeat Buyers & Subscriptions	Correlate frequent buyers (>5 purchases) with subscription likelihood.
10	Revenue by Age Group	Calculate revenue contribution by each age group.
📊 Power BI Dashboard

An interactive Power BI dashboard was created to visualize insights from SQL and Python analyses.

Dashboard Features:

Revenue trends by gender, age, and subscription status

Top-rated and top-selling products

Discount and shipping-type comparisons

Customer loyalty segmentation

💡 Business Insights & Recommendations
Area	Recommendation
Subscriptions	Promote exclusive benefits to increase subscriber base.
Loyalty Programs	Reward repeat buyers to encourage long-term retention.
Discount Strategy	Reassess discount policy to maintain margins.
Product Positioning	Highlight top-rated and high-revenue products in campaigns.
Targeted Marketing	Focus campaigns on high-value age groups and express-shipping users.
🧰 Tech Stack
Tool	Purpose
Python (pandas, numpy, seaborn)	Data cleaning, preprocessing, and visualization
PostgreSQL	SQL-based business insights and aggregation
Power BI	Dashboard and visual storytelling
Excel / CSV	Dataset input and export format
🗂️ Folder Structure
Customer_Shopping_Behavior_Analysis/
│
├── data/
│   ├── customer_shopping_behavior.csv
│
├── notebooks/
│   ├── data_cleaning.ipynb
│   ├── exploratory_analysis.ipynb
│
├── sql/
│   ├── business_queries.sql
│
├── dashboard/
│   ├── PowerBI_Dashboard.pbix
│
├── reports/
│   ├── insights_summary.pdf
│
└── README.md

🚀 How to Run the Project

Clone Repository

git clone https://github.com/yourusername/customer-shopping-behavior-analysis.git
cd customer-shopping-behavior-analysis


Install Dependencies

pip install pandas numpy seaborn matplotlib psycopg2


Run Python Scripts

python notebooks/data_cleaning.ipynb


Run SQL Queries

Import the cleaned_data table into PostgreSQL.

Execute queries from /sql/business_queries.sql.

Open Dashboard

Load the .pbix file in Power BI Desktop to explore visuals.

🏁 Conclusion

This project demonstrates how data-driven insights can guide business strategy in retail and e-commerce.
By integrating Python, SQL, and Power BI, we created a full-cycle data analysis pipeline — from raw data to interactive visualization and actionable recommendations.
