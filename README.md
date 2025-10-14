# 🚗 BMW Sales Report Dashboard (Excel-Based Project)

This project presents a comprehensive **BMW Sales Data Analysis** performed **entirely using Microsoft Excel** — without any external tools or programming.  
It visualizes key metrics like **model performance, fuel-type preference, regional sales distribution, transmission trends, and yearly performance** using **Pivot Tables, Charts, Slicers, and Excel formulas**.

---

## 📋 Project Overview

### 🔹 Key Features

#### 🧹 1. Data Cleaning & Preparation
- **Step 1 – Null Value Check**  
  Used the `COUNTBLANK()` function to identify missing cells in key columns such as *Model*, *Fuel Type*, *Transmission*, *Region*, and *Sales Volume*.  
  Cleaned or replaced blank entries accordingly.

- **Step 2 – Date Standardization**  
  Converted all date fields into a valid Excel date format and derived:
  - Weekday → `=TEXT(A2,"dddd")`
  - Year → `=YEAR(A2)`
  - Month → `=TEXT(A2,"mmm")`

- **Step 3 – Data Consistency**  
  Applied logical and text functions (`IF`, `IFS`, `TEXT`, `TRIM`) to remove extra spaces, fix case, and standardize labels.

- **Step 4 – Derived Calculated Fields**
  - **Engine Size Category**
    ```excel
    =IF(B2<2,"< 2 L",IF(B2<=4,"2–4 L","> 4 L"))
    ```
  - **Sales Classification**
    ```excel
    =IF(C2>7000,"High",IF(C2>4000,"Medium","Low"))
    ```

---

#### 📊 2. Data Analysis & Insights
Used key Excel formulas to uncover insights:
- `COUNTIF()` – Count models sold per region or fuel type.  
- `SUM()` – Total sales or mileage per category.  
- `MAX()` / `MIN()` – Identify top and bottom performers.  
- `VLOOKUP()` – Fetch attributes such as price, mileage, and classification.  
- `FILTER()` – Display filtered subsets dynamically.  

Created **Pivot Tables** to summarize:
- Model-wise, fuel-wise, and transmission-wise sales.  
- Region-wise and year-wise comparisons.  
- Weekday sales performance and yearly trends.

---

#### 🎨 3. Interactive Dashboard Design
- Built dashboards using **Pivot Charts**, **Slicers**, and **Dropdown Filters**.  
- Included visuals:
  - Total Models Sold  
  - Transmission-Wise Sales  
  - Weekday-Wise Trends  
  - Yearly Sales Comparison  
  - Fuel Type Performance  
  - Region & Color Distributions  
- Added conditional formatting and consistent color themes for clarity.

---

#### ⚙️ 4. Formula Summary

| Function | Purpose |
|-----------|----------|
| `COUNTBLANK()` | Detect null / blank cells |
| `IF()` / `IFS()` | Conditional logic (e.g., High / Medium / Low classification) |
| `COUNTIF()` / `SUM()` | Aggregate data by conditions |
| `MAX()` / `MIN()` | Identify best and worst performing values |
| `VLOOKUP()` | Lookup corresponding attributes |
| `FILTER()` | Dynamic filtering of subsets |
| `TEXT()` | Format dates and text labels |
| `TRIM()` | Remove unwanted spaces |
| `UNIQUE()` | Extract distinct Model / Fuel Type / Region values for dropdowns |

---

## 📊 Dashboard Highlights

### 1️⃣ Model-Wise Sales  
Compares all major BMW models — *3 Series, 5 Series, 7 Series, i3, i8, M3, M5, X1, X3, X5, X6* — showing total units sold.

### 2️⃣ Transmission Analysis  
Displays the proportion of **Manual** vs **Automatic** sales per model.

### 3️⃣ Fuel Type Analysis  
Compares **Petrol**, **Diesel**, **Hybrid**, and **Electric** vehicle performance.

### 4️⃣ Region Analysis  
Pie chart representation of sales across **Asia**, **Europe**, **Africa**, **North America**, **South America**, and **Middle East**.

### 5️⃣ Weekday & Yearly Trends  
Line charts revealing:
- **Sunday** as the peak sales day.  
- Sales trend from **2010–2024** showing variation in yearly performance.

### 6️⃣ Color & Engine Insights  
Lists available vehicle colors and groups cars by engine size category.

---

## 🧩 Project Structure

| File | Description |
|------|--------------|
| `BMW_Sales_Report.xlsx` | Main Excel workbook containing data, formulas, and dashboards |
| `BMW_Sales_Data.xlsx` | Cleaned/prepared dataset used for analysis |
| `BMW_Sales_Report.pdf` | Exported PDF of final dashboard |

---

## 🛠️ Excel Tools and Features Used
- Pivot Tables & Pivot Charts  
- Slicers 
- Conditional Formatting  
- Dropdown Lists (Data Validation)  
- Named Ranges and Dynamic Arrays  
- Dashboard Design and Layout Formatting  

---

## 📈 Key Insights
1. **Top Selling Models:** 7 Series and i8 lead global sales.  
2. **Transmission Preference:** ≈ 65 % of sales are Automatic.  
3. **Fuel Trend:** Hybrid and Electric models show steady growth.  
4. **Regional Performance:** Europe and Asia contribute the most sales.  
5. **Peak Day:** Sunday has the highest sales volume.  
6. **Engine Preference:** Cars with 2–4 L engines dominate.  

---

## 🧾 How to Use the Excel Dashboard

### Step 1 – Open Workbook
Open **`BMW_Sales_Report.xlsx`** in Microsoft Excel (2016 or later).

### Step 2 – Navigate Sheets
Each analysis has its own sheet:
- 📍 `Region Wise Sales`
- ⚙️ `Transmission Wise Sales`
- 📅 `Year Wise Sales`
- 🕒 `Daywise Highest Sales`
- 🔢 `Total Number of Sales` 

### Step 3 – Interact with Filters
- Apply slicers for **Region**.  
- Use dropdowns to check availability and engine categories.

---

## 🧠 Future Enhancements
- Automate data refresh via Power Query.  
- Integrate price/review data for deeper insights.  

---

## 🏁 Summary
This project demonstrates how **advanced Excel functions** can achieve complete business-level analytics.  
Through the use of formulas like **COUNTBLANK, FILTER, VLOOKUP, COUNTIF, IF, SUM, MAX, MIN, and UNIQUE**, Excel can serve as a full-fledged data-analysis and dashboarding tool — delivering professional, interactive insights without any external software.

---
