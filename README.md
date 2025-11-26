📊 Profitability, Sales & Returns Analytics Dashboard (Power BI)

📌 Project Overview

This project is an end-to-end Business Intelligence analytics solution built using Power BI, focused on analyzing sales performance, profitability, customer behavior, and product returns across multiple business dimensions.

The dashboard simulates a real-world enterprise reporting scenario using a structured star schema, advanced DAX measures, and interactive visuals to support data-driven decision-making across Sales, Pricing, Operations, and Management teams.

🎯 Business Objectives

The primary goals of this project were to:

Analyze overall sales and margin performance

Identify high- and low-margin products

Understand regional and customer-level performance

Monitor returns behavior and operational issues

Provide executive-level KPIs with drill-down capabilities

🗂 Dataset Description

Synthetic datasets (7 tables) were used to simulate an ERP-style analytics environment.

Tables Used:

Sales – transactional sales data

Customers – customer master with segments & regions

Products – product master with pricing & categories

Regions – geographic hierarchy

SalesReturns – return transactions with reasons

SalesTargets – regional targets

Calendar_New – custom date dimension for time intelligence

🧱 Data Model (Star Schema)

The project uses a proper star schema with:

Sales as the central fact table

Dimensions: Customers, Products, Regions, Calendar

Separate fact table for SalesReturns

Relationships:

Customers (1) → Sales (*)

Products (1) → Sales (*)

Regions (1) → Customers (*)

Calendar_New (1) → Sales (*)

Sales (1) → SalesReturns (*)

This ensures:

Correct filtering behavior

Accurate aggregations

Scalable analytics design

📐 Key Metrics & KPIs

Sales & Profitability

Total Sales

Total Margin

Margin %

Average Unit Price

Customer Count

Top Customers

Low Margin Products

Returns & Operations

Total Returns

Return Rate (%) – based on orders

Return Frequency Index – % of customers with returns

Return Rate by Region

Product Return Heatmap

Return Reasons Breakdown

🧠 DAX Highlights

The project includes advanced DAX measures, such as:

Context-aware margin calculations

Return rate logic using distinct orders

Customer-derived return frequency (via RELATED)

Time intelligence (YTD, MTD, YoY)

Share-of-total calculations using ALL()

All measures are grouped logically (Sales, Margin, Returns, Time Intelligence) following BI best practices.

📊 Dashboard Pages
Page 1 — Executive Sales Overview

Sales, margin, and customer KPIs

Monthly revenue trend

Top customers

Low-margin products

Page 2 — Product & Pricing Analysis

Product profitability comparison

Price vs margin analysis

Category-level insights

Page 3 — Regional & Customer Analytics

Sales by region

Region contribution %

Customer segment performance

Target vs actual analysis

Page 4 — Returns & Operations Analytics

Total returns & return rate

Return trends over time

Return frequency index

Product return heatmap

Return reasons analysis

✅ Data Validation & Quality Checks

Cross-verified totals across pages (Sales = €2.43M, Margin ≈ 33.4%)

Validated margin logic at product, customer, and total levels

Confirmed correct calendar sorting and date filtering

Ensured no orphaned records or broken relationships

Validated return metrics against order-level data

🛠 Tools & Technologies

Power BI Desktop

DAX

Power Query

Star Schema Data Modeling

Excel (data sources)

📌 Key Learnings

Designing robust star schemas is critical for scalability

Context in DAX (row vs filter) directly impacts KPI accuracy

Return analytics require different definitions at order, product, and customer levels

Data validation is essential before publishing analytics

🚀 How to Use

Download the .pbix file

Open in Power BI Desktop

Explore dashboards using slicers and filters

Review measures in the “Measures” table

👤 Author

Roshan Patole
Business Intelligence Developer | Data Analyst
