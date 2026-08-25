# 📊 AtliQ Business Insights 360 — Power BI Dashboard

## 📌 Overview
This project is an interactive Power BI dashboard built for **AtliQ**, a simulated FMCG/CPG (fast-moving consumer goods) company, consolidating Finance, Sales, Marketing, and Supply Chain performance into a single business intelligence tool. It delivers a dynamic Profit & Loss statement that can be sliced by customer, product, market, or time period, alongside dedicated views for sales profitability, marketing performance, and supply chain forecast accuracy — enabling executives and analysts to explore business health from multiple angles in one report.

---

## 🗂️ Data Model

The report is built on a **star schema**:

| Table | Type | Description |
|---|---|---|
| `fact_actuals_estimates` | Fact | Core transactional table with gross sales, net invoice sales, net sales, and deduction amounts |
| `dim_customer` | Dimension | Customer name and market |
| `dim_product` | Dimension | Product, category, segment, and division |
| `dim_market` | Dimension | Market and region |
| `dim_date` | Dimension | Date, fiscal year, quarters, YTD/YTG flags |

A separate `Key Measures` table holds the DAX measures powering the KPIs across the report (Net Sales, Gross Margin, Net Profit, Forecast Accuracy, Net Error, and P&L calculations).

---

## 📄 Report Pages

| Page | Purpose |
|---|---|
| **Home** | Landing page with navigation to all views and a short guide to what each view offers |
| **P&L Check** | Dynamic Profit & Loss statement, filterable by customer, product, market, or time period |
| **Finance View** | Gross Margin, Net Profit, and P&L trends via KPI cards, pivot tables, and area charts |
| **Sales View** | Customer performance across Net Sales and Gross Margin, visualized in a profitability/growth matrix |
| **Marketing View** | Product performance across Net Sales and Gross Margin, visualized in a profitability/growth matrix |
| **Supply Chain View** | Forecast accuracy, Net Error, and risk profile by product, segment, category, and customer |

---

## 📐 Key Metrics (DAX Measures)

- **Net Sales ($)** — current period and prior-year (LY) comparison
- **Gross Margin ($ and %)** — current and LY comparison
- **Net Profit ($ and %)** — current and LY comparison
- **Forecast Accuracy (%)** — current and LY comparison
- **Net Error / ABS Error** — supply chain forecasting deviation
- **P&L Values** — dynamic Profit & Loss line items with YoY % change
- **Risk classification** — based on forecast error thresholds

---

## 📊 Visuals Used
KPI cards, dynamic pivot tables, area charts, donut charts, scatter charts (profitability/growth matrix), waterfall chart, combo line + clustered column chart, and interactive slicers for filtering by customer, product, market, and time period.

---

## 🛠️ Tools Used
- **Power BI Desktop** — data modeling, DAX measures, report design
- **DAX** — KPI calculations, time intelligence (LY comparisons, YoY %), dynamic P&L logic
- **Star Schema Data Modeling** — fact and dimension table design

---

## 🎯 Skills Demonstrated
- Star schema data modeling (fact & dimension tables)
- DAX measure creation (time intelligence, dynamic aggregations, error/risk metrics)
- Dynamic, filterable financial reporting (P&L statement)
- Multi-page executive dashboard design (Finance, Sales, Marketing, Supply Chain views)
- Data visualization best practices (KPI cards, matrices, trend and variance charts)

---

## 🚀 How to Use
1. Download `chapter-10-bi360.pbix`
2. Open in **Power BI Desktop**
3. Navigate through the Home page to explore Finance, Sales, Marketing, and Supply Chain views
4. Use the slicers on each page to filter by customer, product, market, or time period

---

## 🙋 About
This project was built as part of a hands-on Power BI learning exercise to demonstrate practical business intelligence skills — data modeling, DAX, and dashboard design — applied to a realistic FMCG business scenario spanning finance, sales, marketing, and supply chain analytics.
