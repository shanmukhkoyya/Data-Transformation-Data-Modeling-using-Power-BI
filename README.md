# Sales Data Model | Power BI Case Study

<div align="center">

**FROM THREE SOURCE FILES TO ONE ANALYTICAL MODEL**

POWER QUERY · POWER BI · DAX

</div>

## Executive snapshot

This project prepares order, order-detail and sales-target data for analysis. The goal is to review sales, profit, margin and target achievement together rather than judging performance from sales alone.

| Dataset / KPI | Documented value |
|---|---:|
| Source order rows | 560 |
| Order rows selected for transformation | 500 |
| Order-detail rows | 999 |
| Sales-target rows | 36 |
| Unique orders in merged data | 343 |
| Total sales | 283,497 |
| Total profit | -444 |
| Overall profit margin | -0.16% |

The order transformation intentionally selects the first 500 rows of the source List of Orders file, as documented in this project.

## Source-to-model map

| Source | Prepared output | Role |
|---|---|---|
| [List of Orders](raw-data/List_of_Orders.csv) | [Cleaned List of Orders](cleaned-data/Cleaned_List_of_Orders.csv) | Order-level attributes |
| [Order Details](raw-data/Order_Details.csv) | [Cleaned Order Details](cleaned-data/Cleaned_Order_Details.csv) | Product, quantity, sales and profit |
| [Sales Target](raw-data/Sales_Target.csv) | [Cleaned Sales Target](cleaned-data/Cleaned_Sales_Target.csv) | Monthly category targets |

The merged analytical output is [Orders Data](cleaned-data/Orders_Data.csv).

## Transformation notes

Power Query preparation includes date and numeric type handling, customer-name standardisation, a combined City–State field, profit-margin and profit-status calculations, an Order ID merge, and checks for missing and duplicate data.

## Model architecture

The repository documents eight analytical tables:

1. Sales target
2. Order Details
3. List of Orders
4. Orders Data
5. Category Average Profit
6. Monthly Sales Target
7. Order Details Summary
8. Sub-Category Total Amount

![Documented Power BI data model](images/data-model-architecture.svg)

See [Data Model Documentation](docs/Data_Model_Documentation.md) for the table-level explanation.

## What the analysis shows

| Category | Sales | Profit | Target achievement |
|---|---:|---:|---:|
| Electronics | 108,430 | 682 | 84.05% |
| Clothing | 96,641 | 2,387 | 55.54% |
| Furniture | 78,426 | -3,513 | 59.01% |

Clothing has the highest category profit in this prepared dataset, while Electronics has the highest sales. Furniture records a loss. The figures illustrate why sales and profitability need to be interpreted together.

Other documented observations include a -4,640 result for the Tables sub-category and a -1,438 result for Saree despite its 42,375 sales.

## Report artifact

![Static dashboard layout concept](images/Business_Dashboard.svg)

<sub>This SVG is a layout concept, not a screenshot from Power BI Desktop. The editable report is the PBIX file below.</sub>

**[Open the Power BI report](Data%20Transformation%20%26%20Data%20Modeling%20using%20Power%20BI.pbix)**

## Supporting documentation

- [Data Cleaning Report](docs/DATA_CLEANING_REPORT.md)
- [Data Model Documentation](docs/Data_Model_Documentation.md)
- [Business Analysis](docs/Business_Analysis.md)

## Reproduce the analysis

1. Review the three source files in raw-data/.
2. Inspect the prepared CSV files in cleaned-data/.
3. Open the PBIX in Microsoft Power BI Desktop.
4. Review Power Query steps, model relationships, measures and report filters.
5. Compare report outputs with the documented figures.

## Interpretation limits

The results describe the supplied assignment data, not a live company. Category comparisons are descriptive and do not explain why profit or loss occurred. The documented model and calculations should be inspected in Power BI before treating the report as independently validated.

---

**Author:** Shanmukh Koyya · [GitHub](https://github.com/shanmukhkoyya) · [LinkedIn](https://www.linkedin.com/in/shanmukh-koyya/) · [Email](mailto:shanmukhkoyya1234@gmail.com)
