# 📊 Business Analysis — E-Commerce Sales

## 1. Analysis Scope

This analysis uses the prepared `Orders_Data.csv` dataset from the Power BI project.

The dataset contains **999 order-detail rows across 343 unique Order IDs**, covering the selected first 500 rows from the List of Orders source.

The analysis focuses on:

- Sales performance
- Profitability
- Category and sub-category performance
- Regional performance
- Sales target achievement
- Profit/Loss distribution

> **Important:** The figures below describe this project dataset and should not be interpreted as current real-world company performance.

---

## 2. KPI Summary

| KPI | Result |
|---|---:|
| Order-detail rows | 999 |
| Unique orders | 343 |
| Total sales amount | 283,497 |
| Total quantity | 3,734 |
| Total profit | -444 |
| Overall profit margin | -0.16% |
| Profit lines | 513 |
| Loss lines | 452 |
| Break-even lines | 34 |

The dataset has almost zero overall profit, with a slightly negative aggregate profit of **-444**.

---

## 3. Category Performance

| Category | Sales | Profit | Profit Margin | Target | Target Achievement |
|---|---:|---:|---:|---:|---:|
| Electronics | 108,430 | 682 | 0.63% | 129,000 | 84.05% |
| Clothing | 96,641 | 2,387 | 2.47% | 174,000 | 55.54% |
| Furniture | 78,426 | -3,513 | -4.48% | 132,900 | 59.01% |

### Key findings

- **Electronics** generated the highest sales amount and reached approximately **84.05%** of its target.
- **Clothing** generated the highest category profit at **2,387**, with a **2.47%** aggregate margin.
- **Furniture** generated **-3,513** profit and a **-4.48%** aggregate margin.
- Furniture is therefore the main contributor to the dataset's overall negative profit.
- Clothing has positive profitability but the lowest target achievement among the three categories.

---

## 4. Sub-Category Analysis

### Highest-sales sub-categories

| Sub-Category | Sales | Profit | Margin |
|---|---:|---:|---:|
| Saree | 42,375 | -1,438 | -3.39% |
| Printers | 35,197 | 1,053 | 2.99% |
| Phones | 35,121 | 1,019 | 2.90% |
| Bookcases | 32,240 | 1,749 | 5.42% |
| Electronic Games | 27,121 | -2,042 | -7.53% |

### Profitability observations

- **Bookcases** generated 1,749 profit with a 5.42% margin.
- **Trousers** generated 1,104 profit with a 4.81% margin.
- **Printers** and **Phones** also produced positive profit.
- **Tables** generated the largest sub-category loss at **-4,640** and a **-30.84%** aggregate margin.
- **Electronic Games** generated **-2,042** profit with a **-7.53%** aggregate margin.
- **Saree** had the highest sales among sub-categories but still generated a **-1,438** loss, showing that sales volume alone does not guarantee profitability.

---

## 5. Regional Analysis

| State | Sales | Profit | Margin |
|---|---:|---:|---:|
| Maharashtra | 68,740 | 1,704 | 2.48% |
| Madhya Pradesh | 67,153 | 42 | 0.06% |
| Uttar Pradesh | 15,577 | 908 | 5.83% |
| Rajasthan | 14,161 | -351 | -2.48% |
| Gujarat | 13,561 | -350 | -2.58% |

Additional observation:

- Kerala generated 11,302 sales and 1,428 profit, giving a 12.63% aggregate margin in this dataset.

Regional performance should be interpreted together with sales volume because a high margin on a smaller sales base can produce less absolute profit than a lower margin on a larger base.

---

## 6. Sales Target Analysis

Target achievement is calculated as:

**Actual Sales ÷ Sales Target × 100**

| Category | Achievement |
|---|---:|
| Electronics | 84.05% |
| Furniture | 59.01% |
| Clothing | 55.54% |

The project data shows that none of the three categories reached 100% of the supplied target totals.

Electronics had the smallest gap to its target, while Clothing had the largest target gap in absolute terms.

---

## 7. Profit Status Analysis

The 999 order-detail rows contain:

- **513 Profit rows**
- **452 Loss rows**
- **34 Break-Even rows**

This shows why row-level profitability should be investigated rather than relying only on total sales.

A useful dashboard visual is a **Profit Status distribution** alongside total sales and total profit.

---

## 8. Business Questions Answered

### Q1. Which category generated the highest sales?
**Electronics**, with 108,430 in sales.

### Q2. Which category generated the highest profit?
**Clothing**, with 2,387 profit.

### Q3. Which category is contributing most to the overall loss?
**Furniture**, with -3,513 profit.

### Q4. Which sub-category requires profitability investigation?
**Tables**, with -4,640 profit and a -30.84% aggregate margin.

### Q5. Which high-sales sub-category needs attention?
**Saree** generated 42,375 in sales but -1,438 profit.

### Q6. Which category is closest to its target?
**Electronics**, at 84.05% target achievement.

### Q7. Which region has the highest sales?
**Maharashtra**, with 68,740 in sales.

---

## 9. Recommended Analytical Actions

Based on the project dataset:

1. Investigate the pricing/cost structure of **Tables**, which has the largest sub-category loss.
2. Investigate why **Saree** has high sales but negative aggregate profit.
3. Review **Electronic Games**, which combines meaningful sales with negative profitability.
4. Analyze why **Electronics** has strong target achievement but only a small positive aggregate margin.
5. Compare high-volume and high-margin products separately rather than evaluating products using sales alone.
6. Use category, sub-category, state, month, and Profit Status slicers in the Power BI report for drill-down analysis.

These are analytical follow-up actions derived from the project dataset; they are not claims about a real company's operating decisions.

---

## 10. Suggested Power BI Visuals

### Executive KPI page
- Total Sales
- Total Profit
- Profit Margin
- Unique Orders
- Target Achievement %

### Performance page
- Monthly Sales vs Target line/column chart
- Sales by Category
- Profit by Category
- Target Achievement by Category

### Product page
- Sales by Sub-Category
- Profit by Sub-Category
- Profit Margin by Sub-Category
- Profit Status distribution

### Regional page
- Sales by State
- Profit by State
- Sales/Profit by City
- State slicer

### Interactive controls
- Date/Month
- Category
- Sub-Category
- State
- Profit Status

---

## 11. Portfolio Value

This analysis demonstrates the progression from:

**Raw Data → Cleaned Data → Data Model → KPI Analysis → Business Questions → Analytical Insights → Power BI Reporting**

It strengthens the project by showing not only how the data was prepared, but also how an analyst can turn the prepared model into business-focused questions and measurable findings.
