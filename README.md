# elevatelabs_task8_SimpleSalesDashboardDesign
Task 8 – Simple Sales Dashboard
Objective
Design an interactive dashboard to analyze Superstore Sales performance by product category, region, and time (Month-Year).
Dataset
File: Superstore_Cleaned.csv

Columns Used:
Order Date
Region
Category
Sales
Profit

🛠 Tools
Power BI Desktop (for visualization)

GitHub (for submission & version control)

⚙️ Steps Followed
Imported Superstore_Cleaned.csv into Power BI.

Changed data types (Date, Text, Decimal Number).

Created calculated columns:

MonthYear = FORMAT('Superstore_Cleaned'[Order Date], "MMM yyyy")
MonthYearSort = YEAR('Superstore_Cleaned'[Order Date]) * 100 + MONTH('Superstore_Cleaned'[Order Date])
→ Sorted MonthYear by MonthYearSort for proper order.

Created measures:

Total Sales = SUM('Superstore_Cleaned'[Sales])
Total Profit = SUM('Superstore_Cleaned'[Profit])
Profit %     = DIVIDE([Total Profit], [Total Sales])
Built visuals:

Line chart → Sales by Month-Year

Bar chart → Sales by Region

Donut chart → Sales by Category

Slicer → Region and Category filters

KPI Cards → Total Sales, Total Profit, Profit %

Formatted with titles, themes, and aligned layout.
