# Gift Commerce Intelligence

**Excel-based sales, customer, and fulfillment analytics for Ferns N Petals**

Explore sales performance, customer behavior, product demand, order timing, and delivery trends through an Excel-first analytics project built with **Microsoft Excel, Power Query, PivotTables, PivotCharts, slicers, and dashboard reporting**.

## Project at a glance

- **Business domain:** Gift commerce / e-commerce
- **Primary tool:** Microsoft Excel
- **Dataset:** Ferns and Petals sales dataset sourced from Kaggle
- **Focus areas:** Revenue, products, occasions, customers, order timing, and fulfillment

## Dashboard preview

![Gift Commerce dashboard reference](assets/dashboard_reference.png)

## Business questions

This project is designed to answer questions such as:

1. How much revenue does the business generate, and how does it change over time?
2. Which product categories and products contribute most to sales?
3. Which occasions drive the highest revenue?
4. At what times are orders placed most frequently?
5. Which cities contribute most to the order volume?
6. How do order quantity and delivery time relate?
7. What do customer spending patterns tell us about the business?

## Key findings

Previously recorded analysis results:

| Metric | Result |
|---|---:|
| Total orders | 1,000 |
| Unique customers | 100 |
| Products | 70 |
| Total revenue | ₹35,20,984 |
| Average delivery time | 5.53 days |
| Average order value | ₹3,520.98 |

**Metric note:** Average order value is total revenue divided by total orders. The previously calculated average revenue per unique customer was ₹35,209.84. These figures reflect the existing project analysis and have not been independently recalculated in this README update.

## Tools and techniques

- **Excel:** data exploration, formulas, PivotTables, PivotCharts, slicers, and dashboarding
- **Power Query:** data preparation and transformation
- **Data quality checks:** profile reports and validation outputs
- **Business analysis:** revenue breakdowns, product and occasion comparisons, customer metrics, and fulfillment analysis

## Repository structure

```text
gift-commerce-intelligence/
├── Gift_Commerce_Intelligence_Main.xlsx
├── data/
│   ├── Book2.xlsx
│   ├── customers.csv
│   ├── orders_fixed.csv
│   └── products.csv
├── tables/
│   ├── customer_profile.csv
│   ├── orders_enriched.csv
│   ├── product_popularity_by_occasion.csv
│   ├── quantity_vs_delivery.csv
│   ├── revenue_by_category.csv
│   ├── revenue_by_hour.csv
│   ├── revenue_by_month.csv
│   ├── revenue_by_occasion.csv
│   ├── top_10_cities.csv
│   └── top_5_products.csv
├── reports/
│   ├── dashboard_validation.csv
│   ├── data_profile.csv
│   ├── data_quality_checks.json
│   └── workbook_profile.csv
├── assets/
│   ├── dashboard_reference.png
│   └── FernsandPetalsSalesAnalysis.pdf
├── PROJECT_MANIFEST.md
└── README.md
```

## How to explore the project

1. Open `Gift_Commerce_Intelligence_Main.xlsx` in Microsoft Excel.
2. Explore the dashboard and use available slicers or filters to change the view.
3. Review the `tables/` directory for prepared analytical outputs.
4. Check the `reports/` directory for profiling and data-quality summaries.
5. Refer to the PDF and dashboard image in `assets/` for supporting project material.

## Data source and usage

The project dataset was sourced from Kaggle. Please refer to the original Kaggle dataset page for its license, attribution, and redistribution conditions. The repository retains the project’s source files and customer-level fields as provided for this analysis.

## Project outcome

This project demonstrates an end-to-end Excel analytics workflow: preparing sales data, building reusable summaries, validating key metrics, and presenting business insights in a dashboard-oriented format.
