# ElectroHub Sales Analytics Dashboard

## Brief One Line Summary
An interactive Power BI dashboard analyzing sales, profit, and product performance for ElectroHub, a retail company, to support inventory and pricing decisions.

## Overview
This project analyzes retail sales data across products, regions, and time periods to identify performance trends, profitability drivers, and underperforming inventory using Excel, Power Query, and Power BI.

## Problem Statement
ElectroHub needed a comprehensive sales analytics solution to answer key business questions, including:
1. Identifying the top and bottom 5 products by sales, profit, and quantity sold
2. Understanding how sales trends vary over time (daily, monthly, quarterly, annually)
3. Analyzing the relationship between sales and profit
4. Comparing sales, profit, and quantity sold between any two user-selected periods
5. Calculating the average discount offered across each discount category
6. Tracking the total number of orders
7. Providing order-level detail (sales, profit, discount, net sales) filterable by product, date, customer, and promotion category
8. Visualizing sales performance across different cities

## Dataset
Retail sales dataset including Order Date, Product, Category, Region, Customer, Quantity, Price per Unit, Discount, and Sales/Revenue fields.

## Tools and Technologies
- Excel (data cleaning, formulas)
- Power Query (joins, custom columns, transformations)
- Power BI (data modeling, DAX, visualization)

## Methods
- Cleaned raw data: removed duplicates, handled nulls, standardized text and data types
- Used Power Query left outer joins to integrate price-per-unit and discount data
- Built a relational data model with one-to-many relationships across fact and dimension tables
- Created DAX measures for Total Sales, Total Profit, Total Quantity, and period-over-period comparisons

## Key Insights
- Top 5 products drove ~73% of total sales and profit
- Bottom 5 products sold nearly as many units (1,061 vs. 1,352) as top performers but generated under 1% of profit — indicating a pricing/margin issue rather than a demand issue
- Analyzed 3.51K orders totaling ₹122M in sales and ₹12.2M in profit (~10% margin)

## Dashboard
A 5-page interactive Power BI report covering:
1. Overview (map, KPIs, profit vs. sales, trend)
2. Top/Bottom 5 product analysis
3. Period-over-period comparison
4. Order-level detail table with filters
5. Category/discount analysis

See `outputs/ElectroHub_Sales_Dashboard.pdf` for a static preview, or open the `.pbix` file in Power BI Desktop for the interactive version.

## How to Run this Project
1. Clone or download this repository
2. Open `powerbi/sales_project.pbix` in Power BI Desktop
3. Click **Refresh** to reload data if needed
4. Navigate through the report pages using the tabs at the bottom
