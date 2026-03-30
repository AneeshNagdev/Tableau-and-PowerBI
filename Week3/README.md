# 📊 Store Pricing Dashboard – Power BI (Week 3)

Welcome to Week 3 of my data visualization learning journey! This week, I focused on building a simple and clean **Store Pricing Dashboard** using Power BI.

The objective of this project was to understand how product prices vary across different stores and over time, and to practice creating multiple visualizations within Power BI while applying proper data formatting and layout design.

---

## 🌟 Dashboard Preview

![Store Pricing Dashboard Screenshot](dashboard/powerbi_week3_image.png)

---

## 📁 Dataset Overview

The dataset used in this project is a **store pricing dataset**, where each row represents the price of a product at a specific store on a given date.

**Key fields utilized:**
* **`Store`** – The retail store (Walmart, Costco, Target).
* **`Product`** – The product being sold (Rice).
* **`Price`** – The price of the product.
* **`Date`** – The date of the recorded price.

*Note: Before creating any visuals, the dataset was loaded into Power BI and data types were verified (ensuring `Price` was numeric and `Date` was properly formatted as a date field).*

---

## 🛠️ Step-by-Step Tutorial: How I Built the Visualizations

All visualizations were created directly on the Power BI canvas and arranged into a structured dashboard layout.

### 1️⃣ Average Product Price (Column Chart)
*This visualization shows the average price of the product across all stores.*

**Steps:**
1. Select the **Clustered Column Chart** visual.
2. Drag **`Product`** to the *X-axis*.
3. Drag **`Price`** to the *Y-axis*.
4. Change aggregation from *Sum* to **Average**.
5. Enable **Data Labels** for better readability.
6. Rename the chart title to **Average Product Price**.

### 2️⃣ Price Comparison by Store (Bar Chart)
*This chart compares the price of the product across different stores.*

**Steps:**
1. Select the **Bar Chart** visual.
2. Drag **`Store`** to the *Y-axis*.
3. Drag **`Price`** to the *X-axis*.
4. Keep aggregation as **Price** (or Average if required).
5. Enable **Data Labels** to display exact values.
6. Rename the chart title to **Price Comparison by Store**.

### 3️⃣ Price Trend Over Time (Line Chart)
*This visualization shows how product prices vary over time across different stores.*

**Steps:**
1. Select the **Line Chart** visual.
2. Drag **`Date`** to the *X-axis*.
3. Drag **`Price`** to the *Y-axis*.
4. Change aggregation to **Average Price**.
5. Drag **`Store`** to the *Legend* to differentiate stores.
6. Enable **Markers** and **Data Labels** for clarity.
7. Rename the chart title to **Price Trend Over Time**.

---

## 🧩 Dashboard Design & Layout

After creating the visuals, I arranged them into a clean and professional dashboard layout.

**Steps to organize:**
1. Add a dashboard title using a text box: **🛒 Store Pricing Analysis Dashboard**.
2. Place visuals in a structured layout:
   * **Top left** → Average Product Price
   * **Top right** → Price Comparison by Store
   * **Bottom (full width)** → Price Trend Over Time
3. Apply a consistent color scheme:
   * **Walmart** → 🟦 Blue
   * **Costco** → 🟩 Green
   * **Target** → 🟥 Red
4. Adjust spacing, alignment, and sizing for readability.

---

## 🧠 Skills Practiced

Through this project, I practiced several key Power BI concepts:
* Importing data from Excel into Power BI.
* Verifying and correcting data types.
* Using different visual types (column, bar, line charts).
* Applying correct aggregations such as **Average**.
* Using legends to compare categories (stores).
* Designing clean and structured dashboards.
* Enhancing visuals with labels, titles, and formatting.

---

## 🌳 Repository Structure

```text
📦 store-pricing-powerbi-dashboard
┣ 📂 dashboard
┃ ┗ 📜 powerbi_week3_image.png
┣ 📂 dataset
┃ ┗ 📜 store_pricing.xlsx
┗ 📜 README.md
```

---

## 🚀 Reflection

This project helped me understand how even a small dataset can be used to generate meaningful insights through proper visualization techniques. It also strengthened my ability to design dashboards that are not only informative but also visually clear and structured.
