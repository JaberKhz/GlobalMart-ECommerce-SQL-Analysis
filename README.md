# 📊 GlobalMart Solutions: E-Commerce SQL Data Analysis Project

## 🏢 Business Scenario
In this project, I acted as the lead **Data Analyst** at **GlobalMart Solutions**, a major global e-commerce platform. The executive management required deep data insights to optimize logistics, clean customer databases, detect fraud, analyze sales trends, and segment products. 

I designed a scalable PostgreSQL database containing **500 customers**, **100 products**, and **2,000 orders** with interconnected transaction details to simulate real-world big data challenges.

---

## 🛠️ Tech Stack & Skills Demonstrated
- **Database Engine:** PostgreSQL / PgAdmin 4
- **Core SQL Skills Applied:**
  - **Data Cleaning:** `TRIM()`, `LOWER()`, `UPPER()`, `CONCAT()`, `SUBSTRING()`
  - **Conditional Logic:** `CASE WHEN`, `BETWEEN`, `IS NOT NULL`
  - **Aggregations & Grouping:** `SUM()`, `AVG()`, `COUNT(DISTINCT)`, `MAX()`, `MIN()`, `GROUP BY`, `HAVING`
  - **Advanced Joins:** `INNER JOIN` (multi-table), `LEFT JOIN`, `FULL OUTER JOIN`, `CROSS JOIN`
  - **Advanced Techniques:** `SubQueries`, `UNION`, `EXTRACT(HOUR FROM)`, `NOW()`
  - **Data Pipelines:** `CREATE VIEW` (Filtered Pipelines), `SQL Pivot Tables`

---

## 📈 Project Phases & Key Insights

### 1. Customer & Fraud Analysis
- Filtered active customers in specific Arab regions (Egypt, UAE, KSA) with complete delivery data.
- Handled text irregularities by trimming trailing spaces and filtering out potential spam/bot accounts using `TRIM()` and `LIKE 'user_10%'`.

### 2. Inventory & Sales Summary
- Evaluated total inventory count, global price average, and peak ordering hours by extracting time metrics (`EXTRACT(HOUR FROM order_date)`).
- Filtered high-performing order statuses that exceeded a 300-order threshold using `HAVING`.

### 3. Business Intelligence & Strategic Reporting
- **Customer Purchase Journey:** Built a 4-table join query to tie customer information directly to final product shipping statuses.
- **Product Segmentation:** Classified items into `Premium`, `Mid-Range`, and `Budget` segments dynamically.
- **SQL Pivot Table:** Created a matrix displaying the total quantities sold per country across product categories using conditional aggregations.
- **Data Pipeline:** Standardized logistics access by creating a persistent database `VIEW` filtering for completed `Shipped` orders only.

---

## 📂 Repository Contents
- `globalmart_analysis.sql`: Full script including DDL (schema creation) and all 15 business analysis queries.

---
*Developed as part of my Data Analytics Portfolio.*
