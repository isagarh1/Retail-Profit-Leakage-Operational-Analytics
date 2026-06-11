# Retail Profit Leakage & Operational Analytics

## Project Overview

An end-to-end Business Intelligence project built using PostgreSQL and Power BI to analyze retail sales performance, profitability, returns, fulfillment efficiency, and profit leakage across a multi-year retail dataset.

The project goes beyond traditional sales reporting by identifying operational and financial factors that negatively impact profitability, including excessive discounting, loss-making customers, high-return regions, and fulfillment inefficiencies.

The analysis was conducted using SQL for data exploration and business analysis, followed by Power BI for dashboard development and executive-level reporting.

---

# Business Problem

Despite generating strong sales revenue, the business experienced profitability challenges due to margin erosion, return-heavy regions, aggressive discounting, and operational inefficiencies.

The objective was to identify where profit leakage occurs and determine the key operational and commercial factors affecting overall business performance.

---

# Project Objectives

- Analyze overall sales, profit, and margin performance
- Identify loss-making categories and customers
- Measure the impact of discounting on profitability
- Evaluate return trends across regions
- Assess fulfillment and shipping performance
- Analyze sales representative efficiency
- Identify profitable geographic markets and routes
- Generate business recommendations to improve profitability

---

# Tools & Technologies

| Tool | Purpose |
|--------|---------|
| PostgreSQL | Data Analysis & Querying |
| Power BI | Dashboard Development |
| DAX | KPI Calculations |
| CTEs | Complex Business Analysis |
| Window Functions | Trend & Ranking Analysis |
| Time-Series Analysis | Growth & Performance Tracking |

---

# Dataset Overview

The dataset contains retail transaction data including:

- Orders
- Customers
- Products
- Categories & Sub-Categories
- Sales
- Profit
- Discounts
- Returns
- Regions
- States & Cities
- Shipping Modes
- Fulfillment Dates
- Sales Representatives

---

# Key Business Metrics

| Metric | Value |
|---------|---------|
| Total Sales | $2.30M |
| Total Profit | $286.4K |
| Profit Margin | 12.47% |
| Total Orders | 5K |
| Return Rate | 8.0% |
| Avg Fulfillment Days | 34.6 |

---

# SQL Analysis Performed

The SQL workflow focused on uncovering profitability risks, operational inefficiencies, and business growth opportunities.

## Data Validation & Cleaning

- Duplicate record checks
- Data quality validation
- Null value analysis
- Date formatting and transformation

---

## Business Performance Analysis

- Sales & Profit KPIs
- Year-over-Year Growth Analysis
- Month-over-Month Growth Analysis
- Quarterly Performance Analysis
- Rolling Revenue Trends

### SQL Concepts Used

- Aggregate Functions
- CASE Statements
- GROUP BY
- ORDER BY
- Common Table Expressions (CTEs)
- Window Functions
- LAG()
- RANK()
- Rolling Averages

---

## Profit Leakage Analysis

Investigated profitability issues through:

- Loss-Making Categories
- Loss-Making Customers
- Discount Impact Analysis
- Margin Erosion Detection
- Category-Level Profitability Analysis

---

## Returns Analysis

Evaluated:

- Return Rate by Region
- Return Impact on Profitability
- Return Concentration Analysis
- Regional Return Trends

---

## Operations & Fulfillment Analysis

Analyzed:

- Shipping Mode Performance
- Average Fulfillment Duration
- Delivery Efficiency
- Operational Bottlenecks

---

## Customer & Retention Analysis

Evaluated:

- Customer Segmentation
- Customer Profitability
- Churn Customer Identification
- Repeat Purchase Behavior

---

## Geographic Performance Analysis

Analyzed:

- State-Level Profitability
- City-Level Profitability
- Most Profitable Routes
- Regional Performance Trends

---

# Power BI Dashboard

## Page 1 — Executive Overview

Provides a high-level view of business performance through:

### KPI Cards

- Total Sales
- Total Profit
- Profit Margin %
- Return Rate %
- Total Orders
- Avg Fulfillment Days

### Executive Analysis

- Monthly Sales & Profit Margin Trends
- Regional Performance Analysis
- Top Profit-Generating Sub-Categories
- Loss-Making Sub-Categories
- Shipping Mode Performance

---

## Page 2 — Profit Leakage & Operational Analytics

Focused on identifying factors driving profitability pressure.

### Profit Leakage Analysis

- Discount Impact on Sales & Profitability
- Loss-Making Customers Analysis
- Customer Profitability by Sub-Category

### Commercial & Operational Performance

- Sales Representative Efficiency
- Profitability by Geographic Route
- Margin Erosion Analysis

### Executive Insights

Highlights key drivers of profit leakage and operational inefficiencies.

---

# Key Insights

- Profit margin declined significantly as discount levels increased.
- Profitability turned negative in higher discount bands, indicating margin erosion from aggressive discounting.
- Tables, Bookcases, and Supplies were the primary loss-making sub-categories.
- Approximately 155 customers generated negative cumulative profit contribution.
- The West region recorded the highest return rate, contributing to profitability pressure.
- Standard Class shipping showed the longest fulfillment duration.
- Profitability varied significantly across sales representatives and geographic markets.

---

# Business Recommendations

## 1. Optimize Discount Strategy

Reduce excessive discounting and implement targeted promotional campaigns to improve profitability while maintaining sales performance.

## 2. Address Profit Leakage

Regularly monitor loss-making products and customers to identify opportunities for pricing adjustments, product rationalization, or operational improvements.

## 3. Improve Return Management

Investigate high-return regions and product groups to reduce return-related costs and improve customer satisfaction.

## 4. Strengthen Sales Performance Monitoring

Evaluate sales representatives using profit-based KPIs alongside revenue targets to encourage sustainable growth.

## 5. Improve Operational Efficiency

Optimize fulfillment processes and shipping strategies to reduce delivery delays and improve operational performance.

---

# Dashboard Preview

## Executive Overview
 <img width="1280" height="721" alt="Overview" src="https://github.com/user-attachments/assets/7e24b9ba-36cb-4fcf-b5e7-e96d853cc111" />
 
## Profit Leakage & Operational Analytics
<img width="1282" height="710" alt="Profit leakage" src="https://github.com/user-attachments/assets/daa78eb9-9838-4629-b06c-0d3d8af08bd7" />

---

# Files Included

- Power BI Dashboard (.pbix)
- SQL Analysis Queries
- Dashboard Screenshots
- Project Documentation

---

## Author

**Sagar Hiware**

LinkedIn: https://linkedin.com/in/isagarhiware1

GitHub: https://github.com/isagarh1
