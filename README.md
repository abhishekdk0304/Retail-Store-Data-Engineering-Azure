# Retail Store Data Engineering Pipeline on Azure

## Project Overview

This project demonstrates an end-to-end Azure Data Engineering pipeline that ingests retail sales data from multiple sources, processes it using Azure Databricks with PySpark and Spark SQL, stores curated datasets in Azure Data Lake Storage Gen2 (ADLS Gen2) following the Medallion Architecture (Bronze, Silver, Gold), and visualizes business insights using Power BI.

The solution simulates a real-world retail analytics platform by integrating structured data from Azure SQL Database and semi-structured customer data from a REST API.

---

# Technologies Used

- Azure Data Factory (ADF)
- Azure Data Lake Storage Gen2 (ADLS Gen2)
- Azure SQL Database
- Azure Databricks
- PySpark
- Spark SQL
- REST API (JSON)
- Parquet
- Power BI

---

# Project Features

- End-to-End Azure Data Engineering Pipeline
- Multi-source Data Ingestion
- Azure SQL Database Integration
- REST API Integration
- Azure Data Factory Orchestration
- Azure Data Lake Storage Gen2
- Medallion Architecture (Bronze, Silver, Gold)
- PySpark Data Processing
- Spark SQL Transformations
- Data Cleansing and Validation
- Business Aggregations
- Interactive Power BI Dashboard

---

# Data Sources

| Source | Format | Description |
|----------|----------|-------------------------------|
| Azure SQL Database | Tables | Transactions, Products, Stores |
| REST API | JSON | Customer Information |

---

# Pipeline Workflow

1. Ingested transaction, product, and store data from Azure SQL Database and customer data from a REST API using Azure Data Factory.
2. Loaded raw data into the Bronze layer of Azure Data Lake Storage Gen2 in Parquet format.
3. Processed Bronze data using Azure Databricks with PySpark and Spark SQL to perform data cleansing, transformations, and joins, creating Silver datasets.
4. Generated aggregated business metrics from Silver data and stored curated Gold datasets in Azure Data Lake Storage Gen2.
5. Built an interactive Power BI dashboard using the Gold-layer dataset.

---

# Project Architecture

![Architecture](Images/architecture.png)

---

# Medallion Architecture

## Bronze Layer

- Raw data ingested from Azure SQL Database and REST API
- Stored in Azure Data Lake Storage Gen2
- Stored in Parquet format

## Silver Layer

- Data cleansing
- Data type conversion
- Joining multiple datasets
- Business rule validation
- Stored in Azure Data Lake Storage Gen2
- Stored in Parquet format

## Gold Layer

- Business aggregations
- Sales summaries
- KPI datasets optimized for reporting
- Stored in Azure Data Lake Storage Gen2
- Stored in Parquet format

---

# Project Screenshots

## Azure Data Factory Pipeline

![ADF Pipeline](Images/adf-pipeline.png)

---

## Azure Data Lake Storage Gen2 (Bronze, Silver, Gold)

![ADLS](Images/adls-bronze-silver-gold.png)

---

## Azure Databricks Pipeline

![Databricks](Images/databricks-pipeline.png)

---

## Power BI Dashboard

![Power BI](Images/powerbi-dashboard.png)

---

# Repository Structure

```text
Retail-Store-Data-Engineering-Azure
│
├── Architecture
├── Azure-Data-Factory
├── Databricks
├── Images
├── PowerBI
└── README.md
```

---

# Skills Demonstrated

- Azure Data Factory
- Azure Data Lake Storage Gen2 (ADLS Gen2)
- Azure Databricks
- PySpark
- Spark SQL
- SQL
- ETL Pipeline Development
- Data Ingestion
- Data Transformation
- Data Cleansing
- Data Integration
- Medallion Architecture
- Data Warehousing Concepts
- REST API Integration
- Parquet
- Power BI
- Data Visualization

---

# Key Learning Outcomes

- Built an end-to-end Azure Data Engineering pipeline.
- Integrated data from Azure SQL Database and REST API.
- Orchestrated data ingestion using Azure Data Factory.
- Processed and transformed large datasets using Azure Databricks, PySpark, and Spark SQL.
- Implemented the Medallion Architecture (Bronze, Silver, Gold).
- Generated curated analytical datasets for reporting.
- Developed an interactive Power BI dashboard for retail sales analytics.

---

# Future Enhancements

- Implement incremental data loading.
- Store curated datasets using Delta Lake.
- Schedule pipeline execution using Azure Data Factory triggers.
- Integrate Git version control with Azure Data Factory.
- Implement automated data quality validation.
- Add monitoring and alerting for pipeline execution.
- Deploy infrastructure using ARM Templates, Bicep, or Terraform.

---

# Project Type

**Personal Learning Project**

This project was developed for hands-on experience with Azure Data Engineering services and demonstrates an end-to-end cloud data engineering workflow using Azure Data Factory, Azure Data Lake Storage Gen2, Azure Databricks, PySpark, Spark SQL, REST API integration, and Power BI.
