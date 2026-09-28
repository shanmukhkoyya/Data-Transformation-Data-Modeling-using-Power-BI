# Data Cleaning & Transformation Report

## Source Data

This package contains the raw source files used for the Power BI assignment:

- List of Orders
- Order Details
- Sales Target

## Transformation Scope

The cleaned data follows the assignment requirements:

- Restricted List of Orders to the first 500 rows.
- Prepared Order Date as a date field.
- Prepared Amount and Target as numeric/financial fields.
- Standardized CustomerName capitalization.
- Created Location in City, State format.
- Created Profit Margin from Profit / Amount.
- Created Profit Status using Loss, Break-Even, and Profit labels.
- Merged order-level and order-detail data using Order ID.
- Checked missing and duplicate data.
- Prepared supporting summary data for analysis.

## Output Files

- cleaned-data/Cleaned_List_of_Orders.csv
- cleaned-data/Cleaned_Order_Details.csv
- cleaned-data/Cleaned_Sales_Target.csv
- cleaned-data/Orders_Data.csv

## Validation Summary

- List of Orders source rows: 560
- List of Orders transformation scope: first 500 rows
- Cleaned List of Orders rows: 500
- Order Details rows: 1,500
- Sales Target rows: 36
- Orders Data rows after merge: 1,500
- Order IDs from the selected 500 orders were matched to Order Details.

## PBIX Protection

The original Power BI project file is intentionally preserved. No changes were made to the existing PBIX file.

The data package is provided separately so the source and transformed data can be reviewed without modifying the original Power BI project.
