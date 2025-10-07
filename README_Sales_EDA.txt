
# 📊 Sales Performance Analysis - Excel EDA Project

## 🧭 Project Overview
This Excel project explores retail sales data to uncover insights into revenue trends, product performance, and regional sales distribution over six months (April–September 2025).

---

## 🗂️ Dataset Description
The dataset contains daily sales transactions for a small retail business.

**Columns:**
- **Date:** Date of the transaction
- **Region:** Sales region (North, South, East, West)
- **Product:** Product name
- **Category:** Product category (Electronics, Appliances, Furniture)
- **Units Sold:** Number of items sold
- **Unit Price:** Price per item (USD)
- **Total Revenue:** Units Sold × Unit Price
- **Sales Rep:** Sales representative responsible
- **Month:** Month abbreviation (for grouping)

---

## ⚙️ Step-by-Step EDA Process in Excel

### 1️⃣ Data Cleaning
1. Open the file `sales_performance_EDA.xlsx`.
2. On the **Sales_Data** sheet:
   - Use **Data → Remove Duplicates** to remove any repeated entries.
   - Fill or remove blank cells if any appear.
   - Ensure numeric columns (`Units Sold`, `Unit Price`, `Total Revenue`) have correct data types.

---

### 2️⃣ Add Calculated Columns (if needed)
- Add or verify `Total Revenue` using `=E2*F2`.
- Add a `Month` column using `=TEXT(A2, "mmm")` for grouping by month.

---

### 3️⃣ Descriptive Statistics
Use Excel formulas to summarize data:
- **Average Revenue:** `=AVERAGE(G:G)`
- **Max Revenue:** `=MAX(G:G)`
- **Min Revenue:** `=MIN(G:G)`
- **Standard Deviation:** `=STDEV.P(G:G)`

Create a small statistics table to display these values.

---

### 4️⃣ Pivot Table Analysis
Use **Insert → PivotTable** to explore patterns:

#### Pivot 1: Revenue by Region
- Rows: Region  
- Values: SUM of Total Revenue  

#### Pivot 2: Top Products by Sales
- Rows: Product  
- Values: SUM of Total Revenue  
- Sort descending to find top sellers  

#### Pivot 3: Monthly Sales Trend
- Rows: Month  
- Values: SUM of Total Revenue  

---

### 5️⃣ Data Visualization
Use **Insert → Chart** to visualize your insights:

- **Column Chart:** Monthly sales trend  
- **Pie Chart:** Revenue share by region  
- **Bar Chart:** Top 5 products by revenue  

Apply **conditional formatting** to highlight best-performing products or regions.

---

### 6️⃣ Summary of Insights
Write your findings in a new sheet named **Insights**.

Example summary:
> - The **North** region achieved the highest total revenue.  
> - **Electronics** contributed ~60% of all sales.  
> - Sales peaked in **July** due to strong laptop sales.  
> - Average daily revenue was consistent, with a few high-performance days.

---

## 🧩 Optional Add-ons
- Add slicers to pivot tables for interactive filtering (e.g., by Region or Month).  
- Create a Dashboard sheet summarizing key metrics:
  - Total Revenue
  - Average Units Sold
  - Top 3 Products
  - Monthly Trend Chart

---

## ✅ Deliverables
- `sales_performance_EDA.xlsx` — dataset file  
- `README.txt` — this guide with project steps and notes

---

## 📅 Author & Purpose
Created for educational purposes to practice **Exploratory Data Analysis (EDA)** in Microsoft Excel using simulated retail sales data.
