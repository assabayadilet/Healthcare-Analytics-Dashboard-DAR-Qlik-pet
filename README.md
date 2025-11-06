# Qlik Sense Sales Analytics Dashboard

## Overview
This project showcases a **Qlik Sense analytical application** designed to explore and visualize sales performance.  
The dashboard follows the **DAR (Dashboard – Analysis – Reporting)** methodology and demonstrates best practices for KPI design, storytelling, and user experience.

---

## Objectives
- Create a structured Qlik Sense app that follows the **DAR concept**:
  - **Dashboard:** high-level overview of KPIs
  - **Analysis:** detailed exploration of sales by dimensions
  - **Reporting:** tabular and exportable reports
- Ensure clean design and proper labeling of measures and dimensions.
- Provide meaningful business insights for stakeholders.

---

## Tools & Technologies
| Tool | Purpose |
|------|----------|
| **Qlik Sense** | Main BI tool for dashboard creation |
| **Excel (`Продажи.xlsx`)** | Source dataset |
| **Document (`Задача qlik Sense.docx`)** | Technical requirements and design guidelines |
| **QVF file (`Меры и измерения.qvf`)** | Qlik Sense app with all measures and dimensions |

---

## Dataset
The dataset `Продажи.xlsx` contains sales data used for visualization and analysis.

**Key fields include:**
- `Дата` — transaction date  
- `Регион` — sales region  
- `Категория` — product category  
- `Продажи` — total sales amount  
- `Количество` — units sold  

The dataset enables performance comparison by **region**, **category**, and **time**.

---

## Measures & Dimensions
According to the document *“Задача qlik Sense.docx”*, all measures and dimensions are structured as **Master Items** for reusability and clarity.

**Examples:**
- **Measures:**  
  - `Продажи` → `Sum(Продажи)`  
  - `Средняя цена` → `Sum(Продажи) / Sum(Количество)`  
  - `Доля категории` → `Sum(Продажи) / Sum(TOTAL Продажи)`

- **Dimensions:**  
  - `Регион`  
  - `Категория`  
  - `Год`, `Месяц` (from autoCalendar)

---

## DAR Structure

### 1. Dashboard
- Key KPIs (Total Sales, Average Price, Total Quantity)
- Trend line of sales by month
- Top-performing regions and categories
- Quick filters for date and product type

### 2. Analysis
- Drill-down by Region → Category → Product  
- Comparison charts showing category share and growth over time  
- Heatmaps for sales vs. region and profitability

### 3. Reporting
- Detailed tables for export (e.g. Sales by Region/Month)
- Interactive filters for dynamic reporting
- Clean table headers and numeric formatting

---

## Design & UX Principles
- Consistent color palette for categories  
- Proper titles and labels — no technical expressions like `Sum(Продажи)`  
- Each sheet includes:
  - A short **description of purpose**
  - A **cover page** or header  
  - Intuitive navigation between sheets

---

## Insights
- The dashboard identifies top regions contributing most to sales.
- Product categories with the highest average price can be tracked for premium growth.
- Seasonal sales patterns visible in monthly trendlines.

---

## Future Enhancements
- Add profitability and discount analysis.
- Connect to live database for automatic updates.
- Integrate customer segmentation based on purchase behavior.



## 🏷️ Tags
`#qliksense` `#data-analytics` `#dashboard` `#business-intelligence` `#excel` `#dar` `#data-visualization`
