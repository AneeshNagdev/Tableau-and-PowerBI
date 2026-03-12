# ☕ Coffee Shop Sales Dashboard – Tableau (Week 1)

This project is part of my Tableau learning journey. In this week's practice, I worked on building a sales dashboard in Tableau using a coffee shop transactional dataset. The purpose of this project was to understand how raw sales data can be transformed into useful business insights that support managerial strategy and decision-making.

## 📊 Dashboard Preview

![Coffee Shop Dashboard Screenshot](dashboard/tableau%20week1%20image.png)

## 🎯 Business Value & Objectives

The main objective of this dashboard was to create visualizations that help answer four important business questions:
1. **How is revenue changing over time?**
2. **Which product categories generate the most revenue?**
3. **Which products are performing best?**
4. **Which products are underperforming?**

These insights can support decisions related to inventory planning, menu strategy, promotions, pricing, and overall business performance monitoring.

## 📁 Dataset Overview

The dataset used in this project contains coffee shop transaction records. Each row represents a single product purchase made during a transaction. 

Key columns used in this project include:
*   `transaction_date`: Used to analyze revenue over time.
*   `product_category`: Used to compare categories such as coffee, tea, bakery, and drinking chocolate.
*   `product_detail`: Used to identify individual products.
*   `subtotal`: Used as the primary revenue metric across all charts, representing the value generated from each transaction.

Understanding and configuring the correct data types in Tableau (e.g., date for `transaction_date` and numeric for `subtotal`) was a crucial first step before building any visualizations.

## 📈 Project Workflow & Visualizations

The workflow started with importing the CSV dataset into Tableau Desktop and verifying field interpretations. I created individual worksheets for each required graph before assembling the final dashboard:

1. **Monthly Revenue (Line Chart):** Grouped `transaction_date` by month and calculated `SUM(subtotal)` to reveal seasonality, trends, and sales peaks.
2. **Revenue by Product Category (Horizontal Bar Chart):** Compared category revenue in descending order to immediately highlight the strongest-performing product groups.
3. **Top 5 Products (Filtered Bar Chart):** Applied a Top 5 filter based on revenue to identify the best-selling products that drive the business.
4. **Bottom 5 Products (Filtered Bar Chart):** Applied a Bottom 5 filter to highlight underperforming products that may need promotion, pricing review, or removal.
5. **Dashboard Design:** Combined all worksheets into a clean, unified layout using dashboard containers. A consistent color scheme was applied (e.g., positive colors for top performers, warning colors for underperformers) to make the dashboard visually intuitive.

## 🧠 What This Project Demonstrates

This project acts as a practical exercise reflecting a realistic business use case. It demonstrates my ability to take a raw dataset and convert it into a meaningful business dashboard, specifically highlighting skills in:
*   Working with transactional business data.
*   Aggregating revenue using `SUM()` and grouping date data.
*   Using Tableau to build multiple individual worksheets.
*   Applying effective filters (Top N/Bottom N) and sorting data.
*   Designing a dashboard for clear presentation and decision-making.

## 📂 Files Included in This Repository

*   `dataset/`: Contains the raw CSV data used for the analysis.
*   `dashboard/`: Contains the Tableau packaged workbook (`.twb` / `.twbx`) and the dashboard screenshot.
*   `README.md`: This documentation.

### 🌳 Repository Structure

```text
📦 coffee-shop-tableau-dashboard
┣ 📂 dashboard
┃ ┣ 📜 Tableau Week 1 Workbook.twb
┃ ┗ 📜 tableau week1 image.png
┣ 📂 dataset
┃ ┗ 📜 coffee_shop_sales.xlsx - Transactions.csv
┗ 📜 README.md
```
