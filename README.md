# 🏭 Azure Data Engineer – Motorcycle Manufacturing Company

> An end-to-end Azure Data Engineering solution built to ingest, transform, and serve data for a Motorcycle Manufacturing Company using Medallion Architecture.

---

## 📌 Project Overview

This project demonstrates a complete **ETL pipeline** built on Microsoft Azure. Raw manufacturing data is ingested into **Azure Data Lake Storage Gen2 (ADLS Gen2)**, transformed using **Azure Databricks (PySpark)**, and served via **SQL views and stored procedures** for reporting and analytics.

---

## 🏗️ Architecture

```
Raw Data Sources
      │
      ▼
Azure Data Factory (ADF) ──── Ingestion (Full Load & Incremental Load)
      │
      ▼
ADLS Gen2 – Bronze Layer (Raw Data)
      │
      ▼
Azure Databricks + PySpark ──── Transformations & Cleaning
      │
      ▼
ADLS Gen2 – Silver Layer (Cleaned Data)
      │
      ▼
SQL Server – Gold Layer (Views & Stored Procedures)
      │
      ▼
Reporting & Analytics
```

---

## ⚙️ Tech Stack

| Tool | Purpose |
|---|---|
| Azure Data Factory | Pipeline orchestration & data ingestion |
| Azure Data Lake Storage Gen2 | Raw & processed data storage |
| Azure Databricks (PySpark) | Data transformation & processing |
| Azure Synapse Analytics | Data warehousing |
| SQL Server | Gold layer views & stored procedures |
| Azure Logic Apps | Automated pipeline failure alerts |
| Git & GitHub | Version control |

---

## 📂 Project Structure

```
azure-data-engineer-motorcycle-project/
│
├── adf-pipelines/          # Azure Data Factory pipeline JSON exports
├── databricks-notebooks/   # PySpark transformation notebooks
├── sql-scripts/            # SQL views and stored procedures
├── architecture/           # Architecture diagrams
└── README.md
```

---

## 🔄 ETL Pipeline Details

### ✅ Data Ingestion (Bronze Layer)
- Designed and deployed **10+ ETL pipelines** using Azure Data Factory
- Ingested raw data into **ADLS Gen2 (Bronze Layer)**
- Implemented **Full Load** for initial data loads
- Implemented **Incremental Load** for ongoing delta data (500,000+ records per run)
- Eliminated all manual data handling processes

### ✅ Data Transformation (Silver Layer)
- Used **Azure Databricks with PySpark** for data transformation
- Standardized datasets across **5+ raw data tables**
- Applied data cleaning, type casting, and business rules

### ✅ Data Serving (Gold Layer)
- Created **8+ SQL views and stored procedures** in SQL Server
- Loaded transformed data into **Silver and Gold layers** (Medallion Architecture)
- Data ready for reporting and business analytics

### ✅ Monitoring & Automation
- Configured **Azure Logic Apps** for automated pipeline failure alerts
- All code and configurations managed via **Git and GitHub**

---

## 📈 Key Metrics

| Metric | Value |
|---|---|
| ETL Pipelines Built | 10+ |
| Records Processed Per Run | 500,000+ |
| Raw Data Tables Standardized | 5+ |
| SQL Views & Stored Procedures | 8+ |
| Manual Data Handling Eliminated | 100% |

---

## 🚀 How to Use This Project

1. Clone this repository:
```bash
git clone https://github.com/PranayK1723/azure-data-engineer-motorcycle-project.git
```

2. Review ADF pipeline JSONs in `/adf-pipelines`
3. Import Databricks notebooks from `/databricks-notebooks`
4. Run SQL scripts from `/sql-scripts` in your SQL Server

---

## 👤 Author

**Pranaykumar Katam**  
📧 pranayreddykatam@gmail.com  
📍 Hyderabad, India  
🔗 [LinkedIn](https://linkedin.com) | [GitHub](https://github.com/PranayK1723)

---

⭐ If you found this project helpful, please give it a star!
