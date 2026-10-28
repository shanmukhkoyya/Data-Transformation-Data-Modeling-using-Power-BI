# Data Transformation & Data Modeling with Power BI

**Tools:** Power BI Desktop · Power Query · DAX

This project prepares related sales tables for analysis and documents data cleaning, transformation, data modelling, and analysis of sales targets and profitability.

## Business questions
- What are the total sales, profit, margin, and order count in the prepared dataset?
- How do sales and profit differ by category and sub-category?
- How close are categories to their sales targets?
- How are records distributed across profit, loss, and break-even groups?

## Workflow
1. Load order, order-detail, and sales-target source files.
2. Clean fields and set suitable data types in Power Query.
3. Create prepared fields such as location, profit margin, and profit status.
4. Combine order-level and order-line data using Order ID.
5. Prepare supporting summary tables.
6. Review sales, targets, and profitability through measures and report layouts.

## Data model
The repository documents eight analytical tables covering orders, order details, sales targets, prepared orders, monthly targets, category profit, order-detail summaries, and sub-category totals.

![Data Model Structure](images/data-model-architecture.svg)

See [Data Model Documentation](docs/Data_Model_Documentation.md) for details.

## Dashboard preview

![E-commerce sales dashboard layout preview](images/Business_Dashboard.svg)

*This is a static SVG layout preview created for project presentation. It is not a screenshot captured from Power BI Desktop, and its figures should be checked against the opened PBIX and source data before being used for decisions.*

## Selected results
The repository's documented analysis reports these results from the prepared dataset.

| Measure | Result |
|---|---:|
| Total sales | 283,497 |
| Total profit | -444 |
| Profit margin | -0.16% |
| Unique orders | 343 |
| Quantity | 3,734 |

| Category | Sales | Profit | Target achievement |
|---|---:|---:|---:|
| Electronics | 108,430 | 682 | 84.05% |
| Clothing | 96,641 | 2,387 | 55.54% |
| Furniture | 78,426 | -3,513 | 59.01% |

These are project-data results and depend on the model and measure definitions used in the repository.

## Files
| File | Purpose |
|---|---|
| [Power BI file](Data%20Transformation%20%26%20Data%20Modeling%20using%20Power%20BI.pbix) | Data model and Power BI report work |
| [Model documentation](docs/Data_Model_Documentation.md) | Table and model notes |
| [Data cleaning report](docs/DATA_CLEANING_REPORT.md) | Cleaning and transformation notes |
| [Business analysis](docs/Business_Analysis.md) | Measures, results, and analytical notes |
| [Model architecture](images/data-model-architecture.svg) | Data model diagram |
| [Dashboard layout preview](images/Business_Dashboard.svg) | Static design preview |

> **Presentation note:** The SVG dashboard image is a layout preview, not a screenshot exported from the interactive PBIX. Open the PBIX to review the report and replace the preview with a genuine screenshot when available.

## How to review
1. Open the PBIX in Power BI Desktop.
2. Review the Power Query transformations.
3. Inspect tables and relationships in Model view.
4. Review the report pages and compare measures with the documentation.
5. Use the docs folder for more detail.

## Scope and limitations
- Results reflect the supplied project data and the model definitions.
- Descriptive results do not establish causal explanations for profit outcomes.
- Confirm source data and measure definitions before using the figures for a business decision.
- The dashboard SVG is a preview layout and should not be presented as proof of the final interactive report's appearance.

## Author
**Shanmukh Koyya** · [GitHub](https://github.com/shanmukhkoyya) · [LinkedIn](https://www.linkedin.com/in/shanmukh-koyya/) · [Email](mailto:shanmukhkoyya1234@gmail.com)
