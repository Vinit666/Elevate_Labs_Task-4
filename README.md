# 📊 Task 3 – Dashboard Design | Data Analyst Internship

## 📝 Task Objective

Design an interactive dashboard for business stakeholders using a Sales/Financial dataset. The goal is to create a user-friendly visual report with key KPIs, interactivity, and time-series analysis that can inform real business decisions.

---

## 📁 Dataset Used
- **Name:** Superstore Sales (Excel format)​
- **Source:** GitHub (https://github.com/PacktPublishing/Tableau-10-Best-Practices/blob/master/Chapter%205/Sample%20-%20Superstore%20Sales%20%28Excel%29.xls)
- **File Format:** Excel (` Sample - Superstore Sales (Excel).xls`)

---

## 🛠 Tools & Skills Applied
- Microsoft Power BI
- DAX (Data Analysis Expressions)
- Data modeling and transformation
- Visual storytelling and report design

---

## 🎯 Dashboard Summary

The dashboard was created with two interactive pages:

---

### 🔹 Page 1: Overview Dashboard

**Purpose:** Provide a high-level summary of overall business performance.

**Visuals Included:**
- **KPI Cards**:
  - ✅ Total Sales: 14.92M
  - ✅ Total Profit: 1.52M
  - ✅ Profit Margin: 10%
  - ✅ Total Orders: 5,496
- **Line Chart**: Sales & Profit trend over the years
- **Pie Chart**: Sales distribution by Customer Segment
- **Slicers/Filters**: Year, Month, Product Category, Region, Segment

---

### 🔹 Page 2: Regional Sales & Profit Analysis

**Purpose:** Break down performance across regions to identify top/bottom performers.

**Visuals Included:**
- **Clustered Bar Chart**:
  - Regions compared by Total Sales and Total Profit
- **Navigation Button**: Allows switching between pages

---

## 🧮 DAX Measures Created
```DAX
Total Sales = SUM(Orders[Sales])
Total Profit = SUM(Orders[Profit])
Profit Margin = DIVIDE([Total Profit], [Total Sales])
Total Orders = DISTINCTCOUNT(Orders[Order ID])
