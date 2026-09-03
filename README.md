# Gift Commerce Intelligence

**Revenue, Customer & Fulfillment Analytics**

This repository contains a reproducible, privacy-conscious analysis of the Ferns and Petals sales dataset. It organizes the source order and product data into analysis-ready tables, checks the completeness and integrity of every supplied tabular profile, and validates the computed headline metrics against the supplied dashboard PDF.

## Project contents

| Directory | Contents |
|---|---|
| `data/` | Non-sensitive source files used for the analysis: orders and products. |
| `tables/` | Enriched orders plus revenue, product, city, customer-spend, occasion, and delivery analysis tables. |
| `reports/` | Column-level data profile, data-quality checks, and dashboard validation results. |
| `assets/` | Supplied dashboard PDF and reference image. |

## Key findings

The dataset contains **1,000 orders, 100 customers, and 70 products**. The data-quality checks found no duplicate order, customer, or product identifiers; no missing customer or product joins; no non-positive quantities; and no deliveries dated before their corresponding orders. Computed revenue is **₹35,20,984**, and the average delivery time is **5.53 days**, matching the dashboard headline values.

Revenue is highest for **Anniversary** orders at ₹6,74,634, followed by **Raksha Bandhan** at ₹6,31,585. The top five products by revenue are Magnam Set, Dolores Gift, Harum Pack, Deserunt Box, and Nostrum Box. See the CSV files under `tables/` for the complete ranked tables.

The dashboard’s displayed average customer spend of **₹3,520.98** is mathematically equal to total revenue divided by total orders, so it behaves as an average order value rather than an average spend per unique customer. The unique-customer average derived from the data is **₹35,209.84**. This distinction is recorded in `reports/dashboard_validation.csv`.

## Privacy note

The supplied `customers.csv` and `Book2.xlsx` contain direct customer contact and address fields. They were used for validation but are **not copied into this repository**. The uploadable customer profile table contains only synthetic customer IDs, gender, order counts, quantities, revenue, and average order value. Do not commit raw customer contact information or addresses to a public repository.

## Reproducing the outputs

The generated CSV outputs are static analysis deliverables created from the supplied files. The original processing script is retained outside the repository because it contains sandbox-specific input paths. To reproduce the analysis in another environment, adapt the script to point to the two source files in `data/`, load the withheld customer file locally, and regenerate the tables and reports.

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

