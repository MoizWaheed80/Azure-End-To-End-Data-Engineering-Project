# End-to-End Azure Data Engineering Pipeline

An end-to-end Azure data engineering project that ingests data from a database, stores it in Azure Data Lake Storage Gen2, transforms it using Azure Databricks with PySpark and PySpark SQL, and prepares the final data for visualization.

## Architecture

Database
   ↓
Azure Data Factory
   ↓
ADLS Gen2 — Raw Data
   ↓
Azure Databricks
   ↓
PySpark / PySpark SQL
   ↓
ADLS Gen2 — Curated Data
   ↓
Power BI / Tableau

## Technologies

- Azure Data Factory
- Azure Data Lake Storage Gen2
- Azure Databricks
- PySpark
- PySpark SQL
- Power BI
- Tableau
- Azure DevOps Git

## Project Workflow

### 1. Data Ingestion
Azure Data Factory is used to create and orchestrate the data ingestion pipeline from the source database.

### 2. Raw Data Storage
The ingested data is stored in Azure Data Lake Storage Gen2 as raw data.

### 3. Data Transformation
Azure Databricks is used to clean and transform the data using PySpark and PySpark SQL.

### 4. Curated Data
The transformed data is stored back in ADLS Gen2 as analytics-ready data.

### 5. Visualization
The final dataset can be connected to Power BI or Tableau for dashboards, reporting, and business insights.

## Repository Structure

```text
├── dataset/
├── linkedService/
├── pipeline/
├── README.md
└── publish_config.json
