
# Week 1 - Warehouse Logistics Risk Dashboard

**Internship:** NexAfrica Data Internship Program
**Tool:** Microsoft Excel
**Dataset:** E-commerce Inventory & Warehouse Logistics - 3,205 SKUs

### Objective
Identify inventory at risk of stockout to prevent warehouse disruptions.

### What I Did
1.  **Data Cleaning:** Fixed `last_restock_date` formatting issue (##### error) by expanding column and setting Date format.
2.  **Created 3 New Columns:**
    - `Stock_Status` = `=IF([Current_Stock]<= [Reorder_Point], "Low Stock", "In Stock")`
    - `Days_Since_Restock` = `=TODAY() - [last_restock_date]`
    - `Reorder_Risk` = `=IF(AND(Stock_Status="Low Stock", Days_Since_Restock>60), "CRITICAL", IF(Stock_Status="Low Stock", "WARNING", "SAFE"))`
3.  **Analysis:** Built PivotTable to count Stock Status by Reorder Risk and Product Category.

### Key Findings
- Total SKUs: 3,205
- CRITICAL (Low Stock + >60 days): 101 items - Immediate reorder needed
- WARNING: 136 items
- SAFE: 2,967 items
- Highest Risk Category: Pharma (24 CRITICAL items)

### Files in this folder
- `Week1_Logistics_Risk_Dashboard.xlsx` - Excel workbook with formulas & Pivot
- `PivotTable.png` - Screenshot proof of Pivot analysis

### Skills Used
Excel IF, AND, TODAY(), Date Formatting, PivotTables, GitHub Version Control
