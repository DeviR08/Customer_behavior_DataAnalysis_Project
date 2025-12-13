📊 Customer Shopping Behavior Analysis

A complete end-to-end data analysis project exploring customer shopping behavior using Python, SQL (PostgreSQL), and Power BI.
The analysis is based on 3,900 purchase transactions across multiple product categories and customer demographics.

🚀 Project Overview
This project uncovers key business insights such as:
Customer spending patterns
Product preferences
Effect of discounts
Subscription behaviors
Customer segmentation
Category-wise and demographic-wise revenue trends
The cleaned and transformed data is further used for SQL-based analytics and a final Power BI dashboard.

🗂️ Dataset Summary
Total Rows: 3,900
Columns: 18
Key Features:
Customer Details: Age, Gender, Location, Subscription Status
Purchase Info: Item Purchased, Category, Amount, Season, Size, Color
Behavioral Data: Discount Applied, Promo Code Used, Previous Purchases, Frequency, Rating, Shipping Type
Missing Values: 37 missing in review_rating (handled during cleaning)

🐍 Exploratory Data Analysis (Python)
The Python workflow includes:
✔ Data Preparation
Loaded dataset using pandas
Checked structure using df.info() and summary statistics using df.describe()
Handled missing values in review_rating using median per category
✔ Cleaning & Standardization
Converted column names to snake_case
Validated discount-related columns and removed redundant promo_code_used
✔ Feature Engineering
Created age_group by binning age values
Generated purchase_frequency_days
Ensured consistency across discount and purchase fields
✔ Database Integration
Connected Python to PostgreSQL
Loaded the cleaned dataset into a database for SQL analysis

🧮 SQL Analysis (PostgreSQL)
Key business questions answered:
Revenue by Gender – Comparison of total sales between male and female customers
High-Spending Discount Users – Customers who used discounts but still purchased above average
Top 5 Products by Rating – Based on average review scores
Shipping Type Impact – Standard vs. Express: which generates higher order value?
Subscribers vs. Non-Subscribers – Revenue and average spend comparison
Discount-Dependent Products – Products most frequently purchased with discounts
Customer Segmentation – New, Returning, Loyal buyers
Top 3 Products per Category – Based on purchase count
Repeat Buyers & Subscriptions – Are frequent buyers more likely to subscribe?
Revenue by Age Group – Contribution of each age bracket

📈 Power BI Dashboard
An interactive Power BI dashboard was created to visualize:
Revenue trends
Demographic insights
Product performance
Discount impact
Shipping patterns
Customer segments
This allows stakeholders to explore insights dynamically.

💡 Business Recommendations
Based on findings:
Boost Subscriptions: Promote exclusive benefits
Loyalty Programs: Reward repeat buyers to increase retention
Optimize Discounts: Balance margin and sales volume
Highlight Best Products: Promote top-rated and best-selling items
Targeted Marketing: Focus on high-revenue age groups & express-shipping customers

📁 Project Structure
project/
│── data/
│   └── customer_shopping_behavior.csv
│── notebooks/
│   └── eda.ipynb
│── sql/
│   └── business_queries.sql
│── dashboard/
│   └── powerbi_report.pbix
│── README.md
└── requirements.txt


🛠 Technologies Used
Python (Pandas, NumPy, Matplotlib, Seaborn)
PostgreSQL
Power BI
Jupyter Notebook
📬 Contact
For queries or improvements, feel free to open an issue or connect via GitHub!


