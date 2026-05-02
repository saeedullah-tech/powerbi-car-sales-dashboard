🚗 Car Sales Performance Dashboard

📊 Project Overview
This project delivers an end-to-end data analysis and visualization solution for car sales performance using Power BI, SQL, and Excel. The dashboard provides actionable insights into sales trends, pricing behavior, and regional performance, enabling data-driven decision-making.
The solution focuses on YTD, MTD, and YoY analysis, helping stakeholders monitor growth, identify high-performing segments, and optimize sales strategies.

🎯 Business Objectives


Track total sales, cars sold, and average price in real time


Analyze year-over-year (YoY) growth trends


Identify top-performing brands, regions, and body styles


Enable drill-down analysis across multiple dimensions


Reduce manual reporting effort through automation



🛠️ Tools & Technologies


Power BI – Data visualization & dashboard development


SQL – Data extraction and querying


Excel – Data cleaning and preprocessing


DAX – KPI calculations and time intelligence



🔄 Data Preparation (ETL)


Cleaned and transformed raw sales data using Power Query & Excel


Handled missing values, corrected data types, and standardized formats


Built a date (calendar) table to enable time-based analysis


Established relationships between tables for accurate reporting



📈 Key Metrics & KPIs


YTD Total Sales: $371M


YTD Avg Price: $28K


YTD Cars Sold: 13.26K


YoY Sales Growth: 19.73%


MTD Sales: $54.28M



📊 Dashboard Features
🔹 Sales Overview


YTD, MTD, and YoY performance tracking


KPI cards with dynamic updates


🔹 Trend Analysis


Weekly sales trend visualization


Identification of peak and low-performing periods


🔹 Segmentation Analysis


Sales breakdown by:


Body Style


Car Color


Company (Brand)




🔹 Geographic Insights


Interactive map showing sales distribution by region


🔹 Detailed Reporting


Transaction-level table with:


Customer


Dealer


Car Model


Sales Value




🔹 Dynamic Filtering


Filters for:


Body Style


Dealer Name


Transmission


Engine Type





🧮 Key DAX Calculations
Base Measures
Total Sales = SUM(car_data[Price ($)])Total Cars Sold = COUNT(car_data[Car_id])Avg Price = DIVIDE([Total Sales], [Total Cars Sold])
Time Intelligence
YTD Total Sales = TOTALYTD([Total Sales], 'Calendar Table'[Date])MTD Total Sales = TOTALMTD([Total Sales], 'Calendar Table'[Date])PYTD Total Sales = CALCULATE([Total Sales], SAMEPERIODLASTYEAR('Calendar Table'[Date]))
Growth Metrics
Sales Difference = [YTD Total Sales] - [PYTD Total Sales]YOY Sales Growth % = DIVIDE([Sales Difference], [PYTD Total Sales])

📌 Key Insights


Sales reached $371M YTD, showing strong overall performance


19.7% YoY growth indicates consistent business expansion


Certain regions and brands contribute significantly to revenue


Seasonal trends highlight peak sales periods, useful for forecasting


Average price stability (~$28K) suggests consistent market positioning



🚀 Business Impact


Reduced manual reporting effort by ~40% through dashboard automation


Enabled faster decision-making with real-time KPI tracking


Improved visibility into sales performance and customer trends


Provided a scalable reporting solution for business stakeholders



📷 Dashboard Preview
![Image](https://github.com/saeedullah-tech/powerbi-car-sales-dashboard/blob/aefda7b5dccdfcb9f4563cf33628b8754d5271fc/Screenshot%20(69).png)
![Image](https://github.com/saeedullah-tech/powerbi-car-sales-dashboard/blob/aefda7b5dccdfcb9f4563cf33628b8754d5271fc/Screenshot%20(70).png)
![Image](https://github.com/saeedullah-tech/powerbi-car-sales-dashboard/blob/aefda7b5dccdfcb9f4563cf33628b8754d5271fc/CarsSalesDashboard-Trim-ezgif.com-video-to-gif-converter.gif)

📁 Project Structure
Car-Sales-Dashboard/│├── Data/├── PowerBI_File.pbix├── SQL_Scripts/└── README.md

🔗 How to Use


Open the .pbix file in Power BI Desktop


Refresh the dataset if needed


Use filters and slicers to explore insights



👤 Author
Saeed Ullah
Data Analyst | Excel | Power BI | SQL

