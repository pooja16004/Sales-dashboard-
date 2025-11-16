# 📈 Superstore Sales & Profitability Analysis Dashboard

## 🎯 Project Overview

This Power BI dashboard provides a comprehensive analysis of the Superstore's sales, profitability, and operational efficiency across various product categories, customer segments, and geographic regions. The primary goal is to **identify low-profit areas, track key performance indicators (KPIs), and inform strategic decisions** to maximize the overall profit ratio.

## ✨ Key Features & Insights

The dashboard is structured into three main sections to allow for top-down analysis:

### 1. Executive Summary (KPIs)

* **Total Sales & Total Profit:** High-level performance tracking.
* **Profit Ratio:** Measures operational efficiency (Profit / Sales), revealing how effectively revenue is converted to profit. (Calculated as **12.47%** overall in this project).
* **Return Rate %:** Measures operational efficiency and product quality. (Calculated as **2.96%** of total orders).
* **Year-over-Year (YoY) Growth:** [Add this KPI later: e.g., Sales are up 5.2% YoY].

### 2. Trends and Geography

* **Sales & Profit Trend:** Monthly view to identify seasonality and long-term growth patterns.
* **Geographic Analysis:** Map visualization highlighting high-selling regions and states with poor profit margins.

### 3. Root Cause Analysis

* **Profitability by Sub-Category:** Identifies specific products (e.g., Tables, Supplies) contributing to negative profit or low margins—critical for pricing and inventory decisions.
* **Returned Order Detail:** A filtered table showing individual returned orders, profits, and regions to analyze high-cost returns.

## 🔗 Data Sources

This project uses the well-known **Sample Superstore Sales Dataset** for demonstration and educational purposes.

* **Source File:** `Sample - Superstore.xls`
* **Download Link:** [https://community.tableau.com/s/question/0D54T00000CWeX8SAL/sample-superstore-sales-excelxls](https://community.tableau.com/s/question/0D54T00000CWeX8SAL/sample-superstore-sales-excelxls)

The three tables loaded into Power BI are:

1.  `Orders`: Contains all sales transaction details.
2.  `Returns`: A separate table listing only the `Order ID`s that were returned.
3.  `People`: Maps `Region` to the responsible `Regional Manager`.

## ⚙️ Technical Details & Skills

* **Tool:** Microsoft Power BI Desktop
* **Data Modeling:** Established **Many-to-One** relationships between Orders, Returns, and People tables.
* **Advanced DAX:** Creation of complex measures to derive actionable KPIs:
    * `Profit Ratio % = DIVIDE(SUM(Profit), SUM(Sales))`
    * `Return Rate %`: Calculated by linking the Orders and Returns tables.
    * Implicit Measures for Time Intelligence (e.g., YoY).
* **Data Transformation (Power Query):** Cleaning and shaping the imported CSV files (e.g., handling date formats).

## 💡 Learnings & Next Steps

* **Key Insight:** The `Technology` category drives the highest sales but the `Office Supplies` category yields a better **Profit Ratio** due to lower discounts.
* **Future Enhancements:** Implement a **What-If Parameter** to model the impact of different discount strategies on the final Profit Ratio.

---
