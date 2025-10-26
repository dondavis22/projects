🛍️ Retail Sales Analysis Dashboard

📊 Overview

This project showcases an end-to-end data analytics workflow designed to analyze retail sales performance and customer behavior. The process involves data cleaning and transformation using Python, data storage and management using MySQL, and visualization in Power BI.
The goal was to identify sales trends, customer purchasing patterns, top-performing product categories, and key performance metrics through an interactive and dynamic dashboard.

🧰 Project Workflow

1. Data Cleaning & Preprocessing (Python, Pandas)
2. Removed missing values in critical columns like Transaction_ID, Date, Customer_ID, and State.
3. Filled categorical null values (State, Product_Brand, Customer_Segment, Product_Category) with “Unknown”.
4. Filled missing Age values using the median age.
5. Resolved inconsistent gender entries for each unique Customer_ID using the most frequent (mode) gender.
6. Resolved inconsistent customer segments for each unique Customer_ID using the mode of the segment.
7. Filled missing Country values based on the State information (e.g.“California” → “USA”, “Ontario” → “Canada”, etc.).
8. Converted data types to appropriate formats: numeric fields to numeric, and date/time columns to datetime.
9. Created new derived columns:
       Total_Amt = Total_Purchases × Amount
       Extracted Year, Month from the Date column

⚙️ Database Integration (MySQL)

1. Connected to MySQL using SQLAlchemy.
2. Created a new database and stored the cleaned DataFrame as a structured table.
3. Enabled Power BI to extract and visualize data directly from MySQL for real-time analytics.

📊 Data Visualization (Power BI)

Designed an interactive Retail Sales Dashboard displaying key business insights:
  *KPIs: Total Sales, Total Customers, and Total Transactions, Average Age, Average Revenue.
  *Sales data by Product Category, Product Type, and Product Brand, visualized using pie charts with drill-down functionality.
  *Quarterly Sales Trend: Showed seasonal and time-based purchasing patterns.
  *Customer Segmentation: Highlighted customer demographics and spending behavior.
  *Dynamic Filters: Enabled filtering by Country, Year, Gender, and Customer Segment for deeper analysis.


📈 Key Insights from the Dashboard

Sales Performance: The dashboard revealed strong overall sales (~399.6M) across ~292K transactions, with ~86K unique customers.
Top Categories: Electronics category consistently contributed the majority of total sales.
Customer Segmentation: Regular customer segment accounted for a large share of purchases, indicating strong brand loyalty.
Temporal Trends: Monthly trends highlighted peak shopping periods, suggesting potential for seasonal marketing campaigns.
Geographical Insights: USA accounted for the largest share of total revenue, followed by UK & Germany.

🧠 Skills Demonstrated

Python: Pandas, NumPy, Data Cleaning, Data Transformation
SQL: SQLAlchemy, Database Creation, Data Loading
Power BI: Dashboard Design, KPI Tracking, Data Modeling, Interactive Visuals
Data Analytics: ETL Process, Trend Analysis, Customer Behavior Insights
Problem Solving: Handling inconsistent customer attributes and imputing missing values logically


🚀 Outcome

The project successfully built a data-driven retail sales analytics system that combines the power of Python, SQL, and Power BI to deliver business-ready insights. It demonstrates a complete analytics pipeline — from data preprocessing to database integration to dashboard visualization — reflecting real-world data analyst workflows.
