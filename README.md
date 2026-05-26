#  Customer Shopping Behavior Analysis

End-to-end data analytics project analyzing customer purchasing patterns, subscription behavior, customer segmentation, and revenue drivers using Python, SQL, and Power BI on a retail dataset of **3,900 customers**.

---

##  Project Structure

```
customer-shopping-behavior/
├── customer_shopping_behavior.csv        # Raw Dataset
├── customer_behaviour.ipynb              # Python EDA & Preprocessing
├── customer_shopping_behaviour.sql       # MSSQL Business Queries
├── customer_behavior_dashboard.pbix      # Power BI Dashboard
├── SCREENSHOTS/
│   └── customer_behavior_dashboard.png
└── README.md
```

---

##  Dataset Overview

Retail shopping dataset containing customer demographics, purchasing behavior, subscription details, product information, and transaction metrics.

| Feature | Description |
|---|---|
| Customer ID | Unique customer identifier |
| Age | Customer age |
| Age Group | Derived customer segment |
| Gender | Male / Female |
| Item Purchased | Purchased product |
| Category | Product category |
| Purchase Amount (USD) | Transaction value |
| Location | Customer state |
| Season | Season of purchase |
| Review Rating | Customer review score |
| Subscription Status | Subscribed / Not subscribed |
| Shipping Type | Shipping method |
| Discount Applied | Discount usage indicator |
| Previous Purchases | Count of prior purchases |
| Payment Method | Payment type |
| Frequency of Purchases | Weekly, Monthly, etc. |

---

##  Python — Data Cleaning & EDA

Performed data preprocessing and exploratory analysis using Pandas, NumPy, and Matplotlib.

### Data Cleaning & Feature Engineering

- Filled missing `review_rating` values using category-wise median
- Standardized column names into snake_case format
- Renamed inconsistent column names
- Removed redundant columns
- Created `age_group` segmentation using quartile binning
- Converted purchase frequency categories into numeric purchase-day values

### Customer Segments Created

| Segment | Description |
|---|---|
| Young Adult | Lowest age quartile |
| Adult | Second quartile |
| Middle Aged | Third quartile |
| Senior | Highest age quartile |

---

##  SQL — Business Analysis

Solved 10 business problems using Microsoft SQL Server.

| # | Question | SQL Concepts |
|---|---|---|
| 1 | Revenue by gender | `GROUP BY`, `SUM` |
| 2 | High-spending discount users | Subqueries |
| 3 | Top-rated products | `AVG`, `TOP`, `ORDER BY` |
| 4 | Shipping comparison | `HAVING` |
| 5 | Subscriber spending analysis | `COUNT`, `SUM`, `AVG` |
| 6 | Discount usage percentage | `CASE WHEN` |
| 7 | Customer loyalty segmentation | CTE |
| 8 | Top products per category | `ROW_NUMBER()` |
| 9 | Repeat buyers & subscriptions | Aggregation |
| 10 | Revenue by age group | `GROUP BY` |

---

##  Dashboard Pages

| Page | Description |
|---|---|
| **Overview** | KPI cards for customers, average purchase amount, and review ratings |
| **Subscription Analysis** | Customer distribution by subscription status |
| **Category Performance** | Revenue and sales analysis across product categories |
| **Customer Segmentation** | Revenue and sales comparison by age groups |
| **Interactive Filtering** | Dynamic filtering by subscription status, gender, category, and shipping type |

---

##  Dashboard Preview

### Customer Shopping Behavior Dashboard
![Dashboard](SCREENSHOTS/customer_behavior_dashboard.png)

---

##  Tools Used


- **Jupyter Notebook** — Analysis environment 
- **Python** — Data cleaning & EDA 
- **Pandas** — Data manipulation 
- **Microsoft SQL Server** — Business analysis queries
- **Power BI Desktop** — Dashboard development 

---

##  Key Insights

- Subscription customers contribute significantly higher revenue
- Loyal customers are more likely to maintain subscriptions
- Middle-aged and adult customer groups generate the highest sales
- Discount usage does not always reduce purchase value
- Clothing category generated the highest revenue and sales
- Average customer review rating remained strong across categories

---

##  Author

**K Pramod Herald**

-  kpherald7@gmail.com
- [LinkedIn](https://www.linkedin.com/in/k-pramod-herald-92a27b295)

---

⭐ If you found this project useful, consider giving it a star!
