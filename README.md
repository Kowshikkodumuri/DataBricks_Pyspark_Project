# DataBricks_Pyspark_Project
Sales Analytics & Profitability Analysis using PySpark
Project Overview:- This project demonstrates an end-to-end enterprise-level sales analytics pipeline built using PySpark on Databricks.
The goal is to transform raw transactional data into business-ready KPIs that help stakeholders understand sales performance, customer behavior, and profitability.

The solution follows real-world data engineering practices including data ingestion, cleaning, joins, KPI calculations, and persistence.

Business Objectives:-
Analyze sales performance across products, categories, and regions
Identify top customers and most profitable products
Measure profitability using margin-based KPIs
Enable scalable analytics suitable for large datasets
Deliver insights that support business decision-making

Dataset Description:-
Customer Sales Dataset
Contains transactional sales data with the following key fields:
order_id
order_date
customer_id
region
segment
product_id
quantity
unit_price
discount
order_status

Product Master Dataset:-
Contains product-level reference data:
product_id
product_name
category
sub_category
cost_price

Format: JSON
Volume: 500 enterprise-style records
Designed for scalability
Data Processing Workflow
Data Ingestion
Load JSON datasets into PySpark DataFrames
Data Cleaning
Handle nulls and invalid values
Filter cancelled/returned orders for revenue KPIs

Data Transformation
Create derived columns such as:
Net Sales
Profit
Profit Margin
Data Joining
Join sales data with product master using product_id
KPI Computation
Apply Spark aggregations and window functions
Persistence
Save results in Parquet/Delta format for reporting
KPIs Implemented
Core KPIs
Total Sales Revenue
Total Orders
Total Quantity Sold
Sales by Region
Sales by Product Category
Customer KPIs
Top Customers by Revenue
Average Order Value (AOV)
Advanced KPIs
Total Profit
Profit Margin (%)
Monthly Sales Trend
Top 5 Most Profitable Products 

Key Calculations
Net Sales = Quantity × Unit Price × (1 − Discount)
Profit = Net Sales − (Cost Price × Quantity)
Profit Margin (%) = (Profit / Net Sales) × 100
AOV = Total Revenue / Total Orders

Key Insights Generated
Identified products with the highest profit contribution
Analyzed customer segments generating maximum revenue
Discovered seasonal sales patterns
Compared revenue vs profitability across categories

Technologies Used
PySpark
Databricks
Spark SQL
JSON
Parquet / Delta Lake

Scalability & Real-Time Relevance
Although sample data is used, the pipeline is designed to:
Scale to millions of records
Run efficiently in distributed environments
Support production-grade analytics workloads
Future Enhancements
Integrate real-time ingestion (Kafka / Event Streams)
Build dashboards using Power BI / Tableau
Add sales forecasting and anomaly detection
Implement Delta Lake versioning and optimization

Conclusion
This project simulates a real enterprise data engineering use case, demonstrating the ability to design, implement, and scale analytics pipelines using PySpark.
It reflects skills required for Data Engineer / PySpark Developer roles.






This project simulates a real enterprise data engineering use case, demonstrating the ability to design, implement, and scale analytics pipelines using PySpark.
It reflects skills required for Data Engineer / PySpark Developer roles.
