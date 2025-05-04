# Sales and Collection Performance Dashboards (2024)

## Overview
These **Power BI dashboards** provide a comprehensive analysis of 2024 sales and collection performance across regions, top customers, and monthly trends. Built with **Excel data models** and **DAX formulas**, they enable dynamic tracking of key metrics for strategic decision-making.

---

## Key Dashboards

### 1. **Sales Performance Dashboard**
   - **Top 50 Customers**:  
     - John Charles LTD (£0.34bn), Jeffrey Jacobson LTD (£0.17bn), etc.  
     - **66%** of total sales from top performers.  
   - **Regional Breakdown**:  
     - SOUTH-EAST dominates with **£1.5bn** sales.  
   - **Monthly Trends**:  
     - Visualized from Jan–Nov 2024 (peak: **£3bn**).  

### 2. **Collection Performance Dashboard**
   - **Top Collectors**:  
     - Robert Atkinson LTD (£0.38bn), Elizabeth Rodriguez (£0.35bn).  
   - **Regional Collections**:  
     - SOUTH-SOUTH leads with **£1.9bn**.  
   - **Efficiency Metrics**:  
     - **86%** collection rate.  

### 3. **Combined Sales & Collection Dashboard**
   - **Comparative Analysis**:  
     - Sales vs. Collections by region (e.g., SOUTH-EAST: **£1.5bn** vs. **£1.9bn**).  
   - **Monthly Overlays**:  
     - Dual-axis trends for holistic performance tracking.  

---

## Technical Implementation

### Tools & Technologies
- **Power BI**: Interactive visualizations and drill-throughs.  
- **Excel**: Data cleansing and pivot tables.  
- **DAX**: Measures for KPIs like:  
  ```dax
  Collection Rate = DIVIDE([Total Collected], [Total Sales], 0)
Data Model
Star Schema: Fact tables for sales/collections linked to dimension tables (Customers, Dates, Regions).

Dynamic Filters: Slicers for Region, Month/Year, and Customer Tier.

How to Use
Navigation:

Use slicers to filter by region, timeframe, or customer.

Hover over charts for tooltip details (e.g., exact % values).

Data Refresh:

Connect to your data source via Power Query Editor.

Setup Instructions
Prerequisites:

Power BI Desktop.

Excel files with raw sales/collection data.

Steps:

bash
git clone https://github.com/your-repo/sales-dashboards.git
Open .pbix files in Power BI Desktop.

Update data source paths if needed.

DAX Examples
dax
// Top Customer Contribution
Top Customer Sales = 
CALCULATE(
    [Total Sales],
    TOPN(50, Customers, [Total Sales], DESC)
)
Contributing
Enhancements:


Contact
📧 Email: jbignames@gmail.com
🔗 LinkedIn: https://www.linkedin.com/in/okeoghene-akpovwovwo-0291a4150/
