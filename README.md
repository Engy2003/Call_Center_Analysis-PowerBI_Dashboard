# 📊 Call Center Dashboard

## 📌 Project Overview
This project was developed for **Call Center** to monitor and analyze performance metrics.  
The interactive Power BI dashboard helps decision-makers track calls, deals, and agent performance with dynamic comparisons across time periods.

---

## ⚙️ Project Phases

### 1. **Data Preparation**
- Imported datasets from **Microsoft Access (2023)** and **Excel (2024)**.  
- Cleaned and validated data (handled nulls, checked duplicates, corrected data types, and ensured consistency).  
- Merged **First Name** and **Last Name** into a single **Full Name** column.  

---

### 2. **Data Modeling**
- Built a **Calendar Table** using DAX (`CALENDARAUTO`) with fields: Year, Month, Quarter, Weekday, Weekday Type.  
- Marked the Calendar as a **Date Table** and linked `Calendar[Date]` with `Dataset[Date]`.  
- Defined **important tables** (Switch for KPI).  
- Created calculated columns (e.g., **Deal Group** = No Deals, Low Volume Deals, High Volume Deals).  
- Established model relationships for accurate time intelligence and filtering.  

---

### 3. **DAX Measures**
- Created key measures to calculate:  
  - **Total Calls**  
  - **Total Calls Reached**  
  - **Total Deals Closed**  
  - **Total Deals Values ($)**  
- Built **time intelligence measures** for previous Month, Quarter, Year.  
- Developed **comparison measures** (Vs LM, Vs LQ, Vs LY) for percentage and difference.  
- Added **color-formatting measures** to highlight positive vs negative performance (Blue if growth, Red if decline).  
- Built **Dropped Calls** = (Total Calls – Total Calls Reached).  

---

### 4. **Visualization & Dashboard Design**
Designed a professional, interactive **Power BI dashboard** with a clean layout, custom icons, and bookmarks for navigation.  

**Dashboard Layout:**  

1. **KPI Cards (Top Section)**  
   - Displays 4 KPIs: **Total Calls, Calls Reached, Deals Closed, Total Deal Values**.  
   - Under each KPI, a **dynamic comparison line** shows performance vs Last Month, Last Quarter, or Last Year (depending on slicer selection).  
   - The line includes **percentage change and absolute difference** with **+/- signs** and **color coding** (Blue for positive, Red for negative).  

2. **Metric Comparison Chart (Bottom Section)**  
   - A **dynamic stacked column chart** that allows switching between:  
     - Total Calls  
     - Calls Reached  
     - Deals Closed  
     - Deal Values  
   - X-axis can switch between **Year, Month, Quarter, Weekday Type, Weekday** (via bookmarks).  
   - Provides quick visual trend analysis.  

3. **Agent Performance Table (Bottom Section)**  
   - A matrix table displaying: **Agent Full Name, Total Calls, Calls Reached, Dropped Calls, Deals Closed, Deal Values**.  
   - Includes a slicer for filtering by **Deal Group** (No Deals, Low Volume Deals, High Volume Deals).  

4. **Interactive Filters (Side Panel)**  
   - Toggleable filter panel (via bookmark buttons) for selecting **Year, Month, Quarter, Full Name**.  
   - Users can open/close the panel to refine dashboard insights.  

---

## 💡 Dashboard Insights
- **KPI Tracking**: Quick view of calls, deals, and revenue performance with instant YoY, QoQ, MoM comparisons.  
- **Agent Productivity**: Identifies top-performing and underperforming agents.  
- **Operational Efficiency**: Highlights dropped calls and missed opportunities.  
- **Time Trends**: Flexible breakdown across year, quarter, month, weekday.  
- **Deal Analysis**: Groups agents by volume of deals closed for targeted coaching and incentives.  

---

## 🚀 Business Value
- Helps **management** monitor call center efficiency and improve decision-making.  
- Provides **sales and deal insights** to increase revenue.  
- Identifies **agent training needs** by analyzing call-to-deal conversion.  
- Reduces customer churn by analyzing dropped calls.  
- Supports **data-driven strategies** for staffing, performance incentives, and customer engagement.  

---

## 📂 Project Files
- **📁 Images/** → Screenshots of the **data model** and **dashboard**.  
- **📁 Icons/** → Custom icons used in the Power BI dashboard.  
- **📁 Call Center Dataset/** → Source data files:  
  - `Call Center 2023 (Access Database)`  
  - `Call Center 2024 (Excel File)`  
- **📄 Call Center Dashboard.pbix** → Power BI dashboard file.  
- **📄 Important_Columns.txt** → Key dataset columns used in the project.  
- **📄 Important_Measures.txt** → All created DAX measures.  
- **📄 Important_Tables.txt** → Main tables and their role in the model.  

---

## 📬 Contact
👩‍💻 **Engy Saeed**  
- 📧 Email: [engy.saeed@example.com](engysead498@gmail.com)  
- 💼 LinkedIn: [Engy Saeed](https://www.linkedin.com/in/engy-saeed2003/)  

---
