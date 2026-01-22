# 📊 Data Professional Global Survey Breakdown (2022)

<img width="1470" height="956" alt="Screenshot 1" src="https://github.com/user-attachments/assets/4d43ae35-8fd7-4ad3-8772-000ec4e46ec8" />

## 📌 Project Overview
This project explores the global landscape of the data industry using survey data from **630+ professionals**. The objective was to identify the key factors driving career success, salary levels, and job satisfaction in a rapidly evolving field.

By transforming raw, unstructured survey responses into a clean analytical model, this dashboard provides a clear roadmap for anyone looking to enter or advance in the data world.

---

## 🛠️ Tech Stack & Methodology
* **Tool:** Power BI Desktop
* **ETL & Data Cleaning:** Power Query (Crucial for normalizing inconsistent survey entries like salaries and job titles).
* **Modeling:** Calculated columns and DAX measures for salary averaging and sentiment analysis.
* **Key Metrics:** Average Salary by Role, Programming Language Popularity, and Job Happiness Gauges.

---

## 🔍 Key Problems Identified & Analytical Insights

### 1. The "Skill Premium" Gap
* **The Problem:** Aspiring professionals often struggle to decide where to specialize. 
* **Insight:** The data shows a significant salary jump for **Data Architects (€88k avg)** and **Data Scientists (€64k avg)** compared to entry-level Data Analyst roles (€55k).
* **Solution/Action:** To maximize ROI on learning, analysts should prioritize transitioning toward architecture or advanced engineering skills.

### 2. Programming Language Dominance vs. Salary
* **The Problem:** There is an overwhelming choice of languages to learn (Python, R, C++, SQL).
* **Insight:** **Python** is the undisputed leader in voter count, but high-paying roles often require a mix of languages.
* **Solution/Action:** Focus on Python for entry, but diversify into R or JavaScript for specialized roles in Research or Data Visualization to remain competitive.

### 3. Salary Satisfaction vs. Work-Life Balance
* **The Problem:** High tech salaries are often associated with high stress and burnout.
* **Insight:** Interestingly, the **Happiness with Work/Life Balance (5.74/10)** outscores **Salary Satisfaction (4.27/10)**.
* **Strategic Advice:** When negotiating for a new job, the data suggests that "Better Salary" is the top priority for those looking to move, as professionals seem more content with their culture than their paychecks.

---

## 📈 Dashboard Highlights & Impact

> **"Data Cleaning was the backbone of this project."** > Survey data is notoriously messy. I handled over 600 rows of diverse inputs to create a unified view of the global data market across the US, India, UK, and Canada.

* **Demographics:** Captured an average age of 29.8, indicating a young, dynamic workforce.
* **Accessibility:** Measured the "Difficulty to Break into Data," providing realistic expectations for self-taught learners vs. degree holders.

---

## 🧠 DAX Feature: Salary Normalization
I engineered a custom solution to turn salary ranges (e.g., "$100k-$120k") into a single average numerical value to allow for mathematical aggregation:

```dax
Avg Salary = 
VAR MinSal = SELECTEDVALUE('Data'[Min_Salary])
VAR MaxSal = SELECTEDVALUE('Data'[Max_Salary])
RETURN (MinSal + MaxSal) / 2
```


---

## 📂 Project Structure
* `Data Professional Survey Breakdown.pbix`: The primary Power BI report.
* `Data/Power BI - Data Pro Survey.xlx`: The raw dataset used for analysis.
* `Assets/Screenshot1.png`: The screen recording of the dashboard.
* `Assets/Data Professional Survey Breakdown.pdf`: The pdf version of the dashboard.
* `Readme`: The Readme.

---

## 👤 Contact & Links
**[Famous SOUNTON]** - Data Analyst
* [LinkedIn Profile](https://www.linkedin.com/in/famoussounton)
* [Portfolio Website](https://www.datascienceportfol.io/sounntonfamous)
* **Email:** sountonfamous@gmail.com
