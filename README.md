# sql-data-cleaning-eda-project
Data Cleaning and Exploratory Data Analysis (EDA) in SQL using MySQL
# 📊 SQL Project: Data Cleaning & Exploratory Data Analysis (EDA)

## 📌 Project Overview
This project demonstrates a full data analysis workflow using **MySQL**. It covers cleaning raw, unstructured data and performing Exploratory Data Analysis (EDA) to discover meaningful business trends.

---

## 🛠 Tech Stack & Tools
- **Database:** MySQL
- **Tool:** MySQL Workbench
- **SQL Concepts Used:** CTEs, Window Functions (`ROW_NUMBER`, `DENSE_RANK`), Aggregate Functions, Subqueries, Joins.

---

## 🧹 Part 1: Data Cleaning
The goal was to transform raw data into a reliable format ready for analysis.

**Key Steps Performed:**
1. **Removing Duplicates:** Used CTEs and `ROW_NUMBER()` to identify and delete duplicate rows.
2. **Standardizing Data:** Fixed formatting issues in string columns, standardized date fields (`STR_TO_DATE`), and trimmed whitespace.
3. **Handling Null Values:** Imputed missing values where possible based on related entries and populated blank fields.
4. **Removing Irrelevant Data:** Dropped unnecessary columns and unhelpful blank entries.

📁 *See script: data_cleaning.sql

---

## 📈 Part 2: Exploratory Data Analysis (EDA)
After cleaning, I analyzed the data to extract business insights and key metrics.

**Key Insights & Analysis:**
- Summarized key performance metrics using `SUM`, `AVG`, and `GROUP BY`.
- Ranked top entities per category/year using `DENSE_RANK()`.
- Analyzed rolling totals and period-over-period growth using Window Functions.

📁 *See script: exploratory_data_analysis.sql
---

## 🚀 How to Run
1. Import the raw dataset into MySQL.
2. Run `01_data_cleaning.sql` to prepare the clean table.
3. Execute `02_eda_analysis.sql` to view the analysis queries.
