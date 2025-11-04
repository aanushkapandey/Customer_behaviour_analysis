# 🛍️ Customer Shopping Behavior Analysis

## 📘 Project Overview
The **Customer Shopping Behavior Analysis** project explores insights from **3,900 customer transactions** to understand **shopping patterns, product preferences, and subscription trends**.  
The goal is to uncover actionable insights that help businesses **optimize marketing strategies, boost customer retention, and improve revenue performance**.

---

## 📂 Dataset Summary

| **Property** | **Details** |
|---------------|-------------|
| **Rows** | 3,900 |
| **Columns** | 18 |
| **Missing Data** | 37 missing values in `review_rating` |
| **Data Source** | Customer transactional and demographic data |

### **Key Features**
- **Demographics:** `age`, `gender`, `location`, `subscription_status`
- **Purchase Details:** `item_purchased`, `category`, `purchase_amount`, `season`, `size`, `color`
- **Shopping Behavior:** `discount_applied`, `promo_code_used`, `previous_purchases`, `frequency_of_purchases`, `review_rating`, `shipping_type`

---

## 🧹 Data Cleaning & Preparation (Python)

Performed in **Python** using `pandas`, `numpy`, `matplotlib`, and `seaborn`.

### Steps:
1. **Data Loading:** Imported the dataset using pandas.  
2. **Exploration:** Used `df.info()`, `df.describe()`, and visual summaries.  
3. **Missing Data:** Imputed missing `review_rating` values using median ratings per product category.  
4. **Standardization:** Renamed columns to `snake_case` for readability.  
5. **Feature Engineering:**
   - Created `age_group` column by binning customer ages.  
   - Derived `purchase_frequency_days` column.  
6. **Redundancy Check:** Dropped `promo_code_used` due to overlap with `discount_applied`.  
7. **Database Integration:** Loaded cleaned DataFrame into **PostgreSQL** for further SQL analysis.

---

## 🧮 SQL Business Analysis

Performed **MySQL** queries to answer key business questions:

| **#** | **Analysis** | **Objective** |
|-------|---------------|----------------|
| 1 | Revenue by Gender | Compare total revenue between male and female customers. |
| 2 | High-Spending Discount Users | Identify customers using discounts but spending above average. |
| 3 | Top 5 Products by Rating | Find products with highest average review ratings. |
| 4 | Shipping Type Comparison | Compare average spend between Standard vs. Express shipping. |
| 5 | Subscribers vs. Non-Subscribers | Analyze revenue differences based on subscription. |
| 6 | Discount-Dependent Products | Identify products with high percentage of discounted purchases. |
| 7 | Customer Segmentation | Categorize customers as New, Returning, or Loyal. |
| 8 | Top 3 Products per Category | Find most purchased items within each category. |
| 9 | Repeat Buyers & Subscriptions | Correlate frequent buyers (>5 purchases) with subscription likelihood. |
| 10 | Revenue by Age Group | Calculate revenue contribution by each age group. |

---

## 📊 Power BI Dashboard

An **interactive Power BI dashboard** was created to visualize insights from SQL and Python analyses.

### **Dashboard Features**
- Revenue trends by gender, age, and subscription status  
- Top-rated and top-selling products  
- Discount and shipping-type comparisons  
- Customer loyalty segmentation  

---

## 💡 Business Insights & Recommendations

| **Area** | **Recommendation** |
|-----------|--------------------|
| **Subscriptions** | Promote exclusive benefits to increase subscriber base. |
| **Loyalty Programs** | Reward repeat buyers to encourage long-term retention. |
| **Discount Strategy** | Reassess discount policy to maintain profit margins. |
| **Product Positioning** | Highlight top-rated and high-revenue products in campaigns. |
| **Targeted Marketing** | Focus campaigns on high-value age groups and express-shipping users. |

---

## 🧰 Tech Stack

| **Tool** | **Purpose** |
|-----------|-------------|
| **Python (pandas, numpy, seaborn)** | Data cleaning, preprocessing, and visualization |
| **MySQL** | SQL-based business insights and data aggregation |
| **Power BI** | Dashboard and visual storytelling |
| **Excel / CSV** | Dataset input and export format |

---

## 🗂️ Folder Structure
Customer_Shopping_Behavior_Analysis/

data/

customer_shopping_behavior.csv

notebooks/

Customer_Shopping_Behaviour_Analysis.ipynb

sql/

customer_behaviour_sql_query.sql

dashboard/

dashboard.pbix

reports/

Customer_Shopping_Behaviour_Analysis.pdf

README.md

## 🏁 Conclusion
This project demonstrates how **data-driven insights** can shape strategic business decisions in the retail and e-commerce industry.  

By integrating **Python, SQL, and Power BI**, we built a complete analytics workflow — from **data cleaning and preprocessing** to **SQL-based business analysis** and **interactive Power BI dashboards**.  

The analysis uncovered valuable insights into **customer purchase behavior, product performance, and subscription trends**, empowering businesses to make **data-backed marketing and operational decisions** that drive growth, profitability, and customer loyalty.


