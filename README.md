# Gift Commerce Intelligence

**Revenue, Customer & Fulfillment Analytics**

This repository contains an Excel-based analysis of the Ferns and Petals sales dataset. The project uses **Microsoft Excel, Power Query, PivotTables, PivotCharts, slicers, and Excel dashboard measures** to analyze revenue, customer behavior, product performance, and fulfillment. No Python, Pandas, or Power BI is used in this project.

## Start here: primary project file

> **Open `Gift_Commerce_Intelligence_Main.xlsx` first.** This is the main deliverable and contains the Excel workbook with the dashboard, measures, pivot outputs, slicers, and the project’s analysis model. The original workbook is also retained as `data/Book2.xlsx` for traceability.

An interviewer can review the project in this order: open the main workbook, read the dashboard and workbook sheets, inspect the source data in `data/`, and then review the supporting tables and quality reports in `tables/` and `reports/`.

## Project contents

| Location | Contents |
|---|---|
| `Gift_Commerce_Intelligence_Main.xlsx` | **Primary Excel deliverable** containing the dashboard, measures, pivots, slicers, and analysis model. |
| `data/` | Complete supplied source files: `Book2.xlsx`, `customers.csv`, `orders_fixed.csv`, and `products.csv`. |
| `tables/` | Enriched orders plus revenue, product, city, customer-spend, occasion, and delivery analysis tables. |
| `reports/` | Column-level data profiles, workbook sheet profile, data-quality checks, and dashboard validation results. |
| `assets/` | Supplied dashboard PDF and reference image. |

## Key findings

The dataset contains **1,000 orders, 100 customers, and 70 products**. The data-quality checks found no duplicate order, customer, or product identifiers; no missing customer or product joins; no non-positive quantities; and no deliveries dated before their corresponding orders. Computed revenue is **₹35,20,984**, and the average delivery time is **5.53 days**, matching the dashboard headline values.

Revenue is highest for **Anniversary** orders at ₹6,74,634, followed by **Raksha Bandhan** at ₹6,31,585. The top five products by revenue are Magnam Set, Dolores Gift, Harum Pack, Deserunt Box, and Nostrum Box. See the CSV files under `tables/` for the complete ranked tables.

The dashboard’s displayed average customer spend of **₹3,520.98** is mathematically equal to total revenue divided by total orders, so it behaves as an average order value rather than an average spend per unique customer. The unique-customer average derived from the data is **₹35,209.84**. This distinction is recorded in `reports/dashboard_validation.csv`.

## Data and privacy note

The complete supplied files are included because this is a private portfolio repository and the Excel workbook is the primary project deliverable. The customer source file contains contact and address fields; do not make this repository public or reuse those fields outside the intended interview review. The derived customer profile table remains privacy-reduced and contains analytical fields rather than names, phone numbers, emails, or addresses.

## How to review the project

The workbook is the source of truth for the dashboard and Excel measures. The CSV files under `data/` are the supplied source tables, while the CSV files under `tables/` and `reports/` are supporting analysis and validation outputs prepared for review. The project’s analytical workflow is Excel and Power Query based; no Python or Pandas pipeline is required to open or understand the main deliverable.

## Data dictionary

| Table | Purpose |
|---|---|
| `orders_enriched.csv` | Orders joined to product attributes and derived date, time, delivery, and revenue fields. |
| `revenue_by_occasion.csv` | Orders, quantity, and revenue summarized by occasion. |
| `revenue_by_category.csv` | Orders, quantity, and revenue summarized by product category. |
| `revenue_by_month.csv` | Monthly revenue for 2023. |
| `revenue_by_hour.csv` | Order volume and revenue by order hour. |
| `top_5_products.csv` | Five highest-revenue products. |
| `top_10_cities.csv` | Ten cities ranked by order count. |
| `customer_profile.csv` | Privacy-reduced customer spending profile. |
| `product_popularity_by_occasion.csv` | Product performance within each occasion. |
| `quantity_vs_delivery.csv` | Delivery-time comparison by ordered quantity. |

