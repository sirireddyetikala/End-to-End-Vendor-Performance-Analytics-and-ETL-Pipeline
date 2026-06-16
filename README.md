# End-to-End-Vendor-Performance-Analytics-and-ETL-Pipeline
# Vendor Performance Analysis Dashboard

An end-to-end data analytics project focused on evaluating vendor performance, optimizing inventory management, and improving profitability in the retail and wholesale industry.

The project combines data cleaning, business analysis, statistical validation, SQL-based data processing, and interactive dashboarding using Power BI.

---

## 📌 Business Problem

Retail and wholesale companies often face challenges related to:

* Vendor dependency risks
* Inefficient inventory turnover
* Poor pricing strategies
* Excess inventory carrying costs
* Lack of visibility into vendor profitability

This project aims to answer the following business questions:

* Which brands require promotional or pricing adjustments?
* Which vendors contribute the most to sales and purchases?
* How does bulk purchasing impact unit costs?
* Which vendors have low inventory turnover?
* Is there a significant difference in profitability between high-performing and low-performing vendors?

---

## 🎯 Objectives

* Identify underperforming brands with growth potential
* Analyze vendor contribution to overall purchases and profits
* Evaluate the impact of bulk purchasing on unit costs
* Detect slow-moving inventory and quantify unsold capital
* Compare profitability patterns across vendor segments
* Deliver actionable insights through an interactive Power BI dashboard

---

## 🛠️ Tech Stack

* **Programming Language:** Python
* **Libraries:** Pandas, NumPy, SQLAlchemy, SciPy
* **Database:** SQLite
* **Visualization:** Power BI
* **Development Environment:** Jupyter Notebook

---

## 📂 Project Structure

```text
├── data/
│   ├── raw_data/
│   └── processed_data/
│
├── notebooks/
│   └── Vendor Performance Analysis.ipynb
│
├── reports/
│   └── Vendor Performance Report.pdf
│
├── powerbi/
│   └── vendor_performance.pbix
│
├── screenshots/
│   ├── dashboard_overview.png
│   └── vendor_analysis.png
│
├── README.md
└── requirements.txt
```

---

## ⚙️ Project Workflow

```text
Raw Data
    ↓
Data Cleaning & Transformation (Python)
    ↓
SQLite Database
    ↓
Creation of vendor_sales_summary Table
    ↓
Import into Power BI
    ↓
Interactive Dashboard & Business Insights
```

---

## 🧹 Data Cleaning & Preparation

The dataset contained several inconsistencies and anomalies, including:

* Negative gross profit values
* Infinite or negative profit margins
* Products with zero sales quantity
* Extreme freight cost outliers
* Significant variations in product pricing

The following filters were applied to improve analysis quality:

* Gross Profit > 0
* Profit Margin > 0
* Total Sales Quantity > 0

---

## 📊 Key Metrics

* Total Sales
* Gross Profit
* Profit Margin (%)
* Purchase Quantity
* Sales Quantity
* Inventory Turnover
* Unsold Inventory Capital
* Vendor Contribution (%)
* Unit Cost

### Formula: Profit Margin

```text
Profit Margin = (Gross Profit / Total Sales) × 100
```

### Formula: Inventory Turnover

```text
Inventory Turnover = Total Sales Quantity / Total Purchase Quantity
```

---

## 📈 Key Insights

### Vendor Dependency Risk

* The top 10 vendors account for **65.69%** of total purchases.
* Heavy reliance on a few vendors increases supply chain risk.

### Bulk Purchasing Impact

* Bulk purchasing reduced unit costs by approximately **72%**.
* Average bulk purchase cost was around **$10.78 per unit**.

### High-Margin, Low-Sales Brands

* Identified **198 brands** with high profit margins but low sales volume.
* These brands represent opportunities for targeted promotions and pricing optimization.

### Inventory Optimization

* Approximately **$2.71 million** is tied up in unsold inventory.
* Slow-moving inventory increases holding costs and impacts cash flow.

### Vendor Profitability Analysis

* Low-performing vendors achieved higher average profit margins but generated lower sales volumes.
* High-performing vendors relied on volume-driven profitability strategies.
  
### Result

The null hypothesis was rejected, confirming statistically significant differences in vendor profitability models.

---

## 📌 Power BI Dashboard Features

* KPI Cards
* Vendor Ranking Analysis
* Inventory Turnover Tracking
* Profit Margin Comparison
* Interactive Filters and Slicers
* Drill-Down Capabilities
* Dynamic Vendor Performance Analysis

---

## 💡 Business Recommendations

* Diversify vendor partnerships to reduce dependency risks.
* Increase promotional efforts for high-margin, low-sales brands.
* Leverage bulk purchasing to improve cost efficiency.
* Optimize procurement for slow-moving inventory.
* Improve distribution strategies for underperforming vendors.
