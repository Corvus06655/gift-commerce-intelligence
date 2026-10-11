# Gift Commerce Intelligence

**Revenue, Customer & Fulfillment Analytics**

This portfolio project analyzes the Ferns and Petals sales dataset using Microsoft Excel, Power Query, PivotTables, PivotCharts, slicers, and dashboard measures.

## Public repository status

> **Privacy note:** The original customer source file contained names, phone numbers, email addresses, and postal addresses. The source customer CSV and unreviewed Excel workbooks have been removed from the current public branch. The primary workbook is therefore **not currently included** in this public version.

**Important:** Removing files from the latest commit does not remove them from earlier Git history. The repository owner should switch this repository to **Private immediately** and review/rewrite its Git history before making a sanitized public version. Do not publish the original workbook or customer-level source data unless it has been checked and all personal information has been removed.

## Project overview

The analysis covers revenue by occasion, product/category performance, order timing, customer spending, and fulfillment. The project uses Excel and Power Query; it does not require Python, Pandas, or Power BI.

## Remaining materials (review before sharing)

- `tables/`: remaining aggregate and derived analysis tables. The customer-level enriched order export was removed from the public branch; review the remaining files before redistributing.
- `reports/`: data profiles and validation reports.
- `assets/`: presentation/reference materials; inspect all pages and images for personal data before sharing.
- `PROJECT_MANIFEST.md`: project assembly and data-privacy notes.

The original workbook, source customer file, customer-linked order source, customer-level profile, and customer-identifiable enriched order export are intentionally unavailable in this public branch while the privacy review is pending. The remaining `data/` directory contains the product catalog only. The remaining reports may document historical source columns but do not contain the source contact values. Do not treat this copy as a fully reproducible workbook deliverable.

## Key findings from the prior analysis

The project analysis reported 1,000 orders, 100 customers, and 70 products, with computed revenue of ₹35,20,984 and average delivery time of 5.53 days. These are **previously recorded results**, not newly re-run results from this privacy-reduced public copy.

The earlier dashboard’s displayed average customer spend of ₹3,520.98 equals total revenue divided by total orders, so it represents average order value rather than average spend per unique customer. The prior analysis calculated a unique-customer average of ₹35,209.84.

## Before republishing

1. Make the original repository private and review its commit history for exposed personal data.
2. Create a sanitized workbook using synthetic or aggregated customer information.
3. Remove names, phone numbers, emails, addresses, customer-linked order rows, and other identifiers from source files, workbook sheets, pivot caches, hidden sheets, and exported assets.
4. Verify the source dataset's redistribution terms and document the source URL.
5. Publish only the sanitized workbook and privacy-safe derived tables after checking them.

