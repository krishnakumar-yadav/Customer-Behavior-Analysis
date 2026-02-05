# 🛒 Customer Shopping Behavior Analysis

## 📌 Project Overview
This project focuses on analyzing **customer shopping behavior** using transactional data from **3,900 purchases** across multiple product categories.  
The goal is to identify **spending patterns, customer segments, product preferences, and subscription behavior** to support data-driven business decisions.

<p align="center">
  <img src="image.png" width="800">
  
## 📂 Dataset Summary
- **Total Rows:** 3,900  
- **Total Columns:** 18  

### Key Features
- **Customer Demographics:** Age, Gender, Location, Subscription Status  
- **Purchase Details:** Item Purchased, Category, Purchase Amount, Season, Size, Color  
- **Shopping Behavior:**  
  - Discount Applied  
  - Previous Purchases  
  - Frequency of Purchases  
  - Review Rating  
  - Shipping Type  

⚠️ **Missing Data:**  
- 37 missing values in the `Review Rating` column


## 🧹 Data Cleaning & Preparation (Python)
Data preprocessing was done using **Python (Pandas & NumPy)**.

### Steps Performed:
- Loaded dataset using `pandas`
- Used `df.info()` and `df.describe()` for initial exploration
- Handled missing values in **Review Rating** using **median rating per product category**
- Standardized column names to **snake_case**
- Feature Engineering:
  - Created `age_group` column
  - Created `purchase_frequency_days`
- Removed redundant column (`promo_code_used`)
- Loaded cleaned data into **PostgreSQL** for SQL analysis

## 🗄️ SQL Analysis (PostgreSQL)
Business-focused SQL queries were written to answer key questions:

1. Revenue comparison by **Gender**
2. High-spending customers who still used **discounts**
3. **Top 5 products** by average review rating
4. Purchase amount comparison by **Shipping Type**
5. Subscribers vs Non-Subscribers revenue analysis
6. **Discount-dependent products**
7. Customer segmentation:
   - New
   - Returning
   - Loyal
8. Top 3 products per category
9. Subscription likelihood of repeat buyers (>5 purchases)
10. Revenue contribution by **Age Group**


## 📊 Power BI Dashboard
An interactive **Power BI dashboard** was created to visualize:
- Revenue trends
- Customer segments
- Subscription behavior
- Product performance
- Shipping preferences

This helps stakeholders quickly understand insights and take action.


## 💡 Business Recommendations
- 📈 Promote **subscription plans** with exclusive benefits
- 🎯 Introduce **loyalty programs** for repeat customers
- ⚖️ Optimize **discount strategy** to protect margins
- ⭐ Highlight **top-rated & best-selling products**
- 👥 Focus marketing on **high-revenue age groups** and **express shipping users**


## 🛠️ Tools & Technologies
- **Python** (Pandas, NumPy)
- **PostgreSQL**
- **Power BI**
- **Git & GitHub**

