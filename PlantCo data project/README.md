# 🌿 PlantCo Sales Performance Dashboard  

📊 **Power BI | Data Analytics | Business Intelligence**  

![Capture d'écran 2025-02-12 150603](https://github.com/user-attachments/assets/0831c804-934d-46ea-aeaa-3f3157339229)


## 📌 Executive Summary
PlantCo, a global distributor of indoor and landscape plants, faced challenges in tracking real-time profitability across its international markets. This project deliver a high-performance **Power BI solution** that compares **Year-To-Date (YTD)** performance against the **Previous Year-To-Date (PYTD)**. 

The dashboard empowers stakeholders to identify underperforming countries, optimize product mix (Indoor vs. Outdoor), and segment accounts based on their contribution to Gross Profit.

---

## 🛠️ Tech Stack & Advanced Skills
* **Tool:** Power BI Desktop
* **Modeling:** Star Schema with Fact (Sales) and Dimension (Accounts, Hierarchy, Date) tables.
* **DAX Excellence:** * **Time Intelligence:** Complex YTD, PYTD, and SPLY (Same Period Last Year) calculations.
    * **Dynamic Measures:** Switching between Sales, Quantity, and Gross Profit.
    * **Segmentation:** Account Profitability grouping based on GP% thresholds.
* **ETL:** Power Query for data cleansing and normalization of global account IDs.

---

## 🔍 Business Insights & Problem Solving

### 1. The Profitability Leak (YTD vs PYTD)
* **The Observation:** Total Gross Profit stands at **$13.00M**, showing a decline of **-$512.26K** compared to the previous year.
* **Deep Dive:** Analysis reveals that **China** is the primary driver of this decline with a **-$760.40K** drop in performance.
* **Solution:** I implemented a "Bottom 10" waterfall chart to isolate exactly which countries and months are dragging down global margins, allowing for targeted regional interventions.

### 2. Product Mix Optimization
* **The Observation:** Not all plant types are equal. "Indoor" plants show different seasonal velocity compared to "Landscape" products.
* **Insight:** Landscape products often have higher volume but lower GP% compared to specialized Indoor plants.
* **Solution:** The dashboard includes an **Account Profitability Segmentation** scatter plot. This helps marketing teams focus on high-margin accounts rather than just high-volume ones.

### 3. Account Segmentation Strategy
* **The Problem:** Marketing resources were being spread thin across all clients.
* **Solution:** I developed a **GP% vs. Sales** matrix. This segments customers into:
    * **Top Tier:** High Sales / High Margin (Protect & Grow).
    * **Underperformers:** High Sales / Low Margin (Negotiate price or reduce support).

---

## 🧠 Key DAX Formulas Used

**Year-To-Date (YTD) Calculation**
```dax
Sales YTD = TOTALYTD(SUM('Plant_Fact'[Sales_USD]), 'Date'[Date])
```

**Year-Over-Year Variance**
```dax
YTD vs PYTD = [Sales YTD] - [Sales PYTD]
```

**Gross Profit Percentage (GP%)**
```dax
GP % = DIVIDE([Gross Profit], [Sales_USD], 0)
```
---

## 📂 Project Structure
* `Plant Co Performance Report.pbix`: The primary Power BI report.
* `Data/Plant_DTS.xlx`: The raw dataset used for analysis.
* `Assets/Plant Co Performance Report.pdf`: The pdf version of the dashboard.
* `Readme.md`: The Readme.

---

## 👤 Contact & Links
**[Famous SOUNTON]** - Data Analyst
* [LinkedIn Profile](https://www.linkedin.com/in/famoussounton)
* [Portfolio Website](https://www.datascienceportfol.io/sounntonfamous)
* **Email:** sountonfamous@gmail.com
