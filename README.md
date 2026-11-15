# Customer & Sales Analysis

## Project Overview

This project focuses on analyzing customer and sales data to identify business patterns, evaluate customer behavior, and support data-driven decision-making.

The project also emphasizes data quality assurance (QA) and data cleaning to ensure that the dataset is consistent, reliable, and suitable for further analysis.

## Project Objectives

- Analyze sales performance across different dimensions.
- Understand customer characteristics and purchasing behavior.
- Identify data quality issues and potential anomalies.
- Establish business rules for data validation.
- Transform raw data into meaningful insights through data analysis and visualization.

## Dataset Description

The project uses four interconnected datasets:

| Dataset | Description |
|---|---|
| Sales_Data | Transaction-level sales information |
| Customer | Customer profiles and registration information |
| Products | Product-related information |
| Branches | Branch-related information |

**Dataset Overview:**
- Total transactions: 950
- Total customers: 180
- Transaction period: 2025–2026

## Tools & Technologies

- **Microsoft Excel** – Initial data inspection and data quality checks.
- **SQLite / DB Browser for SQLite** – SQL-based data validation and querying.
- **SQL** – Data cleaning, anomaly detection, and analytical queries.
- **Microsoft Power BI** – Data visualization and interactive dashboards.

## Data Cleaning & Quality Assurance

Data quality is an important part of this project. Before conducting further analysis, the datasets are examined to identify inconsistencies and potential anomalies.

The initial validation process includes:

- Data format and consistency checks.
- Duplicate transaction identification.
- NULL value inspection.
- Date consistency validation.
- Business rule development and validation.

### Business Rule: Order Date vs. Signup Date

One of the identified potential anomalies concerns the relationship between transaction dates and customer registration dates.

**Validation Rule:**

`Order_Date < Signup_Date`

A transaction is flagged as a potential anomaly when its order date occurs before the customer's registration date.

This rule is used to identify records requiring further investigation. Flagged records are not automatically deleted or modified without additional validation.

## Analytical Workflow

1. Data Collection – Gather the original datasets.
2. Data Inspection – Examine data structure, formats, and consistency.
3. Data Cleaning & QA – Identify duplicates, missing values, and potential anomalies.
4. SQL Analysis – Perform validation and analytical queries.
5. Data Visualization – Develop interactive dashboards using Power BI.
6. Insight Development – Interpret analytical findings to support business decisions.

## Project Structure

```text
Customer-and-Sales-Analysis/
│
├── customer_sales_analysis_dataset.xlsx
├── README.md
│
├── SQL/
│
├── PowerBI/
│
└── Documentation/
```

## Project Status

This repository serves as the working documentation and portfolio for the Customer & Sales Analysis project.

Further analytical findings, dashboard visualizations, and documentation will be added as the project progresses.

## Author

**Aldis Yahid**

Data Analytics Portfolio Project

---

*This project is developed for analytical learning, data quality assessment, and business intelligence purposes.*
