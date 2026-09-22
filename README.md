# Data Analytics Task 5 — Power BI Business Intelligence Dashboard

## Objective
Transform the cleaned retail sales dataset into an interactive Power BI dashboard, using a proper Fact/Dimension data model and DAX measures, to help management understand performance and make data-driven decisions.

## Data Model
- **Orders** (fact table) — 11,971 transactions
- **Customers** (dimension) — 25 customers linked by CustomerID, each tied to a Region
- **Products** (dimension) — linked via a combined Item+Category key (ProductKey), to correctly handle the "Unknown Item" placeholder that spans multiple categories
- **Calendar** (dimension) — linked by OrderDate

## DAX Measures
Total Sales, Total Orders, Total Customers, Average Order Value, Sales 2022/2023, Sales Growth %, Category Contribution %

## Dashboard
One page containing:
- 4 KPI cards (Total Sales, Total Orders, Total Customers, Average Order Value)
- Sales by Category (bar chart)
- Sales by Region (pie chart)
- Total Sales by Month (line chart, chronologically sorted via a MonthSort column)
- Total Sales by Segment (column chart)
- Top 10 Products by Sales (table)
- Slicers: Region, Segment, and an OrderDate range slider — all cross-filtering the full page live

## Key Findings
- Total sales: €1,552,071 across 11,971 orders (average order value €129.65)
- Category and regional performance are both tightly clustered (13.5% and 3.1% spreads) — no single standout or weak spot
- High Value customers (top third by spend) drive a disproportionate ~38% of revenue
- Monthly sales follow a recurring up-down pattern rather than a clear growth/decline trend
- January 2022 was the single highest month on record

## Recommendations
1. Build a loyalty/retention program targeting the High Value customer segment
2. Investigate what drove the January 2022 spike to see if it's repeatable
3. Avoid concentrating investment into one "top" category or region, since demand is evenly spread

## Deliverables
- `Norysca_DataAnalytics_Task5.pbix`
- `Norysca_DataAnalytics_Task5_SourceData.csv`
- `Business_Insights_Report.pdf`

## Tools
Power BI Desktop — Power Query, Data Modeling, DAX, Interactive Visualizations, Slicers
