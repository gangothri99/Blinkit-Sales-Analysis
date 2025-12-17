Blinkit Sales Analysis Dashboard

📌 Problem Statement

The Blinkit Sales Analysis Power BI Project aims to deliver an insightful and interactive dashboard for analyzing sales performance across multiple dimensions.

This dashboard empowers stakeholders to:

Visualize key performance metrics

Identify trends and patterns

Extract actionable insights from sales data

Support data-driven decision-making and strategic planning

⚙️ Steps Followed

Data Loading
Imported the dataset (CSV file) into Power BI Desktop.

Data Profiling & Cleaning
Used Power Query Editor to check:

Column distribution

Column quality

Column profiling

Extracted, cleaned, and transformed data to ensure accuracy and consistency.

KPI Creation
Defined key performance indicators (KPIs) according to business requirements, such as Total Sales, Average Sales, Average Rating, and Number of Items.

Dashboard Development
Built an interactive Power BI dashboard with slicers, cards, and visuals.

Designed a metrics table with the following DAX expression to integrate KPIs dynamically:

Metrics = { ("Total Sales", NAMEOF('BlinkIT Grocery Data'[Total Sales]), 0), ("Avg Sales", NAMEOF('BlinkIT Grocery Data'[Avg Sales]), 1), ("Avg Rating", NAMEOF('BlinkIT Grocery Data'[Avg Rating]), 2), ("No of Items", NAMEOF('BlinkIT Grocery Data'[No of Items]), 3) }

DAX Measures
Created the following measures:

Total Sales

Total Sales = SUM('BlinkIT Grocery Data'[Sales])

Average Sales

Avg Sales = AVERAGE('BlinkIT Grocery Data'[Sales])

Average Rating

Avg Rating = AVERAGE('BlinkIT Grocery Data'[Rating])

Number of Items

No of Items = COUNTROWS('BlinkIT Grocery Data')

Visualized each measure using card visuals for clarity.

Dashboard Publication
Created a single-page report in Power BI Desktop.

Published the dashboard to Power BI Service for stakeholder access.

📊 Key Insights 🔹 Sales Performance

Total Sales: $1.20M

Top Category: Fruits & Vegetables – $178.12K

Lowest Category: Seafood – $9.08K

By Outlet Size:

Medium size – $507.9K (highest)

High size – $248.99K (lowest)

🔹 Average Ratings (Selected Categories)

Meat: 4.0 / 5

Fruits & Vegetables: 3.91 / 5

Household: 3.95 / 5

Health & Hygiene: 3.93 / 5

Soft Drinks: 3.89 / 5

Canned Goods: 3.95 / 5 (Null values were excluded from calculations.)

🔹 Additional Insights

Total Items Sold: 8,523 across multiple outlets.

Sales by Fat Content:

Low Fat – 776.32K

Regular Fat – 425.36K

Peak Year: 2018 recorded the highest revenue.

📷 Dashboard Snapshots

Power BI Desktop visuals

Published report in Power BI Service (Screenshots attached in the project folder)

🚀 Conclusion

The Blinkit Sales Analysis Dashboard provides a comprehensive view of sales performance across categories, outlets, and customer preferences. It enables stakeholders to monitor KPIs, evaluate trends, and make informed business decisions effectively.
