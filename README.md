# 📊 Financial Performance & Operations Dashboard

An interactive executive dashboard built in **Power BI** to analyze enterprise financial performance, sales trends, geographic distribution, and discounting strategies using standard corporate financial datasets.

---

## 📌 Project Overview
This project transforms raw transactional data into actionable financial insights. The dashboard provides executives and financial analysts with a high-level overview of revenue, net profitability, product performance, and customer segment dynamics while allowing deep-dive exploration via dynamic slicers.

---

## 🔑 Key Metrics & Performance Summary
* **Total Sales:** $118.73M
* **Total Profit:** $16.89M
* **Profit Margin:** 14.23%
* **Total COGS:** $101.83M
* **Total Units Sold:** 1.13M units

---

## 💡 Key Business Insights

1. **High Manufacturing Cost Structure:** COGS represents ~85.7% ($101.83M) of total revenue ($118.73M), highlighting that profitability is heavily sensitive to production and operational costs.
2. **Q4 Seasonality Surge:** Sales peak significantly in Q4 (reaching over $20M in December alone) compared to a steady $5M–$7M monthly baseline during earlier quarters.
3. **Customer Segment Concentration:** **Government (44.2%)** and **Small Business (35.7%)** combined drive nearly **80%** of total segment sales, presenting a potential concentration risk.
4. **Product Flagship Performance:** **Paseo** is the top revenue generator (~$33M), significantly outperforming secondary offerings like Carretera ($14M).
5. **Discount Strategy Impact:** High discount bands drive considerable volume (398K units) but erode net profit margins—indicating a need for tighter promotional guardrails.

---

## 🛠 Tech Stack & Tools
* **Business Intelligence & Data Visualization:** Power BI Desktop
* **Data Transformation & ETL:** Power Query (Data cleaning, whitespace trimming, typing)
* **Data Modeling & Analytics:** DAX (Data Analysis Expressions)

---

## ⚙️ Data Pipeline & Transformation Workflow

1. **Power Query ETL:**
   * Cleaned header whitespace across all columns (including leading space in `Sales`).
   * Validated column types (Fixed Decimal for financial figures, Whole Number for volume counts, Date for timeline attributes).
2. **DAX Measures Created:**
   * `Total Sales = SUM(financials[Sales])`
   * `Total Profit = SUM(financials[Profit])`
   * `Total COGS = SUM(financials[COGS])`
   * `Total Units Sold = SUM(financials[Units Sold])`
   * `Profit Margin % = DIVIDE([Total Profit], [Total Sales], 0)`

---

## 🖼 Dashboard Preview

---

## 🚀 How to Run / View
1. Clone this repository:
   ```bash
   git clone [https://github.com/your-username/your-repo-name.git](https://github.com/your-username/your-repo-name.git)
