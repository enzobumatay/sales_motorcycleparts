# Analyzing Motorcycle Part Sales
This project analyzes motorcycle parts sales data to understand revenue performance across product lines, warehouses, customer segments, payment methods, and time. Using SQL, the analysis identifies key sales drivers, performance trends, and growth opportunities to support data-driven decisions that can improve overall revenue performance.

The analysis is guided by the following overall business question:
_How can the company identify its strongest sales drivers and growth opportunities to improve revenue performance across product lines, warehouses, customer segments, and time?_

## Business Questions
To address the overall business question, the analysis was divided into eight supporting business questions covering product, warehouse, customer, payment, and time-based performance:
_Analyze Sales Performance_
1. Which product lines generate the most revenue?
2. Which warehouses have the best sales performance?
3. How do Wholesale and Retail sales compare?
4. How does sales revenue change month-to-month?
_Identify Sales Drivers_
5. Which payment methods generate the most sales and incur the highest payment fees?
6. How much is Wholesale net revenue each product line generated per month per warehouse?
7. Which product line and warehouse combinations generate the highest net revenue each month?
_Identify Growth Opportunities_
8. Which product lines have the highest month-over-month revenue growth?

Together, these questions provide a progression from understanding overall sales performance, to identifying the factors driving revenue, and finally to finding areas with potential for growth.

## Dataset
The analysis uses a single sales table containing transactional sales records from June to August 2021.

The table contains information on:

Order: order_number, date
Sales dimensions: product_line, warehouse, client_type, payment
Sales measures: quantity, unit_price, total, payment_fee

The dataset represents individual sales transactions, allowing revenue performance to be analyzed across different product lines, warehouses, customer segments, payment methods, and months.

## Data Quality Assessment
Before conducting the SQL analysis, the dataset was assessed to determine whether it was reliable enough to answer the business questions.

The assessment covered:
Missing or NULL values
Data types
Column structure
Order number format
Categorical values
Date values
Potential inconsistencies in the data

The inspection found no NULL values requiring treatment, and the available values and data types were suitable for the planned analysis. No data-cleaning transformation was required before proceeding to the SQL analysis.

## Analysis and Key Findings
The analysis begins by looking at where revenue is coming from. Among the product lines, Suspension & Traction is the strongest revenue contributor, followed by Frame & Body and Electrical System. This establishes the company's primary product-line drivers and provides a starting point for understanding overall sales performance.

``<img width="527" height="210" alt="image" src="https://github.com/user-attachments/assets/ea9c7d73-14e6-49a0-8065-f6f63b77ac2f" />

Revenue performance also varies significantly across warehouses. Central generates the highest revenue at $141,982.88, followed by North at $100,203.63 and West at $46,926.49. This suggests that sales performance is not evenly distributed across locations, making warehouse-level performance an important factor when identifying opportunities for improvement.

``<img width="334" height="133" alt="image" src="https://github.com/user-attachments/assets/ef2784b5-4a43-45fa-aacf-1e54d17d450e" />

Looking at customer segments, Wholesale generates $159,642.33, compared with $129,470.67 from Retail. Wholesale therefore represents the larger revenue contributor, indicating that customer type plays an important role in the company's overall sales performance.

``<img width="453" height="106" alt="image" src="https://github.com/user-attachments/assets/4562d431-e32b-4b1c-98ef-2d0683873668" />

Monthly revenue dipped slightly in July before recovering in August, suggesting a positive recent trend. Further analysis of payment methods, product–warehouse performance, and monthly growth helps identify where revenue is being generated most efficiently and which product lines show the strongest growth potential.

``<img width="706" height="127" alt="image" src="https://github.com/user-attachments/assets/98b7c18a-8841-4aff-aa0c-7e9c5fead797" />

A more detailed view of Wholesale net revenue reveals how individual product lines perform across months and warehouses. This helps identify where the company's strongest combinations of product, location, and customer segment are concentrated. Comparing these combinations month by month provides a more targeted view of where revenue is being generated most efficiently.

``<img width="850" height="576" alt="image" src="https://github.com/user-attachments/assets/c0feac8f-b797-4b3a-82e5-0222cb5ddd06" />

Overall, the findings point to opportunities to strengthen top-performing products and locations while identifying high-growth areas for further revenue expansion.

## Overall Business Insight
Suspension & Traction, the Central warehouse, and Wholesale customers are the company's strongest revenue drivers. The company can build on these strengths while addressing opportunities in the North and West warehouses and prioritizing product lines with strong month-over-month growth to further improve revenue performance.

## Technology
SQL | PostgreSQL

## Skills
SQL Aggregations & Filtering | SQL CTEs & Window Functions
Descriptive Analysis
Data Storytelling
