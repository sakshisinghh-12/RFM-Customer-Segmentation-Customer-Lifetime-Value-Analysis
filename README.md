# RFM Customer Segmentation & Customer Lifetime Value Analysis

## Business Problem

This company had 5,878 customers but was allocating its retention budget without knowing which customers were actually worth retaining. The goal of this project was to segment customers based on their purchasing behaviour — how recently they bought, how often they bought, and how much they spent — and estimate the lifetime value of each segment so that marketing spend could be directed intelligently.

## Dataset

Online Retail II UCI Dataset — sourced from Kaggle.

1,067,371 transactions from a UK-based online retailer between December 2009 and December 2011.

8 columns: Invoice, StockCode, Description, Quantity, InvoiceDate, Price, Customer ID, Country.

Raw data issues handled: 243,007 rows with no Customer ID (guest checkouts), 18,744 return transactions (negative quantity), and 71 rows with zero or negative prices.

After cleaning: 805,549 transactions across 5,878 unique customers.

## Tools Used

Python (Pandas, Matplotlib, Seaborn) — data cleaning, RFM calculation, CLV estimation, visualizations

Power BI — interactive 2-page dashboard

Jupyter Notebook — development environment

## Business Recommendations
Champions (1,045 customers): These customers have a CLV of £14,765 each. Priority should be keeping them engaged — early access to new products, loyalty rewards, and personalised communication. Do not treat them like regular customers.

Loyal Customers (1,014 customers): CLV of £3,138. The goal here is upselling — they already trust the brand. Targeted product recommendations based on past purchases can increase their average order value.

At Risk (1,104 customers): CLV drops to £976 but they were once good customers. A win-back campaign with a time-limited offer is justified. Acting before they move to Lost is significantly cheaper than trying to recover a Lost customer.

Potential Loyalists (894 customers): Recent buyers who haven't bought frequently yet. A follow-up email sequence in the 2-4 weeks after their first purchase could convert many of these into Loyal Customers.

Lost (1,459 customers): CLV of £106. Aggressive spend on this group is hard to justify. A single low-cost re-engagement email is reasonable. Beyond that, marketing budget is better spent elsewhere.
