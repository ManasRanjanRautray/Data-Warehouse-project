# Datawarehouse and Analytics Project

A SQL-based data warehouse that brings raw data from multiple sources into one
clean, organised model, so that KPIs and reports can be produced quickly.

## Overview
Raw data is often messy and spread across different files and tables. This
project cleans and transforms it using SQL, and loads it into a star schema
designed for fast reporting and decision-making.

- Integrates [number] datasets/sources: [e.g. CRM data, ERP sales data]
- ETL workflows written in SQL using CTEs, joins and functions
- Star schema with optimized fact and dimension tables
- Reporting queries for KPIs such as [total sales, monthly trend, top customers]

## Tech Stack
- SQL Server, T-SQL
- SQL Server Management Studio (SSMS)
- Git and GitHub


## Architecture / Data Flow
Source data -> Staging (raw copy) -> Cleaning and transformation -> Warehouse
(star schema) -> KPI reports

## Data Model (Star Schema)
- **Fact table:** [e.g. fact_sales] with measures such as [quantity, sales amount]
- **Dimension tables:** [e.g. dim_customer, dim_product, dim_date]

## ETL Process
1. **Extract:** load raw data from [CSV files / source tables] into staging tables.
2. **Transform:** remove duplicates, handle NULLs, fix data types and date formats,
   standardise names, and join the sources.
3. **Load:** insert the cleaned data into the dimension and fact tables.

## Example KPI Queries
```sql
-- [Paste one real query from your project, e.g. monthly sales]
```

## Project Structure
```
datasets/      raw source files
scripts/       SQL scripts (staging, cleaning, dimensions, fact, reports)
docs/          data model diagram
README.md
```

## How to Run
1. Install SQL Server and SSMS.
2. Create the database and run the scripts in the `scripts/` folder in order.
3. Run the report queries to see the KPIs.

## What I Learned
- Designing a star schema with fact and dimension tables
- Writing ETL logic in SQL with CTEs, joins and functions
- Checking data quality (duplicates, NULLs, row counts)

## Future Improvements
- Incremental loading and scheduling
- Data quality checks
- A dashboard for visualisation

## Author
Manas Ranjan Rautray
[LinkedIn](https://www.linkedin.com/in/manas07) | [LeetCode](https://leetcode.com/u/ManasRanjan7/)
