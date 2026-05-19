# Retail Operations & Profitability Dashboard

## Overview
This project analyzes retail sales, profitability, returns, and fulfillment performance using SQL and Power BI. The dashboard was designed to identify margin leakage, operational inefficiencies, and regional return trends through KPI-driven retail analytics and business-focused data visualization

## Business Problem
Despite consistent sales growth, the business faced profitability pressure due to high discounting, return-heavy regions, and fulfillment inefficiencies. 
The objective was to identify operational and financial areas impacting overall business performance.

## Tools & Technologies
- SQL
- PostgreSQL
- Power BI
- Window Functions
- CTEs
- Time-Series Analysis

## Key Insights
- Identified over $25K in losses across Tables and Bookcases caused by aggressive discounting
- Found the West region had the highest return rate (~15%)
- Observed significantly longer fulfillment duration in Standard Class shipping modes
- Analyzed category-level profitability and operational performance across 4 years of retail data

## Dashboard Preview

<img width="1312" height="762" alt="Retail Operations" src="https://github.com/user-attachments/assets/248009c3-fceb-49d9-96d2-cced9acaee96" />

## SQL Concepts Used
- CTEs
- Window Functions
- LAG()
- RANK()
- Conditional Aggregation
- Rolling Averages
- Time-Series Analysis

## Files Included:
Sql Queries
-  YoY sales and profit growth:
```WITH yoy_growth AS(
SELECT 
	EXTRACT(YEAR FROM order_date) AS current_year,
	SUM(sales) AS total_sales,
	SUM(profit) AS total_profit,
	LAG(SUM(sales)) OVER(ORDER BY EXTRACT(YEAR FROM order_date)) AS prev_year_sales,
	LAG(SUM(profit)) OVER(ORDER BY EXTRACT(YEAR FROM order_date)) AS prev_year_profit
FROM sales
GROUP BY EXTRACT(YEAR FROM order_date) 
)
SELECT *,
	ROUND((total_sales - prev_year_sales) / prev_year_sales * 100,2) AS yoy_sales_pct,
	ROUND((total_profit - prev_year_profit) / prev_year_profit * 100,2) AS yoy_profit_pct
FROM yoy_growth;
```
- Return problems in regions with return pct:
```SELECT 
	region,
	SUM(sales) AS total_sales,
	SUM(profit) AS total_profit,
	COUNT(*) AS total_orders,
	SUM(CASE WHEN returned = 'Yes' THEN 1 ELSE 0 END) AS total_returns,
	ROUND(SUM(CASE WHEN returned = 'Yes' THEN 1 ELSE 0 END)::numeric * 100.0 / COUNT(*),2) AS return_pct
FROM sales
GROUP BY region
ORDER BY return_pct DESC;
```
- Dataset :
  [sales.csv](https://github.com/user-attachments/files/28011524/sales.csv)# Retail Operations & Profitability Dashboard
  
## Author
Sagar Hiware

- LinkedIn: https://linkedin.com/in/isagarhiware1
- GitHub: https://github.com/isagarh1

## License
This project is licensed under the MIT License.








