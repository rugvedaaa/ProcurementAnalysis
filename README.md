# 📦 Procurement Analysis Dashboard | Power BI Project

## 👋 Introduction

Welcome! This is a Power BI dashboard project focused on analyzing procurement data across multiple dimensions—purchase orders, suppliers, product categories, buying patterns, and more. The goal of this project was to transform raw procurement records into meaningful insights that can help businesses make data-driven decisions around sourcing and purchasing.

I created this report to explore trends in purchase volumes, identify top suppliers, and evaluate spending behavior across years and categories. It uses various Power BI features including DAX, slicers, drill-through pages, and tooltips to build an interactive, insightful, and user-friendly dashboard.

---

## 🎯 Project Objectives

- Track total purchase volume and value over time.
- Analyze supplier performance based on quantity and spend.
- Understand procurement behavior by packaging types and categories.
- Drill into specific suppliers or items to get detailed insights.
- Deliver insights in a clean, intuitive, and interactive dashboard layout.

---

## 🛠 Tools & Technologies Used

- **Power BI Desktop** – for building interactive visualizations and data models.
- **DAX (Data Analysis Expressions)** – used extensively to create calculated columns and measures like:
  - Total Final PO
  - YOY % Increase in Purchases
  - Categorized Supplier Contribution
- **Power Query Editor** – for cleaning, shaping, and transforming the raw data.
- **Excel** – used as the primary data source for procurement records.

---

## 📊 Dashboard Pages Overview

### 🔹 1. Procurement Analysis (Main Page)

This is the landing page with a snapshot of overall procurement activity.

**Key features:**
- KPI cards for:
  - Total Quantity (135M)
  - Total Purchases ($2.08B)
  - Total POs (6,553)
- Year range slicer to dynamically adjust the visuals.
- Bar charts for:
  - POs by Buying and Selling Package (e.g., Carton, Each)
  - POs by Year
- Donut chart showing distribution of POs by supplier category.
- Narrative insights (auto-updated based on filters) highlighting:
  - Purchase growth trends
  - Supplier contributions
  - Peak procurement years

---

### 🔹 2. Tooltip Page (Hover Insight)

This tooltip page is triggered when hovering over certain visuals in the main dashboard.

**Purpose:**
To give quick item-level breakdowns without the need to navigate away from the main view.

**Contains:**
- Table with Top 10 Stock Items based on:
  - Total Purchases
  - Total Quantity
  - Number of POs

---

### 🔹 3. Detailed Page (Drill-through)

This is where the **Drill-through functionality** comes into play.

**How it works:**
When a user right-clicks on a supplier or item in the main dashboard and selects “Drill through,” they land on this page.

**What's here:**
- A detailed table showing:
  - Supplier Name
  - Contact
  - Stock Item
  - Buying Package
  - Purchase value, Quantity, and PO count
- Date slicer is scoped to the year selected (example: 2016)
- This page is great for **deep-dives** when analyzing individual supplier/item performance.

---

## 📌 Key Insights Derived

- Purchases increased by **704%** between 2013 and 2016.
- Quantity grew by **822%** over the same period.
- **2016** was the highest procurement year with over **$536M** in spend.
- Most purchases came in **Carton** packaging.
- **Fabrikam, Inc.** and **A. Datum Corporation** are top suppliers by value and PO count.
- Clothing suppliers contributed to over **68%** of POs.
- The item **"The Gu" red shirt XML tag t-shirt** was a top purchase across several sizes.

---

## 📈 DAX Highlights

DAX was used throughout the project for calculating custom metrics and performing time-based calculations. A few examples include:

- `Total Final PO = CALCULATE(COUNTROWS('Table'), 'Table'[Status] = "Final")`
- YOY growth calculations for both purchase value and quantity.
- Percentage breakdowns for supplier categories and packaging types.

---

## 🔄 Interactive Features

- **Date Slicers** – Filter the entire dashboard based on year/month.
- **Drill-through** – Navigate from overview charts directly to detailed supplier/item views.
- **Tooltips** – Hover-based insights to view top stock items instantly.
- **Dynamic Commentary** – Auto-updating text box with narrative insights.

---

## 📂 File Structure

📦 Procurement-Analysis
┣ 📁 Screenshots
┃ ┣ PA1.png
┃ ┣ PA2.png
┃ ┣ PA3.png
┣ Procurement_Analysis.pbix
┣ README.md



---

## 💡 What I Learned

- The power of drill-throughs in enhancing dashboard storytelling.
- How to clean and model procurement data for analytical consumption.
- Building dynamic visuals that update with filters.
- Writing DAX measures that support real-world use cases like year-on-year analysis and segmentation.

---

## ✅ Future Improvements

- Add cost-saving opportunity detection.
- Integrate supplier performance KPIs (like delivery lead times).
- Create scenario forecasting using What-If Parameters.
- Add role-level security for different stakeholder views (finance, ops, etc.).

---

## 🙌 Thanks for checking this out!

If you found this project interesting or have feedback, feel free to reach out. I’m always open to collaboration and learning from the community.

