🧾 README — Sales Performance Power BI Dashboard
📌 Project Overview

The Sales Performance Dashboard provides a comprehensive analysis of company sales, employee performance, and product returns.
It enables management to monitor key performance indicators (KPIs), understand sales trends, and identify improvement areas across regions, categories, and salespeople.

This dashboard was created as part of the DP K S Analytics Assignment using Power BI Desktop.
----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

📂 Datasets Used

Orders.xlsx – Contains detailed transactional data of customer orders.

Fields: Order ID, Order Date, Ship Mode, Customer Name, Sales, Quantity, Discount, Profit, Region, etc.

People.xlsx – Contains employee or salesperson mapping.

Fields: Region, Person

Returns.xlsx – Includes records of returned orders.

Fields: Order ID, Returned, Region
-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

⚙️ Data Preparation & Modeling

Imported all datasets into Power BI Desktop.

Cleaned and transformed data using Power Query Editor:

Removed duplicates and null values.

Changed data types for consistency.

Created calculated columns and measures (e.g., Total Sales, Profit Margin, Return Rate).

Built relationships:

Orders[Order ID] ↔ Returns[Order ID]

Orders[Region] ↔ People[Region]
------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

📊 Dashboard Features

The report consists of interactive visuals and filters for dynamic analysis:

1️⃣ Sales Overview Page

KPIs: Total Sales, Total Profit, Quantity Sold, Average Discount

Year-over-Year (YoY) Sales and Profit comparison

Sales trend by Month and Category

Regional Sales Performance

2️⃣ Employee Performance Page

Sales and Profit by Salesperson

Region-wise contribution per employee

Performance segmentation by category and customer type

3️⃣ Returns Analysis Page

Total Returned Orders and Return Rate (%)

Return patterns by Region and Category

Impact of returns on Profit

4️⃣ Customer Insights (optional)

Top 10 Customers by Sales

Customer ratings and performance segmentation
--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

💡 Key Insights

Identified top-performing regions and employees contributing the most revenue.

Noted that high discounts correlate with lower profits.

Detected return hotspots in specific product categories.

Visualized year-over-year growth patterns and profit fluctuations.

🧠 Tools & Technologies

Power BI Desktop

Power Query (Data Cleaning)

DAX (Data Analysis Expressions) for calculated measures

Excel (Data Source)

🪄 How to Use

Open the file DP K S Analytics Assignment.pbix in Power BI Desktop.

Enable data model relationships if prompted.

Use the filters and slicers to explore the dashboard.

visuals for detailed insights and too
----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
📈 KPIs & Measures
KPI	Formula	Description
Total Sales	SUM(Orders[Sales])	
Total revenue generated
Total Profit	SUM(Orders[Profit])	Net profit after discounts
Profit Margin %	DIVIDE([Total Profit],[Total Sales])	Profitability ratio
Return Rate %	COUNT(Returns[Order ID]) / COUNT(Orders[Order ID])	Percentage of returned orders
YoY Growth %	([Current Year Sales] - [Previous Year Sales]) / [Previous Year Sales]	Year-over-year sales change
------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
👤 Author

Darshan Patil
B.E. in Artificial Intelligence and Data Science (2021–2025)
Sahyadri Valley College of Engineering and Technology, Pune
📍 Pune, Maharashtra
🔗 LinkedIn
