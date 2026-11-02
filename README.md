<p align="center"><img src="assets/readme-hero.svg" width="100%" alt="Sales data architecture"/></p>

# SALES ANALYTICS / MODEL BLUEPRINT

<p align="center">
<img src="https://img.shields.io/badge/SOURCE%20TABLES-03-315B75?style=for-the-badge"/>
<img src="https://img.shields.io/badge/MODEL%20TABLES-08-1A8A77?style=for-the-badge"/>
<img src="https://img.shields.io/badge/DELIVERY-PBIX-D9A900?style=for-the-badge"/>
</p>

## 01 — Data architecture

```mermaid
flowchart LR
 O[Orders] --> PQ[Power Query]
 D[Order Details] --> PQ
 T[Sales Targets] --> PQ
 PQ --> ST[Cleaned tables]
 ST --> M[Eight-table model]
 M --> DX[DAX measures]
 DX --> R[Interactive report]
```

## 02 — Model layers

| Layer | Design responsibility | Review question |
|---|---|---|
| Source | Orders, order details, sales targets | Are source fields understood? |
| Transform | Power Query cleanup and shaping | Are types and keys consistent? |
| Model | Eight-table data model | Do relationships filter correctly? |
| Measure | DAX calculations | Do totals reconcile? |
| Report | Sales, profit, margin and target views | Can users answer business questions? |

## 03 — Visual architecture map

![Project overview](images/project-overview.svg)

## 04 — KPI catalogue

<table>
<tr><th>MEASURE FAMILY</th><th>BUSINESS QUESTION</th></tr>
<tr><td>💰 Sales</td><td>What is the sales total and how does it trend?</td></tr>
<tr><td>📈 Profit</td><td>Which categories contribute profit?</td></tr>
<tr><td>％ Margin</td><td>How does profit compare with sales?</td></tr>
<tr><td>🎯 Targets</td><td>How does actual sales compare with monthly targets?</td></tr>
<tr><td>🗓️ Time</td><td>How do results change across periods?</td></tr>
</table>

## 05 — Open the engineering package

- [Power BI report](Data%20Transformation%20%26%20Data%20Modeling.pbix)
- [Raw data](Raw%20Data/)
- [Cleaned data](Cleaned%20Data/)
- [Project documentation](Documentation/)

## 06 — Validation gates

- [ ] Reconcile source and transformed row counts.
- [ ] Inspect relationship cardinality and filter direction.
- [ ] Validate DAX totals against source tables.
- [ ] Confirm target-period alignment.
- [ ] Test slicers, cross-filtering and visual interactions.

> The SVG is an overview illustration, not a Power BI screenshot. Validate numerical outputs in the PBIX before presenting them externally.