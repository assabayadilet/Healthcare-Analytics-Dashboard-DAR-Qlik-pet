# Project Title
Short one-line summary of the project purpose (e.g. *Telecom Analytics Dashboard – Revenue and Customer Insights*).

---

## Overview
Briefly describe what the project does and what problem it solves.

**Example:**
This project analyzes telecom usage data to identify customer behavior patterns, segment users, and forecast revenue using SQL and Power BI.

---

## Objectives
List key goals or business questions the project answers.

- Analyze revenue trends by tariff
- Identify active and loyal customers
- Forecast revenue (CORE_REV) using DAX
- Create segmentation dashboard by user activity and spending

---

## Tools & Technologies
List the main tools, programming languages, and libraries you used.

| Tool / Tech | Purpose |
|--------------|----------|
| SQL (T-SQL) | Data aggregation and KPI calculation |
| Power BI | Data visualization, DAX modeling |
| Excel | Data cleaning and preparation |
| Python / Qlik Sense (optional) | Advanced analytics and visualization |

---

## Dataset
Describe your data source(s):  
- File name(s): `sales.xlsx`, `abonents_all.csv`, etc.  
- Number of records, key columns, and metrics.

**Example:**
Dataset contains telecom usage records:
- `tariff_id`, `user_id`, `usage_date`, `revenue`, `DATA_MB`, `MOU`
- Time range: Jan 2020 – Dec 2020  
- Total users: 25,000

---

## Data Model / ETL
Explain how data was prepared or structured:
- Joins, cleaning, transformation, DAX/SQL measures
- Mention tables or relationships (if using Power BI or Qlik Sense)

**Example:**
Power BI data model connects 3 fact tables (Usage, Revenue, Tariff) with 2 dimension tables (Users, Calendar).

---

## Key Calculations
Show examples of key queries or formulas used.

**SQL Example:**
```sql
SELECT
  tariff_id,
  FORMAT(usage_date, 'yyyy-MM') AS month,
  SUM(revenue) AS total_revenue
FROM tariff_usage
GROUP BY tariff_id, FORMAT(usage_date, 'yyyy-MM');
