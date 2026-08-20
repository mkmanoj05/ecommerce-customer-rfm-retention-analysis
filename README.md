# ecommerce-customer-rfm-retention-analysis
E-commerce customer analysis using Python, SQL and Power BI with RFM segmentation and cohort retention analysis.
# E-Commerce Customer Analytics

## Project Overview

This project analyzes e-commerce customer transactions to understand sales performance, customer behavior, customer value and retention.

I used Python for data cleaning and exploratory analysis, SQL for customer analysis, RFM segmentation and cohort retention analysis, and Power BI to build an interactive dashboard.

## Business Questions

- How much revenue does the business generate?
- How many customers and orders does the business have?
- Which countries generate the most revenue?
- Which customers are the most valuable?
- Which customers are loyal or at risk?
- How are customers distributed across RFM segments?
- How well does the business retain customers after their first purchase?

## Tools Used

- Python
- Pandas
- NumPy
- SQL
- SQLite
- Power BI
- Excel

## Project Workflow

Raw Data
↓
Python Data Cleaning
↓
Exploratory Customer Analysis
↓
SQL Analysis
↓
RFM Segmentation
↓
Cohort Retention Analysis
↓
Power BI Dashboard

## Data Cleaning

The dataset was checked for:

- Missing Customer IDs
- Cancelled invoices
- Negative quantities
- Invalid/zero prices
- Duplicate records

A Revenue column was created using:

Revenue = Quantity × Unit Price

Only valid customer transactions were used for the customer-level analysis.

## RFM Analysis

RFM analysis was performed in SQL using:

- Recency — how recently a customer purchased
- Frequency — how often a customer purchased
- Monetary — how much a customer spent

Customers were scored from 1 to 5 for each RFM component using SQL window functions.

Based on the RFM scores, customers were grouped into segments such as:

- Champions
- Loyal Customers
- Potential Loyalists
- At Risk
- Lost Customers
- Other

## Customer Retention Analysis

Cohort analysis was performed in SQL by:

1. Identifying each customer's first purchase month.
2. Assigning customers to monthly cohorts.
3. Tracking customer activity in subsequent months.
4. Calculating retained customers.
5. Calculating retention percentage.

The results were visualized in Power BI using a cohort retention heatmap.

## Power BI Dashboard

### Page 1 — Customer & Sales Overview

- Total Revenue
- Total Customers
- Total Orders
- Units Sold
- Average Order Value
- Monthly Revenue Trend
- Revenue by Country

### Page 2 — RFM Customer Segmentation

- Customer Segments
- Revenue by Customer Segment
- RFM Score Distribution
- Customer-level RFM details

### Page 3 — Customer Retention

- Cohort Retention Heatmap
- Customers Retained Over Time
- Cohort filtering

## Key Skills Demonstrated

- Data cleaning
- Exploratory data analysis
- SQL CTEs
- SQL window functions
- NTILE()
- Customer segmentation
- RFM analysis
- Cohort analysis
- Retention analysis
- Data visualization
- Power BI dashboard development
- Business-oriented analysis

## Project Structure

```text
Ecommerce-Customer-Analysis/
│
├── data/
├── python/
├── sql/
├── powerbi/
├── dashboard pdf/
└── README.md
