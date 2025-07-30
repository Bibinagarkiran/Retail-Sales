# Retail Sales Performance Dashboard – Power BI

## Overview
An interactive Power BI dashboard designed to visualize and analyze **retail sales data** across different product categories, customer segments, and regions. This report helps businesses understand trends, monitor KPIs, and make informed decisions.

---

## Project Files

- `RetailSalesPerformance.pbix` – Power BI dashboard file  
- `sales_data.csv` – Raw sales transaction data  
- `calendar.csv` – Calendar table for time intelligence  
- `background.png` – Custom background used in the dashboard  
- `README.md` – Project documentation (this file)

---

## Objectives

- Track **Total Sales**, **Average Order Value**, and **Total Orders**
- Analyze sales by **Category**, **Sub-Category**, and **Region**
- Visualize **Monthly Sales Trends** using a Line Chart
- Drill into customer segments for targeted insights

---

## Key Visuals

| Visual                        | Description                                 |
|------------------------------|---------------------------------------------|
| **KPI Cards**                | Total Sales, Avg. Order Value, Orders       |
| **Bar Chart by Category**     | Compare sales across product categories     |
| **Bar Chart by Sub-Category** | Deep dive into detailed product types       |
| **Sales by Region Map**       | Geographical visualization of sales         |
| **Line Chart (Sales MOM)**    | Month-over-month sales trend                |
| **Slicers**                   | Region & Customer Segment filters           |

---

## Tools & Techniques

- **Power Query**: Data cleaning, transformation (split columns, remove nulls)
- **DAX Measures**:
  - `Total Sales = SUM(Sales[SalesAmount])`
  - `Avg Order Value = DIVIDE([Total Sales], COUNT(Sales[OrderID]))`
  - `Orders = COUNT(Sales[OrderID])`
- **Modeling**: Star schema; Calendar table with relationship to `OrderDate`
- **Design**: Custom canvas background with a modern dashboard layout

---

## Calendar Table Usage

- Used for accurate time-based reporting (e.g., MOM trends)
- Marked as **Date Table** in Power BI
- Joined with `Order Date` column in Sales data

---

## Insights

- Top-performing product: **Men (subcategory)**
- Highest sales region: **East**
- Noticeable drop in sales: **September**
- Highest MOM spike: **April**

---

## Outcome

This project demonstrates how to:
- Design a clean, performance-optimized dashboard
- Apply Power BI best practices (query folding, DAX measures, relationships)
- Deliver actionable insights from raw retail data

---
