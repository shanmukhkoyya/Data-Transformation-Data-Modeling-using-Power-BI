# 🔄 Data Transformation & Data Modeling using Power BI

A hands-on **Power BI Data Analytics project** focused on **data transformation, data preparation, data modeling, and business-ready reporting structure**.

This project demonstrates an important part of a real-world analytics workflow: taking multiple business tables, preparing them for analysis, and organizing them into a model that can support meaningful reporting.

---

## 📌 Project Overview

In a professional analytics environment, a dashboard is only as reliable as the data model behind it.

This project focuses on the foundation of Power BI reporting:

**Source Data → Power Query → Data Cleaning & Transformation → Data Model → Relationships → Business Analysis**

The PBIX contains a multi-table model built around **orders, order details, sales targets, categories, sub-categories, monthly targets, and aggregated analysis tables**.

---

## 🎯 Business Objective

The project is designed to prepare a sales dataset for business reporting and help answer questions such as:

- How are sales performing over time?
- How can sales be compared with monthly targets?
- Which categories contribute to sales and profit?
- Which sub-categories require closer analysis?
- How can order-level and order-detail data be structured for reporting?
- How should supporting summary tables be organized for efficient analysis?

---

## 🧹 Data Transformation

The project demonstrates the data-preparation stage required before visualization.

### Key areas

- Data loading into Power BI
- Data preparation using Power Query
- Data transformation
- Data organization
- Aggregation and summary-table preparation
- Preparing data for analytical relationships
- Structuring business data for reporting

---

## 🧩 Data Model

The PBIX contains **8 verified tables**:

| Table | Analytical Purpose |
|---|---|
| `List of Orders` | Order-level business data |
| `Order Details (1)` | Detailed order-line information |
| `Sales target (1)` | Sales target reference data |
| `Orders Data` | Prepared order dataset |
| `Monthly Sales Target` | Monthly target analysis |
| `Category Average Profit` | Category-level profit reference |
| `Order Details Summary` | Aggregated order-detail structure |
| `Sub-Category Total Amount` | Sub-category aggregation |

### Model Architecture

![Data Model Structure](images/data-model-architecture.svg)

The PBIX includes a model diagram, confirming that the project contains a dedicated **data-modeling layer**.

---

## 📊 Business Analysis Structure

A validated business analysis is documented in [Business Analysis](docs/Business_Analysis.md), using the prepared project dataset to calculate KPIs, category performance, target achievement, sub-category profitability, regional performance, and profit-status distribution.

The prepared model is designed to support a reporting layer covering:

### KPI Analysis
- Total Sales
- Total Profit
- Total Orders
- Profit Margin
- Sales Target Achievement

### Trend Analysis
- Monthly Sales Trend
- Monthly Target Comparison

### Category Analysis
- Sales by Category
- Profit by Category
- Category-level performance

### Sub-Category Analysis
- Sales by Sub-Category
- Profit contribution
- Sub-category performance comparison

### Interactive Analysis
- Date/Month filtering
- Category filtering
- Sub-category filtering
- Business-level drill-down analysis

> **Note:** These are the analytical areas the verified model is structured to support. The current PBIX report page does not contain completed report visuals, so this repository does not claim dashboard results that are not actually present.

---

## 🛠️ Tools & Technologies

- **Power BI**
- **Power Query**
- **Data Transformation**
- **Data Cleaning & Preparation**
- **Data Modeling**
- **Table Relationships**
- **Aggregation**
- **Business Intelligence Reporting**

---

## 💡 What I Learned

Through this project, I practiced:

- Preparing business data for analysis
- Transforming data with Power Query
- Working with multiple related tables
- Designing a structured analytical model
- Creating supporting summary tables
- Preparing sales and target data for comparison
- Thinking from a business-question perspective before building visuals
- Understanding how data modeling supports Power BI reporting

---

## 📁 Repository Structure

```text
Data-Transformation-Data-Modeling-using-Power-BI/
│
├── Data Transformation & Data Modeling using power BI.pbix
│
├── images/
│   └── data-model-architecture.svg
│
├── docs/
│   ├── Data_Model_Documentation.md
│   ├── DATA_CLEANING_REPORT.md
│   └── Business_Analysis.md
│
└── README.md
```

---

## 🚀 How to Explore the Project

### Step 1 — Download
Download the PBIX file from this repository.

### Step 2 — Open
Open the file using **Microsoft Power BI Desktop**.

### Step 3 — Review Data Preparation
Open **Transform Data** to review the Power Query/data-preparation layer.

### Step 4 — Review the Model
Open **Model view** and inspect the available tables and relationships.

### Step 5 — Review the Reporting Layer
Open **Report view** to inspect the current report structure and extend the model into business-focused visuals.

---

## 📚 Documentation

- [Data Model Documentation](docs/Data_Model_Documentation.md)
- [Data Model Architecture](images/data-model-architecture.svg)
- [Business Analysis & Validated Insights](docs/Business_Analysis.md)

---

## ⚠️ Scope & Limitations

This repository documents the **verified contents of the current PBIX**.

The model and analytical direction are documented based on the project file. Numerical KPI results, relationship cardinalities, and dashboard findings are intentionally not presented unless they are verified from the source PBIX.

The current report page is not yet a completed dashboard. The next development stage is to build the visual reporting layer from the prepared model.

---

## 🔮 Future Enhancements

Planned improvements include:

- Build a professional executive dashboard
- Add KPI cards and business-focused visuals
- Add monthly sales vs target analysis
- Add category and sub-category performance visuals
- Add interactive slicers and navigation
- Improve dashboard usability and visual storytelling
- Add validated business insights and recommendations
- Extend the project with Python-based exploratory analysis

---

## ⭐ Portfolio Value

This project is part of my hands-on **Data Analytics portfolio** and demonstrates the foundation behind professional Power BI reporting.

It complements projects focused on:

- End-to-end dashboard development
- SQL business analysis
- Power BI & DAX analysis
- Data transformation and data modeling

Together, these projects demonstrate my learning across different stages of the **Data Analyst workflow**.

---

## 👤 About Me

**Shanmukh Koyya**

Aspiring Data Analyst | Power BI | SQL | Excel | Python

📧 **Email:** [shanmukhkoyya1234@gmail.com](mailto:shanmukhkoyya1234@gmail.com)

💼 **LinkedIn:** [linkedin.com/in/shanmukh-koyya](https://www.linkedin.com/in/shanmukh-koyya/)

💻 **GitHub:** [github.com/shanmukhkoyya](https://github.com/shanmukhkoyya)

---

⭐ If you find this project useful, feel free to explore the repository and my other Data Analytics projects.
