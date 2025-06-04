<h2>Project Overview</h2>
The Order Data ETL and Sales Analysis project is a complete data pipeline and analytical reporting solution focused on e-commerce order transactions. Built using Python and MySQL, this project simulates a real-world retail sales environment where data is ingested, cleaned, enriched, and analyzed for performance insights. By combining Python’s powerful data wrangling tools with SQL’s analytical capabilities, the project enables stakeholders to make informed decisions about product performance, regional trends, and sales growth.

<br />

<h2>Key Features</h2>

- <strong>Data Ingestion and Cleaning</strong>  
Raw order data is imported from a CSV file using pandas, with missing values handled appropriately. Optional preprocessing steps standardize column names by converting them to lowercase and replacing spaces with underscores.

- <strong>Feature Engineering</strong>  
New fields such as <code>profit</code> are derived using formulas (e.g., <code>profit = sale_price - cost_price</code>), and dates are converted to datetime format for advanced time-based analytics. Redundant columns are removed to optimize data structure.

- <strong>ETL and Database Loading</strong>  
The cleaned and transformed data is loaded into a MySQL database using SQLAlchemy and PyMySQL. Data is appended to a table named <code>df_orders</code> to support incremental data loading workflows.

- <strong>SQL-Based Business Analysis</strong>  
The project includes SQL queries to perform key analyses, such as:
  - Top 10 highest revenue-generating products
  - Top 5 best-selling products in each region using window functions
  - Month-over-month sales comparison for 2022 vs. 2023
  - Highest-grossing month per product category
  - Sub-category with the largest year-over-year growth in profit

These queries leverage CTEs, aggregation, date functions, and <code>ROW_NUMBER()</code> to extract meaningful patterns and trends.

<br />

<h2>Tech Stack</h2>

- Python (pandas, SQLAlchemy) – Data ingestion, transformation, and database integration  
- MySQL – Data storage and SQL-based analytics  
- PyMySQL – MySQL database connector for Python  
- SQL – Advanced queries for business insights (CTEs, window functions, aggregation)

<br />

<h2>Why This Project?</h2>

This project was created to demonstrate the full lifecycle of a data analytics pipeline — from raw CSV ingestion to deep business insights through SQL. It mimics how sales and operations teams at an e-commerce or retail company would use data to track product performance, identify high-growth areas, and plan inventory. By integrating both Python and SQL components, the project provides a scalable foundation for real-time dashboards or business intelligence reporting tools like Power BI or Tableau.
