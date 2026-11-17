# Sales-Performance-Dashboard-PowerBI
# 📊 Sales Performance & Revenue Analytics Dashboard (Power BI & Excel)

## 📌 Project Overview
This project analyzes retail sales performance across multiple product categories, customer segments, and geographic regions. The goal is to transform raw transactional data into an interactive **Power BI Dashboard** that helps management track KPIs, identify revenue bottlenecks, and optimize sales strategy.

---

## 🛠️ Tools & Technical Methodology
- **Data Cleaning & Transformation (Power Query & Excel):** Handled missing values, standardized date formats, removed duplicate records, and created calculated columns using Power Query and Advanced Excel (`XLOOKUP`, `INDEX-MATCH`, `Pivot Tables`).
- **Data Modeling:** Built a **Star Schema** data model connecting a central `Fact_Sales` table with dimension tables (`Dim_Product`, `Dim_Customer`, `Dim_Region`, `Dim_Calendar`).
- **DAX Calculations (Intermediate):** Created dynamic measures for business KPIs:
  - `Total Revenue = SUM(Fact_Sales[Sales_Amount])`
  - `Total Profit = SUM(Fact_Sales[Profit])`
  - `Profit Margin % = DIVIDE([Total Profit], [Total Revenue], 0)`
  - `YoY Sales Growth % = DIVIDE([Total Revenue] - [Previous Year Sales], [Previous Year Sales], 0)`
- **Data Visualization (Power BI):** Designed a multi-page interactive dashboard with slicers, drill-through filters, conditional formatting, and KPI cards.

---

## 🔍 Key Analytical Insights
1. **Top Revenue Drivers:** The **Electronics & Gadgets** category contributed **42%** of total revenue, while **Accessories** delivered the highest profit margin (**28%**).
2. **Seasonal Trends:** Peak sales occurred during **Q4 (October–December)**, showing a **19.5% increase** compared to Q3 due to seasonal promotions.
3. **Regional Performance:** Urban hubs generated **65%** of overall sales volume, while emerging regional markets showed the fastest Quarter-over-Quarter (QoQ) growth rate (**14%**).
4. **Discount Impact:** Discounts above **20%** significantly eroded net profit margins without generating proportional volume growth.

---

## 💡 Business Recommendations
- **Optimize Discount Strategy:** Cap standard promotional discounts at **15%** and bundle high-margin accessories with core products.
- **Inventory Allocation:** Increase stock levels by **20%** ahead of Q4 for top-performing SKUs to prevent stockouts.
- **Regional Expansion:** Allocate targeted digital marketing budgets to high-growth secondary regions.

---

## 📂 Repository Structure
- `README.md` – Project documentation, DAX formulas, and business insights.
- `sales_data_cleaned.csv` – Sample cleaned retail dataset used for analysis.
