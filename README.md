## Sales-Data-Analysis-Dashboard

## Problem Statement

This dashboard helps business stakeholders understand overall sales performance and identify key trends across time, regions, products, and customers.
It enables decision-makers to track revenue growth, sales quantity, and profitability, helping them focus on high-performing segments and improve underperforming areas.

### Business Requirement

1) Top/Bottom 5 product by Sales/Profit/Quantity Sold.
2) How do sales trends vary over time (daily, monthly, quarterly, annually) ?
3) Show relationship between sales & profit.
4) Compare sales/profit/quantity sold between any two periods selected by the user.
5) Average discount offered in each discount category.
6) Total number of orders.
7) Show Sales/Profit/Discount/Net Sales/All remaining fields for each order that could be filtered using visual filters. (Product/Date/Customer ID/Promotion Categories)
8) Show sales by different cities.

By using this dashboard, the organization can:

- Monitor sales trends over time

- Identify top-performing products and regions

- Analyze customer contribution to revenue

- Support data-driven sales strategy decisions

## Steps followed

Step 1 : Loaded sales dataset into Power BI Desktop.

Step 2 : Opened Power Query Editor and enabled:

- Column distribution

- Column quality

- Column profile

Step 3 : Enabled column profiling based on entire dataset.

Step 4 : Checked for missing values and data inconsistencies in sales, quantity, and date columns.

Step 5 : Cleaned and transformed data by:

- Correcting data types

- Removing null/duplicate values

Step 6 : Created relationships between sales, product, and customer tables (if applicable).

Step 7 : Selected an appropriate theme in Report View.

Step 8 : Added slicers for:

- Date

- Region

- Product Category

- Customer Segment

Step 9 : Created KPI card visuals for:

- Total Sales

- Total Quantity Sold

- Total Profit

- Average Order Value

Step 10 : Added bar and line charts for:

- Sales by Region

- Sales by Product Category

- Monthly / Yearly Sales Trend

Step 11 : Used table and matrix visuals to analyze detailed sales breakdown.

Step 12 : Created calculated columns for time-based analysis (Year, Month).

Step 13 : Created DAX measures for business KPIs.

Step 14 : Added text boxes, shapes, and icons for better dashboard layout.

Step 15 : Final dashboard was published to Power BI Service.

## DAX Measures Used
`Total Sales = SUM(Sales[Sales_Amount])`

`Total Quantity = SUM(Sales[Quantity])`

`Total Profit = SUM(Sales[Profit])`

`Average Order Value = 
DIVIDE([Total Sales], DISTINCTCOUNT(Sales[Order_ID]))`

## Snapshot of Dashboard (Power BI Service)

<img width="1365" height="735" alt="FullPage" src="https://github.com/user-attachments/assets/c06fb0de-8a89-4a43-b7ff-85a2c655a21b" />

## Model View : Star Schema

<img width="805" height="450" alt="ModelView" src="https://github.com/user-attachments/assets/c69ddaaf-5a19-439d-bb0c-9a4a1e7a355f" />

## Report Snapshot (Power BI Desktop)

<img width="876" height="487" alt="Home" src="https://github.com/user-attachments/assets/6f0709e0-e2f8-4ec5-b133-b11bc68cd7b6" />

<img width="872" height="488" alt="OverView" src="https://github.com/user-attachments/assets/6cd8963e-c024-4821-a19f-941497ed7229" />

<img width="873" height="485" alt="Sales_Profit_QTY" src="https://github.com/user-attachments/assets/b062f133-de16-46dd-87e4-07d8ae7b6b0a" />

<img width="872" height="484" alt="Top_Bottom" src="https://github.com/user-attachments/assets/ae159853-a586-4bf3-9250-6ef799adc23a" />

<img width="874" height="488" alt="Tabel_View" src="https://github.com/user-attachments/assets/c0571292-c242-4d83-bc0c-06fc580ddf64" />

## Insights

A single-page interactive report was created using Power BI Desktop.

Following insights can be drawn from the dashboard:

[1] Sales Performance

- Sales show a clear growth trend over time.

- Certain months contribute significantly higher revenue, indicating seasonality.

[2] Regional Analysis

- Some regions outperform others in both sales and profit.

- Underperforming regions present opportunities for targeted improvement.

[3] Product Analysis

- A small number of product categories generate the majority of revenue.

- Low-performing products can be reviewed for pricing or promotion strategies.

[4] Customer Insights

- High-value customers contribute a major share of total sales.

- Customer segmentation helps identify loyal and repeat buyers.

[5] Profitability

- Not all high-sales products generate high profit.

- Profit analysis helps optimize discount and cost strategies.

## Tools & Technologies

- Power BI Desktop – Data modeling & dashboard development

- Power BI Service – Report publishing & sharing

- DAX – KPI and measure creation

- Power Query – Data cleaning & transformation

- Figma – Dashboard UI/UX design and layout planning

- CSV / Structured Sales Dataset

## Conclusion

This Sales Data Analysis dashboard provides a comprehensive view of business performance, enabling stakeholders to make informed, data-driven decisions.
It helps identify growth opportunities, optimize sales strategies, and improve overall profitability.
