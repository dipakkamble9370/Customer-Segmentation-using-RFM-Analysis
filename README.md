Customer Segmentation using RFM Analysis
Overview:
A behavioral customer segmentation project using RFM (Recency, Frequency, Monetary) analysis on e-commerce transaction data, identifying which customers drive the majority of revenue and which are at risk of churning.

Objective:
Segment customers by purchasing behavior to find high-value customers worth retaining and at-risk customers worth re-engaging before they're lost entirely.

Dataset:
~3,383 transaction line items across 1,122 invoices from 180 customers, structured similarly to the UCI "Online Retail" dataset
Fields: InvoiceNo, StockCode, Description, Quantity, InvoiceDate, UnitPrice, CustomerID, Country

Tools Used:
Python (pandas) — data cleaning, RFM calculation, quintile scoring, segment labeling
Power BI — segment visualization and revenue concentration analysis

Approach:
Cleaned transaction data — removed cancelled orders, missing CustomerIDs, and non-positive quantities/prices
Calculated Recency (days since last purchase), Frequency (number of unique invoices), and Monetary (total spend) per customer
Scored each metric into quintiles (1–5) and summed them into a combined RFM score
Mapped RFM scores to five behavioral segments: Champions, Loyal Customers, At Risk, Hibernating, Lost
Visualized segment size and revenue concentration in Power BI using bar charts and a Recency-vs-Monetary scatter plot colored by segment
