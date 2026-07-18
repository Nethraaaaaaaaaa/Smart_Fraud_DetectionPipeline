# 🛡️ Smart Fraud Detection Pipeline using PySpark & Databricks

![PySpark](https://img.shields.io/badge/PySpark-Data%20Engineering-orange)
![Databricks](https://img.shields.io/badge/Databricks-Platform-red)
![Spark SQL](https://img.shields.io/badge/Spark_SQL-Analytics-blue)
![Delta Lake](https://img.shields.io/badge/Delta_Lake-Storage-green)
![Python](https://img.shields.io/badge/Python-3.x-yellow)

## 📌 Project Overview

The **Smart Fraud Detection Pipeline** is an end-to-end data engineering project developed using **PySpark, Spark SQL, and Databricks**. The project processes banking transaction data through the **Medallion Architecture (Bronze → Silver → Gold)** to identify suspicious transactions and generate business-ready analytical insights.

The pipeline demonstrates how raw banking data can be transformed into reliable and structured datasets for fraud analysis using scalable data engineering techniques.

---

# 🎯 Problem Statement

Financial institutions process thousands of transactions every day, making fraud detection challenging. Raw transactional data often contains inconsistencies, missing values, and duplicate records.

This project builds a scalable fraud detection pipeline that:

- Ingests raw banking datasets
- Cleans and validates data
- Applies fraud detection rules
- Produces business-ready analytical tables
- Generates SQL-based insights for decision-making

---

# ✨ Features

- Raw CSV data ingestion
- Medallion Architecture implementation
- Data cleaning and preprocessing
- Null value handling
- Duplicate removal
- Data type casting
- Dataset integration using joins
- Rule-based fraud detection
- Delta Lake storage
- Spark SQL analytics
- Business summary tables

---

# 🏗️ Architecture

```
CSV Files
      │
      ▼
Databricks Volume
      │
      ▼
Bronze Layer
(Raw Data)
      │
      ▼
Silver Layer
(Cleaned & Enriched Data)
      │
      ▼
Gold Layer
(Fraud Analytics)
      │
      ▼
Spark SQL Analytics
      │
      ▼
Business Insights
```

> *(You can replace this section later with your architecture diagram.)*

---

# 🛠️ Tech Stack

| Technology | Purpose |
|------------|---------|
| Python | Programming Language |
| PySpark | Data Processing |
| Spark SQL | Data Analysis |
| Databricks | Development Platform |
| Delta Lake | Data Storage |
| GitHub | Version Control & Portfolio |

---

# 📂 Dataset

The project uses three CSV datasets:

| Dataset | Description |
|----------|-------------|
| accounts.csv | Customer account information |
| transactions.csv | Banking transaction records |
| known_fraud_accounts.csv | Fraud watchlist |

---

# ⚙️ Pipeline Workflow

## 🥉 Bronze Layer

### Purpose
Store raw data without modifications.

### Tables
- bronze_accounts
- bronze_transactions
- bronze_frauds

### Operations
- CSV ingestion
- Schema inference
- Delta table creation

---

## 🥈 Silver Layer

### Purpose
Clean and transform raw data.

### Operations

- Duplicate removal
- Null value handling
- Data type conversion
- Data validation
- Dataset integration using joins

### Tables

- silver_accounts
- silver_transactions
- silver_frauds
- silver_combined_dataset

---

## 🥇 Gold Layer

### Purpose

Generate business-ready datasets for fraud analysis.

### Fraud Detection Rules

- High-value transactions
- International transactions
- Known fraud accounts
- Suspicious transaction flag

### Tables

- gold_fraud_transactions
- gold_customer_summary
- gold_branch_summary
- gold_daily_transactions

---

# 📊 SQL Analytics

The project includes Spark SQL queries to generate business insights such as:

- Total Transactions
- Suspicious Transactions
- High Value Transactions
- International Transactions
- Known Fraud Accounts
- Top Customers
- Branch-wise Transaction Analysis
- Branch-wise Suspicious Transactions
- Daily Transaction Summary
- Fraud Type Distribution

---

# 📁 Project Structure

```
Smart-Fraud-Detection-Pipeline/
│
├── datasets/
│   ├── accounts.csv
│   ├── transactions.csv
│   └── known_fraud_accounts.csv
│
├── notebooks/
│   ├── 01_Bronze_Ingestion
│   ├── 02_Silver_Transformation
│   ├── 03_Gold_Analytics
│   └── 04_SQL_Analytics
│
├── screenshots/
│
├── architecture/
│
└── README.md
```

---

# 🚀 How to Run

1. Upload the datasets to Databricks Volume.
2. Execute the Bronze notebook.
3. Execute the Silver notebook.
4. Execute the Gold notebook.
5. Run the SQL Analytics notebook.
6. Analyze the generated Delta tables and SQL outputs.

---

# 📈 Results

- Successfully implemented a Medallion Architecture pipeline.
- Improved data quality through cleaning and validation.
- Detected suspicious transactions using rule-based logic.
- Generated business-ready analytical tables.
- Produced meaningful fraud insights using Spark SQL.

---

# 🔮 Future Enhancements

- Real-time fraud detection using Spark Structured Streaming
- Machine Learning-based fraud prediction
- Power BI Dashboard Integration
- Apache Airflow Workflow Automation

---
