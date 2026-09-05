# Retail Semantic & Visualisation Layer (Tableau)

An interactive Tableau dashboard for exploring customer behaviour, sales performance and revenue using retail data transformed with dbt and Snowflake.

## Live Dashboard

[View Dashboard on Tableau Public](https://public.tableau.com/views/RetailAnalyticsDashboardCoffeeShop/RetailAnalyticsDashboardCoffeeShop)

## Dashboard Preview

![Retail Analytics Dashboard](dashboard.png)

## What the Dashboard Shows

Five interactive visualisations answering key business questions:

- **Monthly Revenue Trend**: How does revenue change month over month?
- **Top 10 Customers by Lifetime Value**: Who are the highest-value customers?
- **Order Status Breakdown**: What proportion of orders are complete vs. returned?
- **Revenue by Payment Method**: Which payment methods drive the most revenue?
- **Customer Order Frequency**: How many orders do customers typically place?

## Data Source

Data sourced from the mart layer of the [retail-analytics-dbt](https://github.com/tessogamba/retail-analytics-dbt) project:

| Table | Description | Rows |
|-------|-------------|------|
| `fct_orders` | Order transactions with payment details | 99 |
| `dim_customers` | Customer profiles with aggregated order metrics | 100 |

Raw data modelled using dbt on Snowflake; staging and mart layers with 18 passing data quality tests.

## Sample Insights Surfaced

- Credit card dominates revenue at £2,132 vs coupon at £1,688
- Revenue peaked in January 2018 at £952, declining to £114 by May
- Kathleen is the highest value customer at £398 lifetime spend
- 97% order completion rate with only 2 returns
- 70 customers placed zero orders, suggesting an acquisition without conversion opportunity

## Tools

Tableau Public, Microsoft Excel, SQL, dbt, Snowflake

## Related Projects

- [case-management-analytics-platform](https://github.com/tessogamba/case-management-analytics-platform) - Production SQL Server-to-Power BI analytics platform with dimensional modelling, DAX and governed data-quality controls
- [retail-analytics-dbt](https://github.com/tessogamba/retail-analytics-dbt) - dbt and Snowflake transformation project that produced the dashboard datasets
- [financial-analytics-bigquery](https://github.com/tessogamba/financial-analytics-bigquery) - Financial analytics project using BigQuery and reusable SQL models across 12 public companies and 23 metrics
- [financial-analytics-looker-studio](https://github.com/tessogamba/financial-analytics-looker-studio) - Looker Studio dashboard for exploring financial growth, profitability and risk

---
*Built by Tess Ogamba · [github.com/tessogamba](https://github.com/tessogamba) · [LinkedIn](https://linkedin.com/in/tessogamba)*
