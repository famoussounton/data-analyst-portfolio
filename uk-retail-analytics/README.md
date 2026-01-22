# 🚀 UK Retail Strategy: Demand & Inventory Optimizer
<img width="1470" height="956" alt="Page 1" src="https://github.com/user-attachments/assets/14db52e0-84f8-4f31-8b80-10a007e6c7bb" />

## 📌 Business Overview
In the competitive UK retail landscape, balancing supply with fluctuating demand is critical for maintaining profitability. This project analyzes **6 years of retail data (2017-2023)** to move beyond basic reporting and provide **actionable business intelligence**.

By connecting sales trends, pricing competitiveness, and inventory logistics, this dashboard identifies key operational bottlenecks and proposes data-driven strategies to recover declining growth and optimize stock levels.

---

## 🛠️ Tech Stack & Methodology
* **Tool:** Power BI Desktop
* **ETL:** Power Query for data cleaning and normalization.
* **Analysis:** DAX (Data Analysis Expressions) for complex measures (YoY Growth, Forecast Bias, Stock Health).
* **Modeling:** Star Schema architecture for optimized report performance.

---

## 🔍 Problem Statement & Data Observations

### 1. The Revenue Challenge
* **Observation:** The dashboard shows a **Total Net Revenue of €24.69M**, but a concerning **YoY Growth of -23.01%**.
* **Analysis:** Revenue is heavily concentrated in the "Homeware" and "DIY" categories. However, high regional rent indices in "Central" and "East" areas are compressing net margins.
* **Proposed Solution:** Implement a regional pricing strategy that adjusts discounts based on the local **Retail Rent Index** to protect profitability in expensive urban zones.

### 2. Supply Chain Inefficiency
* **Observation:** The current **Forecast Accuracy is 64.06%**, indicating a significant mismatch between predicted and actual demand.
* **Analysis:** There are currently **91 products at "Stockout Risk"**, while other categories show excessive "Weeks of Coverage" (over-stocking).
* **Proposed Solution:** Transition from static ordering to a **Dynamic Replenishment Model**. Use the "Stock Health Score" (Critical/Optimal) to trigger internal stock transfers between regions (e.g., moving surplus from North to West).

---

## 📊 Key Insights & Business Impact

| Metric | Value | Business Meaning |
| :--- | :--- | :--- |
| **Net Revenue** | €24.69M | Strong overall market presence despite growth headwinds. |
| **Estimated Margin** | €7.41M | Represents a 30% margin, needing protection against rising rents. |
| **Order Efficiency** | 89.85% | High conversion from orders to sales, but logistics are strained. |
| **Stockout Risk** | 91 SKUs | Immediate revenue at risk due to potential empty shelves. |

---

## 🧠 Advanced Analytics (DAX Samples)

To achieve these insights, I developed custom logic such as:

* **Forecast Accuracy:** Measuring the absolute variance between demand and sales to penalize both over-ordering and under-ordering.
* **Stock Health Status:** A dynamic indicator that flags SKUs where `Inventory Level < Demand Forecast`.
* **Price Competitiveness:** A ratio comparing internal prices vs. competitor benchmarks to guide discount strategies.

---

## 🎥 Dashboard Preview
![ScreenRecordingUKRetailDashboard-ezgif com-video-to-gif-converter](https://github.com/user-attachments/assets/eaa4efc1-96ca-4f21-a41d-fdab42117449)

---

## 📂 Project Structure
* `Uk_Retail_Dashboard.pbix`: The primary Power BI report.
* `UK_Retail.csv`: The raw dataset used for analysis.
* `Screenshots/`: A folder containing high-resolution views of each dashboard page.

---

## 👤 Contact & Links
**[Famous SOUNTON]** - Data Analyst
* [LinkedIn Profile](https://www.linkedin.com/in/famoussounton)
* [Portfolio Website](https://www.datascienceportfol.io/sounntonfamous)
* **Email:** sountonfamous@gmail.com
