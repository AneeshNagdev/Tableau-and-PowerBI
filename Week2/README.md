# 📊 Sales & Profit Dashboard – Tableau (Week 2)

Welcome to Week 2 of my Tableau learning journey! This week, I focused on building an interactive **Sales and Profit Dashboard** using the classic Superstore dataset. 

The primary goal of this project was to practice building multiple specialized Tableau worksheets, combining them into a comprehensive dashboard, and implementing filters and interactivity to allow users to explore the data dynamically.

## 🌟 Dashboard Preview

![Sales & Profit Dashboard Screenshot](dashboard/Tableau%20Week2%20Image.png)

## 📁 Dataset Overview

The dataset used in this project is the **Superstore dataset**, which contains retail sales records. Each row represents a specific product purchased within a customer order.

**Key fields utilized:**
* **`Order Date`** – Used for time-based trend analysis.
* **`Sales`** – The revenue generated from each order.
* **`Profit`** – The profit earned or lost from each sale.
* **`Category` & `Sub-Category`** – High-level and detailed product classifications.
* **`Region`** – The geographic sales region.
* **`Product Name`** – The individual product identifier.

*Note: Before creating any charts, the dataset was imported into Tableau and data types were verified (e.g., ensuring `Order Date` was properly interpreted as a date field).*

---

## 🛠️ Step-by-Step Tutorial: How I Built the Visualizations

Each visualization was constructed in its own distinct worksheet before being assembled into the final dashboard. Here is exactly how I built each one:

### 1️⃣ Sales Trend (Line Chart)
*This visualization shows how sales change over time and compares two different years.*

**Steps:**
1. Drag **`Order Date`** to the *Columns* shelf.
2. Change the date level to **`MONTH(Order Date)`**.
3. Drag **`Sales`** to the *Rows* shelf.
4. Ensure the aggregation is set to **`SUM(Sales)`**.
5. Change the *Marks* type to **Line**.
6. Drag **`YEAR(Order Date)`** to the *Color* shelf to differentiate the years.
7. Add a filter for **`YEAR(Order Date)`** and select only `2016` and `2017`.
8. Enable labels for the line ends so the chart clearly displays `2016` and `2017` at the end of each respective line.

### 2️⃣ Sales by Category (Bar Chart)
*This chart compares how much revenue each major product category generates.*

**Steps:**
1. Drag **`Category`** to the *Columns* shelf.
2. Drag **`Sales`** to the *Rows* shelf.
3. Ensure the measure is **`SUM(Sales)`**.
4. Change the *Marks* type to **Bar**.
5. Drag **`Category`** to the *Color* shelf to create a visual legend.
6. Drag **`Sales`** to the *Label* shelf so the exact total values appear on each bar.
7. Sort the bars in **descending order** so the highest sales appear first.

### 3️⃣ Profit by Sub-Category (Horizontal Bar Chart)
*Shows which product groups are profitable and which generate losses using a distinct color scale.*

**Steps:**
1. Drag **`Sub-Category`** to the *Rows* shelf.
2. Drag **`Profit`** to the *Columns* shelf.
3. Ensure the aggregation is **`SUM(Profit)`**.
4. Change the *Marks* type to **Bar**.
5. Drag **`Profit`** to the *Color* shelf.
6. Edit the color palette to use a **Red–Green diverging scale**.
7. Set `0` as the center value, so:
   * 🟩 **Green** represents profit.
   * 🟥 **Red** represents losses.
8. Drag **`Profit`** to the *Label* shelf to display exact profit/loss values.
9. Sort the chart so the highest profit appears first.

### 4️⃣ Sales by Region (Bar Chart)
*Compares revenue across geographic regions and acts as a dynamic filter for the dashboard.*

**Steps:**
1. Drag **`Region`** to the *Columns* shelf.
2. Drag **`Sales`** to the *Rows* shelf.
3. Ensure the measure is **`SUM(Sales)`**.
4. Change the *Marks* type to **Bar**.
5. Drag **`Region`** to the *Color* shelf.
6. Drag **`Sales`** to the *Label* shelf.

### 5️⃣ Top 10 Products by Sales (Filtered Bar Chart)
*Highlights the highest-revenue individual products.*

**Steps:**
1. Drag **`Product Name`** to the *Rows* shelf.
2. Drag **`Sales`** to the *Columns* shelf.
3. Ensure the aggregation is **`SUM(Sales)`**.
4. Sort the chart in **descending order**.
5. Apply a filter on **`Product Name`**:
   * Select **Top**.
   * Choose **Top 10 by SUM(Sales)**.
6. Drag **`Category`** to the *Color* shelf.
7. Drag **`Sales`** to the *Label* shelf.

---

## 🧩 Assembling the Interactive Dashboard

After creating the individual worksheets, I combined them into a single, cohesive Tableau dashboard.

**Steps to assemble:**
1. Create a new dashboard and set an appropriate size.
2. Add a prominent dashboard title: **Sales & Profit Dashboard**.
3. Arrange the worksheets in a structured layout.
4. Add global filters to the dashboard for **Region** and **Category**.
5. Configure the **Sales by Region** chart to act as a dynamic visual filter by enabling **Use as Filter**. 
   * *Result:* Users can click a specific region on this chart, and all other charts instantly update to reflect only that region's data.

---

## 🧠 Skills Practiced

Through this project, I successfully practiced several core Tableau concepts:
* Building multiple linked worksheets from a single dataset.
* Aggregating data using `SUM()` measures and level-of-detail date fields.
* Creating and formatting line charts and bar charts.
* Applying sophisticated filters and performing Top-N analysis.
* Using custom divergent color scales (Red/Green) to highlight profitability intuitively.
* Designing interactive dashboards with clear, usable structures.
* Implementing chart-as-filter functionality for dynamic data exploration.

---

## 🌳 Repository Structure

```text
📦 sales-profit-tableau-dashboard
┣ 📂 dashboard
┃ ┣ 📜 Tableau Week 2 Workbook.twb
┃ ┗ 📜 Tableau Week2 Image.png
┣ 📂 dataset
┃ ┗ 📜 superstore_dataset.csv
┗ 📜 README.md
```
