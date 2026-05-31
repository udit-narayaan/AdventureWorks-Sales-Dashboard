# 📊 AdventureWorks Sales Performance Dashboard | Power BI

![Power BI](https://img.shields.io/badge/Power%20BI-Dashboard-yellow?style=flat-square&logo=powerbi)
![DAX](https://img.shields.io/badge/DAX-Data%20Modeling-orange?style=flat-square)
![Status](https://img.shields.io/badge/Status-Complete-green?style=flat-square)

## 📌 Project Overview

An end-to-end Power BI dashboard built for AdventureWorks Bike Shop — a fictional global cycling equipment retailer. The dashboard tracks **$24.9M revenue, $10.5M profit, 25.2K orders and a 2.2% return rate** across multiple years, product categories, and customer segments.

The goal was to design a professional, interactive reporting solution that gives business stakeholders a complete picture of sales performance — from high-level executive summaries down to individual product and customer-level insights.

🔗 **[View Live Dashboard](https://app.powerbi.com/view?r=eyJrIjoiZGZmNmVhNmMtMzNkMS00MjBhLWJjMGItZDhhNTFiOTcwNzQ3IiwidCI6ImUxNGU3M2ViLTUyNTEtNDM4OC04ZDY3LThmOWYyZTJkNWE0NiIsImMiOjEwfQ%3D%3D)**

---

## 🗂️ Dataset Structure

10 raw CSV files connected across a relational data model:

| Table | Description |
|---|---|
| `AdventureWorks_Sales_Data_2020` | Transaction-level sales records for 2020 |
| `AdventureWorks_Sales_Data_2021` | Transaction-level sales records for 2021 |
| `AdventureWorks_Sales_Data_2022` | Transaction-level sales records for 2022 |
| `AdventureWorks_Customer_Lookup` | Customer demographics and details |
| `AdventureWorks_Product_Lookup` | Product names, prices, and costs |
| `AdventureWorks_Product_Categories_Lookup` | Top-level product categories |
| `AdventureWorks_Product_Subcategories_Lookup` | Product subcategories |
| `AdventureWorks_Returns_Data` | Product return records |
| `AdventureWorks_Territory_Lookup` | Sales territory and regional data |
| `AdventureWorks_Calendar_Lookup` | Date table for time intelligence |

---

## 🔧 Tools Used

- **Power BI Desktop** — dashboard development
- **DAX** — calculated measures and KPIs
- **Power Query** — data transformation and cleaning
- **Data Modeling** — star schema with relationships across 10 tables

---

## 📋 Dashboard Pages

### 1. Executive Summary
![Executive Dashboard](Screenshots/01_Exec_Dashboard.png)

Tracks top-level KPIs including total revenue, profit, orders, and return rate. Includes a Top 10 product performance table with conditional formatting showing orders, revenue, and return % at a glance — designed for quick executive decision-making.

### 2. Geographic Map
![Map](Screenshots/02_map.png)

Interactive map visualising sales distribution across global territories, enabling regional performance comparison and identification of high and low performing markets.

### 3. Product Detail
![Product Detail](Screenshots/03_product_detail.png)

Deep-dive product analysis page featuring a what-if price adjustment parameter, target vs actual gauges for orders, revenue and profit, and dynamic metric selection — allowing stakeholders to model pricing scenarios and track performance against targets.

### 4. Customer Detail
![Customer Detail](Screenshots/04_customer_detail.png)

Customer segmentation analysis covering 17.4K unique customers broken down by income level, occupation, and revenue per customer trends — enabling targeted marketing and customer strategy decisions.

---

## 💡 What the Data Revealed

The dashboard was built to answer real business questions — here is what the analysis uncovered.

**Sales Performance:** Revenue grew consistently from 2020 through 2022, with the Bikes category driving the majority of total revenue. Accessories contributed the highest order volume but lowest revenue per unit — signalling a high-frequency, low-margin product line that benefits from bundling strategies.

**Product Reliability:** The 2.2% overall return rate masks significant variation at the product level. Certain products showed return rates exceeding 3% — a threshold that, when crossed at scale, represents a meaningful cost and customer satisfaction risk worth investigating at the manufacturing level.

**Customer Behaviour:** The top revenue-generating customers skew toward the Professional and Skilled Manual occupation segments with high income levels — suggesting AdventureWorks' premium pricing strategy resonates most with this demographic and should inform future customer acquisition targeting.

---

## 📊 DAX Measures Developed

- Total Revenue, Total Profit, Total Orders, Return Rate
- Revenue vs Target, Profit vs Target, Orders vs Target
- Month-over-month and year-over-year growth
- 90-day rolling revenue
- Customer lifetime value metrics
- Contribution % by product and category

---

## 📁 Project Structure

```
AdventureWorks-Sales-Dashboard/
│
├── 📂 Datasets/
│   ├── AdventureWorks_Calendar_Lookup.csv
│   ├── AdventureWorks_Customer_Lookup.csv
│   ├── AdventureWorks_Product_Categories_Lookup.csv
│   ├── AdventureWorks_Product_Lookup.csv
│   ├── AdventureWorks_Product_Subcategories_Lookup.csv
│   ├── AdventureWorks_Returns_Data.csv
│   ├── AdventureWorks_Sales_Data_2020.csv
│   ├── AdventureWorks_Sales_Data_2021.csv
│   ├── AdventureWorks_Sales_Data_2022.csv
│   └── AdventureWorks_Territory_Lookup.csv
│
├── 📂 Screenshots/
│   ├── 01_Exec_Dashboard.png
│   ├── 02_map.png
│   ├── 03_product_detail.png
│   └── 04_customer_detail.png
│
├── 📄 AdventureWorks_Sales_Dashboard.pbix
└── 📄 README.md
```

---

## 🚀 How to Run

1. Clone this repository
   ```bash
   git clone https://github.com/udit-narayaan/AdventureWorks-Sales-Dashboard.git
   ```

2. Open `AdventureWorks_Sales_Dashboard.pbix` in Power BI Desktop

3. If data doesn't load automatically, go to **Transform Data → Data Source Settings** and point to the `Datasets/` folder

4. Or view the live interactive dashboard directly via the link above — no Power BI installation needed

---

## 👤 Author

**Udit Narayan** — BBA Graduate | Data Analyst

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue?style=flat-square&logo=linkedin)](https://www.linkedin.com/in/udit-narayan-7902aa293/)
[![GitHub](https://img.shields.io/badge/GitHub-Follow-black?style=flat-square&logo=github)](https://github.com/udit-narayaan)
