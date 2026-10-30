# Blinkit Grocery Sales & Outlet Performance Analytics

An end-to-end data analytics capstone exploring grocery sales, product-category performance, and outlet performance using **Microsoft Excel** and **Power BI**.

**Author:** Uday Dubey  
**Tools:** Excel · Power BI · DAX  
**Dataset:** Blinkit grocery item-outlet data

---

## Business Problem

Blinkit operates 10 outlets across Tier 1, Tier 2, and Tier 3 cities, stocking 1,559 items across 16 product categories. The business problem described in this case study is the lack of a consolidated view of sales, category performance, item ratings, and outlet age to support merchandising and expansion decisions.

## Project Scope

- **8,523** item-outlet records
- **10** unique outlets
- **1,559** distinct item identifiers
- **16** product categories
- **3-page** interactive Power BI report

## Tools & Workflow

| Stage | Tool | Work |
|---|---|---|
| Data cleaning | Microsoft Excel | Data inspection, standardization, missing-value treatment |
| Data modelling & analysis | Power BI | KPI measures, comparisons, trends, and interactive analysis |
| Calculations | DAX | Measures used across report pages |
| Communication | PDF case study | Business problem, methodology, findings, and recommendations |

## Data Cleaning

The case study documents these preparation steps:

1. Standardized inconsistent item-fat-content labels into **Low Fat** and **Regular**.
2. Treated missing item weights by using values from the same item where available, then category medians.
3. Treated zero item-visibility values as missing rather than as literal zero visibility.
4. Calculated outlet age using a fixed **2023** reference year.

## Power BI Report

The report is organized into three analytical pages:

### 1. Executive Summary
Sales KPIs, sales by outlet establishment year, sales by rating, leading product categories, outlet type, and outlet location tier.

### 2. Product & Outlet Analysis
Sales by item fat content, outlet size, and item type, along with sales versus item visibility by outlet type.

### 3. Outlet Performance
Average sales per outlet, average rating by outlet, sales by outlet identifier, and an outlet-by-item-category detail table.

## Business Questions & Findings

### Which outlet formats and locations drive sales?
The case study reports that **Supermarket Type 1 contributes 65.5% of total sales**. Tier 3 cities lead Tier 2 and Tier 1 in the location-tier comparison.

### Which categories over- or under-perform their shelf visibility?
The sales-share versus visibility-share index in the case study highlights:
- **Household:** 1.15x
- **Health & Hygiene:** 1.11x
- **Breakfast:** 0.78x
- **Baking Goods:** 0.85x

### Do item rating and visibility predict sales?
The case study reports negligible correlations:
- Sales and item rating: **0.011**
- Sales and item visibility: **0.001**

### How does outlet age relate to performance?
The case study reports a weak negative correlation of **-0.25**.

## Recommendations

1. Prioritize **Supermarket Type 1** in **Tier 3** cities for the next expansion round.
2. Reallocate shelf space from Breakfast and Baking Goods toward Household and Health & Hygiene, while validating the change against local demand.
3. Avoid treating rating and visibility as primary merchandising KPIs; focus review effort on category mix and outlet-format fit.

## Dataset Total — Validation Note

The uploaded cleaned Excel workbook contains 8,523 records. Summing its `Sales` column gives **1,201,681.66**. The first-page KPI in the supplied PDF appears to show **1,20,168**, while the detailed analysis and dashboard show approximately **1.20M**. The workbook sum is the value independently calculated from the uploaded dataset; the PDF cover KPI should be corrected to match before external publication.

## Repository Files

The following project deliverables are available in the repository root:

| File | Description |
|---|---|
| `Blinkit Cleaned Dataset.xlsx` | Cleaned dataset used for analysis |
| `blinkit Report.pbix` | Interactive Power BI dashboard |
| `BlinkITCase Study Report.pdf` | Case study summary, findings, and recommendations |

## How to Use

1. Download `Blinkit Cleaned Dataset.xlsx` to inspect the cleaned data.
2. Open `blinkit Report.pbix` in Power BI Desktop.
3. Use the report slicers to explore outlet size, establishment year, item fat content, and location type.
4. Read `BlinkITCase Study Report.pdf` for the business problem, data-cleaning summary, findings, and recommendations.

## Author

**Uday Dubey**  
BBA Finance Student | Aspiring Data Analyst

---

*This is an academic portfolio case study. Findings and recommendations are based on the supplied dataset and the accompanying case study analysis.*
