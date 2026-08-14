# 📊 Supply Chain Analysis Dashboard | Power BI

## 📌 Project Overview

This project presents an interactive **Supply Chain Analysis Dashboard** developed using Microsoft Power BI.

The objective of the project is to analyze supply chain performance across **sales, profitability, delivery operations, products, shipping modes, and customer segments** and provide actionable business insights through interactive dashboards.

---

## 🎯 Business Objectives

The project focuses on answering the following business questions:

- How are overall sales and profitability performing?
- Which products and categories generate the highest sales?
- Which products generate the highest profit?
- What percentage of orders are delivered late?
- Which shipping modes have higher shipping times?
- How does actual shipping time compare with scheduled shipping time?
- Which customer segments contribute the most sales and profit?
- How does delivery performance change over time?
- Which factors are driving overall profitability?

---

## 🛠️ Tools & Technologies

- **Microsoft Power BI**
- **DAX**
- **Power Query**
- **Data Modeling**
- **Data Visualization**
- **CSV Dataset**

---

## 🗂️ Data Model

The original transactional dataset was transformed into a **star-schema data model** to improve organization, analysis, and report performance.

### Fact Table

**Fact_Order**

Contains transactional information such as:

- Order ID
- Order Date
- Sales
- Profit
- Quantity
- Shipping information
- Delivery information

### Dimension Tables

**Dim_Customer**
- Customer information
- Customer segment
- Customer location

**Dim_Product**
- Product information
- Product category

**Dim_Date**
- Date
- Year
- Month
- Quarter
- Day
- Month-Year

### Model Structure

```text
                 Dim_Date
                    │
                    │
Dim_Customer ─── Fact_Order ─── Dim_Product
