# 🏗️ SALES ANALYTICS — DATA ARCHITECTURE

<p align="center"><img src="https://img.shields.io/badge/SOURCES-03-315B75?style=for-the-badge"/> <img src="https://img.shields.io/badge/MODEL%20TABLES-08-1A8A77?style=for-the-badge"/> <img src="https://img.shields.io/badge/OUTPUT-PBIX-D9A900?style=for-the-badge"/></p>

## Architecture schematic
```mermaid
flowchart TB
 A[Orders] --> D[Power Query]
 B[Order Details] --> D
 C[Sales Targets] --> D
 D --> E[Cleaned tables]
 E --> F[Eight-table data model]
 F --> G[DAX measures]
 G --> H[Interactive report]
```

## System layers
| Layer | Responsibility | Review output |
|---|---|---|
| Sources | Orders, order details, sales targets | Three source datasets |
| Transform | Power Query cleanup and shaping | Prepared tables |
| Model | Relationships and DAX | Eight-table model |
| Report | Sales, profit, margin and target views | Interactive PBIX |

## Project overview
![Data transformation project overview](images/project-overview.svg)

## KPI design board
| KPI family | Business question |
|---|---|
| Sales | What is total sales and its trend? |
| Profit | Which categories contribute profit? |
| Margin | How does profit compare with sales? |
| Targets | How does actual sales compare with monthly targets? |
| Time | How do results change across periods? |

## Source package
- [Editable Power BI report](Data%20Transformation%20%26%20Data%20Modeling.pbix)
- [Raw data folder](Raw%20Data/)
- [Cleaned data folder](Cleaned%20Data/)
- [Documentation folder](Documentation/)

## Model acceptance tests
- [ ] Reconcile source and transformed row counts.
- [ ] Inspect relationships and filter direction.
- [ ] Validate DAX totals against source tables.
- [ ] Confirm target-period alignment.
- [ ] Test slicers and visual interactions.

> The SVG is an overview illustration, not a Power BI screenshot. Validate numerical outputs in the PBIX before presenting them externally.