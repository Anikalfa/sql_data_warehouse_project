# Data Warehouse and Analytics Project
Building a modern data warehouse with SQL server, including ETL process, data modeling, and analytics.

Welcome to the **Data Warehouse and Analytics Project** repository! 🚀
This project demonstrates a comprehensive data warehousing and analytics solution, from building a data warehouse to generating actionable insights. Designed as a portfolio project, it highlights industry best practices in data engineering and analytics.

## Data Architecture

![Data Architecture](docs/PROJECT%20arc.drawio.png)

The data architecture for this project follows Medallion Architecture: **Bronze**, **Silver**, and **Gold** layers:

1. **Bronze Layer**: Stores raw data as-is from the source systems. Data is ingested from CSV Files into SQL Server Database.
2. **Silver Layer**: This layer includes data cleansing, standardization, and normalization processes to prepare data for analysis.
3. **Gold Layer**: Houses business-ready data modeled into a star schema required for reporting and analytics.
---

## 🛠️ Data Engineering (Building the Data Warehouse)

### 🎯 Objective
To develop a centralized data warehouse that consolidates disparate sales data, enabling reliable analytical reporting and business intelligence.

### 📋 Specifications & Scope
* **Data Sources:** Ingestion and integration of data from two distinct source systems provided as CSV files:
    * **ERP (Enterprise Resource Planning):** Core transactional and operational sales data.
    * **CRM (Customer Relationship Management):** Customer profiles and interaction data.
* **Data Quality & Cleansing:** Implementation of preprocessing pipelines to identify, cleanse, and resolve data quality issues (e.g., missing values, duplicates, formatting inconsistencies) prior to loading into the final model.
* **Integration & Modeling:** Merging both sources into a unified, optimized data model tailored specifically for analytical queries.
* **Scope Limitation:** Focused strictly on the **latest dataset only**. Historization (SCDs/tracking historical changes) is explicitly out of scope for this phase.
* **Documentation:** Comprehensive documentation of the final data model schemas to support both business stakeholders and downstream analytics teams.

---

## 📊 Data Analysis (BI, Analytics & Reporting)

### 🎯 Objective
To develop robust, high-performance SQL-based analytics that extract actionable business intelligence from the consolidated data warehouse.

The reporting layer delivers detailed insights into three critical business pillars:

1.  **Customer Behavior:** Analyzing purchasing patterns, customer segmentation, and engagement metrics.
2.  **Product Performance:** Identifying top-performing products, revenue contributors, and inventory/sales velocity.
3.  **Sales Trends:** Evaluating sales performance over time to detect seasonality, growth trajectories, and market shifts.
