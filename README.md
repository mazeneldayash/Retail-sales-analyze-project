📊 Retail Sales Analytics – End-to-End Data Analysis Project
Python • SQL • Power BI
📍 Introduction
This project is an end-to-end retail sales analytics workflow created using uncleaned real-world retail data.
The main objective was to clean messy raw data, prepare it for analysis, build meaningful KPIs using SQL, 
and create an interactive Power BI dashboard that provides insights into customer behavior, sales performance, and product trends.

🧾 Dataset Information
The uncleaned real data contained the following columns:
-Date
-Transaction ID
-Customer ID
-Customer Phone Number
-Customer Age
-Customer Gender
-Transaction Method
-Product Category
-Brand Name
-City
-State
-Quantity
-Unit Price
-Cost
-Review After 2 Months
This dataset had many errors such as wrong formats, inconsistent names, missing values, duplicates, outliers, and unmatched brand–category combinations.

🧹 Python – Data Cleaning & Preparation
All cleaning work was done using the script:
Python/Retail sales data - Cleaned.py

✔ Tasks completed in Python:
-Removed duplicates
-Cleaned and standardized date formats
-Standardized transaction_id and customer_id
-Cleaned phone numbers and age values
-Standardized and corrected gender and transaction method
-Fuzzy matched and corrected product categories, brands, cities
-Generated branch_id and sales_rep based on city
-Removed rows with wrong brand-category mapping
-Treated outliers (using IQR + category-level price ranges)
-Filled missing values using grouped medians and modes
-Created important columns:
-total_price = quantity * unit_price
-profit = total_price – (quantity * cost)
-Exported final cleaned dataset → Retail sales data - Cleaned.csv

🗄️ SQL – KPIs & Business Analysis
All SQL work is in:
SQL/Retail sales data - Analyze.sql

✔ Tasks completed in SQL:
-Loaded cleaned CSV into MySQL table
-Created KPI view (Total Sales, Total Profit, Avg Sales, Quantity, Customer Count)
-Yearly, Monthly, and Quarterly sales & profit analysis
-Category-wise and Brand-wise metrics
-State, City & Branch analysis
-Gender-wise and Age-group customers analysis
-Customer Lifetime Value (CLV) view
-Repeated customers analysis
-Review & Rating analysis (Brand, Category, Product)
-Created SQL stored procedures:
-Top 5 by Sales
-Bottom 5 by Sales

Created SQL functions for:
-AOV (Average Order Value)
-Profit Margin
-Created a final KPI view combining multiple metrics

📊 Power BI – Dashboard & Visualization
Dashboard file: PowerBI/Retail sales data - Dashboard.pbix

✔ Things done in Power BI:
-Loaded cleaned dataset
-Built a multi-page dashboard including:
-Executive Summary
-Sales & Profit Trends
-Category & Brand Performance
-Customer Insights
-Sales Rep Performance
-State & City Analysis
-Applied slicers for dynamic filtering
-Used DAX for calculated fields (if required)
-Designed a clean, interactive, insights-focused report

🎯 What I Learned
Through this project, I improved my skills in:
🧑‍💻 Python:
-Handling extremely messy real-world data
-Fuzzy matching using RapidFuzz
-Outlier treatment methods
-Feature engineering
-Data validation & cleaning automation

🗄️ SQL:
-Creating views, functions, and stored procedures
-Building analytical queries for KPIs
-Grouped aggregations and segmentation
-Managing real datasets with multiple dimensions

📊 Power BI:
-Building business dashboards
-Using slicers, drill-downs, and interactions
-Visual storytelling with KPI cards, charts, and maps
-Connecting cleaned data with insights
