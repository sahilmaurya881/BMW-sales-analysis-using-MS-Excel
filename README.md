# 🚗 BMW SALES REPORT

---

## 📋 Project Overview
This project presents a comprehensive **BMW Sales Data Analysis (2010–2024)** built entirely in **Microsoft Excel**, without using external tools or programming.  
It demonstrates data cleaning, transformation, analysis, and visualization—culminating in a professional, interactive dashboard.

---

## ❗ Problem Statement
BMW’s global sales data spans multiple models, regions, and years, making it difficult to analyse performance trends manually.  
There was no centralized, visual system to identify best-selling models, regional strengths, transmission or fuel-type preferences, or yearly variations.  
Hence, this project aims to create a **single Excel-based dashboard** that consolidates all BMW sales information and delivers quick, interactive insights for decision-making.

---

## 📈 Dashboard Highlights
The dashboard showcases **eight major analytical areas** offering a quick visual overview of BMW’s performance from **2010–2024**:

- **Total Model Sales:** The 7 Series leads overall, followed by i3 and i8.  
- **Transmission-Wise Sales:** Automatic models dominate, indicating a shift toward convenience.  
- **Weekday-Wise Sales:** Sunday records peak sales; Friday and Monday are the lowest.  
- **Week-Wise Model Sales:** All models peak on Sundays, confirming weekend buying behavior.  
- **Year-Wise Sales:** Sales stayed stable 2010–2018, dipped during 2020–2023, and rebounded in 2024.  
- **Fuel-Type-Wise Sales:** Petrol and Hybrid perform slightly better; EVs are steadily growing.  
- **Total Sales (Pie Chart):** Balanced model distribution; 7 Series slightly ahead.  
- **Region-Wise Sales:** Equal contribution across regions showing strong global presence.  

📄 *A detailed explanation for each chart is available in the workbook’s **“Conclusion” sheet.***

---

## ⚙️ Key Features

### 1️⃣ Data Cleaning & Preparation
- **Null Value Check:**  
  Used `COUNTBLANK()` to identify missing entries in key columns like Model, Fuel Type, Transmission, Region, and Sales Volume.  
  Cleaned or replaced blanks accordingly.  
- **Date Standardization:**  
  Converted all date fields into valid Excel date formats and derived:  
  - Weekday → `=TEXT(A2,"dddd")`  
  - Year → `=YEAR(A2)`  
  - Month → `=TEXT(A2,"mmm")`

---

### 2️⃣ Data Analysis & Insights
Used Excel formulas for trend analysis:
- `COUNTIF()` – Count models sold per region/fuel type  
- `SUM()` – Aggregate sales/mileage  
- `MAX()` / `MIN()` – Identify top and bottom performers  
- `VLOOKUP()` – Retrieve attributes  
- `FILTER()` – Dynamically display subsets  

**Pivot Tables** summarize:
- Model-wise, fuel-wise, and transmission-wise sales  
- Region-wise and yearly comparisons  
- Weekday and year-wise performance trends  

---

### 3️⃣ Interactive Dashboard Design
Developed using **Pivot Charts, Slicers, and Dropdown Filters**, featuring:
- Total Models Sold  
- Transmission Trends  
- Fuel Type Analysis  
- Weekday & Yearly Performance  
- Regional Distributions  
- Engine Category Insights  

Enhanced with **conditional formatting**, consistent themes, and a clear layout for professional readability.

---

### 4️⃣ Formula Summary
Key Excel functions used include:  
`COUNTBLANK()`, `IF()`, `IFS()`, `COUNTIF()`, `SUM()`, `MAX()`, `MIN()`,  
`VLOOKUP()`, `FILTER()`, `TEXT()`, `TRIM()`, and `UNIQUE()`.

---

## 🧩 Project Structure
- **BMW sales data (2010–2024) Raw.xlsx** – Unprocessed dataset  
- **BMW Sales Report.xlsx** – Cleaned, analysed dataset with dashboard  
- **BMW_Sales_Report_Dashboard.pdf** – Exported PDF of the final dashboard  

---

## 🧰 Excel Tools and Features Used
- Pivot Tables & Pivot Charts  
- Slicers  
- Conditional Formatting  
- Data Validation (Dropdowns)  
- Named Ranges & Dynamic Arrays  
- Dashboard Layout Formatting  

---

## 📊 Key Insights
- **Top Models:** 7 Series, i3, i8  
- **Transmission:** ~65% Automatic  
- **Fuel Mix:** Hybrid & Electric gaining traction  
- **Regions:** Europe and Asia strongest markets  
- **Peak Day:** Sunday  
- **Engine Range:** 2–4 L, most popular  

---

## 🧭 How to Use the Excel Dashboard
1️⃣ **Open Workbook:** `BMW_Sales_Report.xlsx`  
2️⃣ **Navigate Sheets:**  
   - Dashboard  
   - Static Analysis  
   - Conclusion (Detailed Observations)  
   - Region-Wise Sales  
   - Transmission-Wise Sales  
   - Year-Wise Sales  
   - Day-Wise Highest Sales  
   - Total Sales Summary  
3️⃣ **Filters:**  
   Apply slicers for region, fuel type, and transmission to explore results dynamically in the Dashboard.

---

## 🚀 Future Enhancements
- Automate data refresh using **Power Query**  
- Integrate **price and review data** for deeper insights  
- Add **VBA automation** for interactive storytelling  

---

## 🌐 Data Source
[https://www.kaggle.com/datasets/ahmadrazakashif/bmw-worldwide-sales-records-20102024/data](https://www.kaggle.com/datasets/ahmadrazakashif/bmw-worldwide-sales-records-20102024/data)

---

## 📜 Project Scope
The project focuses on building a **complete analytical workflow within Excel**, including:
- Cleaning and standardizing BMW sales data (2010–2024)  
- Performing analysis by Model, Fuel Type, Transmission, Region, and Year  
- Designing an interactive dashboard using Pivot Tables, Charts, and Slicers  
- Summarizing all key findings in a dedicated **Conclusion sheet** for quick reference  

---

## 🚧 Limitations
- **Data Size:** Excel’s performance may degrade with very large datasets.  
- **Manual Updates:** Dashboard refresh requires manual data import.  
- **Static Output:** No real-time automation or web-based interactivity.  
- **Historical Focus:** Analysis is retrospective; no forecasting included.  
- **Tool Constraints:** Visual and automation options are limited compared to BI tools like Power BI or Tableau.  

---

## 🏁 Final Summary
BMW’s sales performance remains **balanced and resilient** across models, fuel types, and regions.  
The **7 Series** dominates total sales, supported by strong electric i-model growth.  
Automatic transmissions lead, weekend sales peak, and hybrid-electric trends reflect BMW’s steady progress toward sustainability.  
After brief disruptions in **2020–2023**, **2024 marks a strong recovery** and renewed consumer confidence.
