# 🏗️ SALES ANALYTICS — MODEL BLUEPRINT

<p align="center"><img src="https://img.shields.io/badge/SOURCE-3%20FILES-315B75?style=for-the-badge"/> <img src="https://img.shields.io/badge/MODEL-8%20TABLES-1A8A77?style=for-the-badge"/> <img src="https://img.shields.io/badge/OUTPUT-POWER%20BI-D9A900?style=for-the-badge"/></p>

## Architecture map
| Layer | Inputs / process | Output |
|---|---|---|
| 01 · Sources | Orders, order details, sales targets | Three source datasets |
| 02 · Transform | Power Query cleanup and shaping | Prepared tables |
| 03 · Model | Relationships and DAX | Eight-table model |
| 04 · Report | Sales, profit, margin and target views | Interactive PBIX |

## Visual overview
![Data transformation project overview](images/project-overview.svg)

## KPI design board
| KPI family | Question |
|---|---|
| Sales | What is total sales and its trend? |
| Profit | Which categories contribute profit? |
| Margin | How does profit compare with sales? |
| Targets | How does actual sales compare with monthly targets? |
| Time | How do results change across periods? |

## Project files
- [Editable Power BI report](Data%20Transformation%20%26%20Data%20Modeling.pbix)
- [Raw data folder](Raw%20Data/)
- [Cleaned data folder](Cleaned%20Data/)
- [Documentation folder](Documentation/)

## Model acceptance checklist
- [ ] Reconcile source and transformed row counts.
- [ ] Inspect relationships and filter direction.
- [ ] Validate DAX totals against source tables.
- [ ] Confirm target-period alignment.
- [ ] Test slicers and visual interactions.

> The SVG is an overview illustration, not a Power BI screenshot. Validate numerical outputs in the PBIX before presenting them externally.