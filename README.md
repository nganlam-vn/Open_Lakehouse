# 🚀 OpenLakehouse Platform  
### A Fully Local, Open-Source Lakehouse for Ingestion, Storage, Processing, and Orchestration

This project implements a complete **Open Lakehouse architecture** using 100% open-source technologies. It is designed for end-to-end data ingestion, processing, storage, orchestration, and analytics - all running locally via Docker.

The architecture follows the **Medallion Model (Bronze → Silver → Gold)** and provides a unified environment for ETL/ELT, metadata management, SQL analytics, and data quality pipelines.

---
## 🧱 Lakehouse Architecture Summary

### 🗄️ **Data Lake Storage**
- **MinIO** - S3-compatible object storage for all Bronze, Silver, and Gold layers.

### 📁 **Supported File Formats**
- **Parquet**, **ORC**, **CSV**, **JSON**, and other semi-structured formats.

### 🧩 **Open Table Format**
- **Delta Lake** - ACID transactions, schema evolution, time travel, and optimized Parquet storage.

### 🗃️ **Metastore**
- **Hive Metastore** - central metadata catalog for Delta Lake and Trino.

### 💻**Processing Engine**
- **Apache Spark + Delta Lake** - Performs ETL/ELT jobs and medallion transformations.

### ⚙️ **Orchestration Layer**
- **Apache Airflow 3.1**  - For automate the process: Schedules ingestion, processing, and enrichment jobs.

### 📊 **Compute Engine**
- **Trino** - distributed SQL query engine for analytics across the entire Lakehouse.

### 🐳 **Containerization & Deployment**
- **Docker & Docker Compose** - orchestrates MinIO, Hive Metastore, Trino, Spark, and Airflow into a fully local Lakehouse environment.
