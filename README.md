# Coffee-Shop-Sales-Analysis- Understanding business drive, customer preferences, and sales performance across three NYC coffee shop locations
## Background and Scenario
As a newly appointed franchise owner of a coffee shop chain with three locations in New York City, I collected transactional data from January to June 2023 — the first half of the year — to better understand purchase behaviour and streamline operations across all three stores.
## Business Problem & Objectives
The franchise needs to move from raw transactional data to actionable operational and strategic insights.

As a franchise owner, I need clear visibility into:

  •	How revenue is trending month over month across all three locations
  
  •	Which products and categories are driving the most revenue
  
  •	When peak trading hours occur, to inform staffing and operational decisions
  
  •	How the three NYC stores compare in performance against each other
  
  •	Where the revenue growth opportunities and operational risks exist
  
This project was designed to answer one core question:
"Can the coffee pay the rent? Understanding business drive, customer preferences, and sales performance across three NYC coffee shop locations."
## Dataset Overview
  •	Data Source: Maven Analytics- Coffee Shop Sales Dataset (publicly available)
  
  •	Time Period Covered: January 2023 – June 2023 (H1 only)
  
  •	Volume: 149,116 transaction records
  
  •	Format: Excel (.xlsx)
## Key Columns
  •	transaction_id
  
  •	transaction_date
  
  •	transaction_time
  
  •	transaction_qty
  
  •	store_id
  
  •	store_location
  
  •	product_id
  
  •	unit_price
  
  •	product_category
  
  •	product_type
  
  •	product_detail
  <img width="1566" height="677" alt="image" src="https://github.com/user-attachments/assets/7615c3ef-23cf-417f-8f7f-bc1b1be831f1" />

## Tools Used
  •	Microsoft Excel — Data cleaning, calculated columns, pivot tables, dashboard design, slicers, dynamic KPI linking
  
  •	Paper sketch — Wireframing the dashboard layout and visual hierarchy before building
## Data Cleaning and Validation

  •	Verified zero null values across all 11 columns

  •	Confirmed no duplicate transaction IDs
  
  •	Validated unit_price range ($0.80 – $45.00) — no anomalies found
  
  •	Validated transaction_qty range (1–8) — no anomalies found
  
  •	Confirmed transaction_date range: Jan 1 – Jun 30, 2023 only
  
  •	Confirmed 3 store locations: Astoria, Hell's Kitchen, Lower Manhattan
  
  •	Confirmed 9 product categories and 29 product types
The raw dataset was clean. No records needed to be removed or corrected. 

The primary preparation work was enriching the data by deriving new columns that the raw data did not contain.

## Calculated Columns Added

Five new columns were derived from the raw data to enable time-based and financial analysis across all 149,116 rows:

  •	Revenue     
  
  •	Month       
  
  •	Month Name  
  
  •	Day of Week 
  
  •	Hour        

Why two month columns? The Month number enables correct chronological sorting in pivot tables. Without it, Excel sorts months alphabetically (April before January). The Month Name provides the readable label for chart axes. Both are required and serve different purposes.

<img width="1567" height="661" alt="image" src="https://github.com/user-attachments/assets/f3447267-af69-4bd9-9545-1609ea7c4691" />
## Dashboard Design and Visualising
### Wireframe
Before building anything in Excel, I planned the dashboard layout in excel, mapping out which chart goes where and why. This step ensured the final dashboard tells a logical story rather than being a random collection of visuals.
<img width="1219" height="636" alt="image" src="https://github.com/user-attachments/assets/55619386-53cf-400f-8ef4-6f5ae10f3c21" />

### Dashboard Features
The interactive dashboard includes:

  •	Total Revenue KPI 
  
  •	Total Transactions 
  
  •	Average Order Value (AOV) 
  
  •	Revenue Trend by Month 
  
  •	Revenue by Product Category 
  
  •	Transactions by Hour 
  
  •	Transactions by Day of Week 
  
  •	Top Performing Products 
  
  •	Location slicer for dynamic filtering
<img width="1252" height="636" alt="image" src="https://github.com/user-attachments/assets/f6eb06fc-3674-491d-b295-590e5b6e1913" />

## Key Insights
  •	Total revenue reached $698,812 in H1 2023, increasing from $81,678 in January to $166,486 in June, representing approximately 104% growth.
  
  •	Coffee and Tea dominated sales, contributing 38.6% and 28.1% respectively, and together accounted for 66.7% of total revenue. 
  
  •	Approximately 36.2% of all transactions occurred between 8 AM and 10 AM, indicating a strong dependence on morning peak hours. 
  
  •	Barista Espresso generated the highest revenue per order at $5.57, compared to $1.28 per order for lower-value items such as Sugar Free Syrup. 
  
  •	Revenue was evenly distributed across locations, with Hell's Kitchen contributing 33.8% ($236,511), Astoria 33.2% ($232,244), and Lower Manhattan 32.9% ($230,057). 
  
  •	Lower Manhattan recorded the highest Average Order Value at approximately $4.81, compared to $4.59 in Astoria, indicating stronger customer spend per visit. 
  
  •	Coffee and Tea combined accounted for more than two-thirds of total revenue, highlighting potential risk from heavy category concentration.

## Recommendations
  •	Maintain inventory levels and staffing to support continued growth, and monitor month-over-month performance to sustain the 104% revenue increase observed from January to June. 
  
  •	Expand and promote non-beverage product categories to reduce dependence on Coffee and Tea, which currently account for 66.7% of total revenue. 
  
  •	Increase staffing and ensure operational readiness between 8 AM and 10 AM, as this window drives 36.2% of total transactions. 
  
  •	Prioritize marketing and upselling of high-value products such as premium espresso drinks to improve revenue per order. 
  
  •	Replicate best-performing sales practices across locations to improve performance consistency and maximize revenue at each store. 
  
  •	Introduce complementary product bundles to reduce reliance on the two dominant categories and diversify revenue streams. 
  
  •	Implement upselling strategies across all locations to close the Average Order Value gap (~$0.22) and increase overall revenue.
  
## Conclusion
### The coffee can pay the rent. But only if the owner knows what the data is telling them

This project fulfilled all three brief objectives and exceeded the recommendation requirement.

Starting from 149,116 rows of raw transaction data, the analysis delivered:

  •	A clean, enriched dataset with 5 derived analytical columns
  
  •	6 structured pivot tables each answering a specific business question
  
  •	A fully dynamic Excel dashboard with interactive location filtering
  
  • Statistically backed insights with specific revenue figures and actionable recommendations

The dashboard gives any franchise owner regardless of their data background a clear, honest picture of where their revenue comes from, when their business is most vulnerable, and exactly what to do about it.

In conclusion the analysis reveals strong revenue growth and consistent performance across locations. However, the business relies heavily on morning sales and beverage categories. By optimizing staffing, improving product mix, and promoting off-peak sales, the coffee shop can further increase revenue and operational efficiency.

## Limitations
  •	H1 data only: The dataset covers January–June 2023. H2 seasonal patterns such as back-to-school, holiday season are unknown and cannot be predicted from this data alone 
  
  •	No cost data: Revenue analysis cannot be extended to profit or margin analysis such as rent, staff costs, and COGS are not in the dataset 
  
  •	No customer demographics: Individual customers are not identified, repeat purchase rate, customer lifetime value, and segmentation analysis are not possible 
  
  •	No competitor data: It is not possible to determine whether performance is strong or weak relative to similar NYC coffee shops in the same neighborhoods 
  
  •	No marketing data: Promotions, campaigns, or external events that may have driven the May–June spike are not captured

Including cost data and a full 12-month period would transform this from a performance analysis into a full profitability and forecasting model.


I am Halimat,your Business, Sales and Finacial Analyst.

  





























































  
