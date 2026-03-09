# Power-BI-Project-Bakery-Sales-Analysis
Built a Power BI bakery sales dashboard using a star schema model with orders + line items merged into a single Sales fact table.  Implemented a custom Date table, DAX measures (Sales, Order Count, YoY change), and dynamic “Top by” analysis using field parameters. 

# Bakery Sales Dashboard (Power BI)

A Power BI dashboard built with semi-realistic bakery sales data to demonstrate best practices in data modeling, DAX measures, and report design.

## Overview
This project analyzes bakery sales performance across time, products, stores, and employees. The dataset is structured like real transactional systems using a **Sales Orders (header)** table and a **Sales Order Lines (line items)** table, then merged to form a clean **Sales fact table** for a proper **star schema** model.

## Key Features
- **Star schema data model** (Sales fact + dimension tables)
- **Merged header + line items** to support filtering by product/date correctly
- **Custom Date table** (supports time intelligence + relative periods)
- Core DAX measures:
  - Sales Amount
  - Count of Sales (distinct orders)
  - Current Year vs Last Year Sales
  - Year-over-Year (YoY) % change + arrow label
- **Field Parameters** for dynamic “Top by” analysis (Store / Category / Flavor / Salesperson)
- Conditional formatting:
  - Heatmap-style matrix for seasonality patterns
  - Highlighting top category in bar chart
  - Red/green YoY labels
- Clean UI styling with theme import, layout cards, and sparklines

## Data
Data is provided as CSV/text files and includes:
- Sales Orders (header)
- Sales Order Lines (line items)
- Products
- Stores
- Employees
- Sales Goals
- Date table script (`date.txt`)

> Note: Names and email addresses are fictitious and used for learning purposes.



## Dashboard Insights (examples)
- Identifies busiest months and weekdays using a heatmap matrix
- Shows top-performing store/category/flavor/salesperson dynamically
- Tracks YoY performance with clear up/down indicators

## Tech Stack
- Power BI Desktop
- Power Query (data prep + merge)
- DAX (measures + time intelligence)
- Field Parameters (dynamic dimensions)

## Project Structure
- `/data/` — CSV files (sales, products, stores, employees, goals)
- `/date/` — `date.txt` script for the Date table
- `BakerySalesDashboard.pbix` — Power BI report file (if included)

## Credits
Dashboard workflow inspired by common Power BI modeling patterns (star schema, header/line item merge, and time intelligence).
