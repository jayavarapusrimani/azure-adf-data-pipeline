# Customer Account Data Pipeline using Azure Data Factory

## Overview

This project demonstrates an end-to-end ETL pipeline built using Azure Data Factory to process customer account datasets. The pipeline ingests, transforms, and loads data into Azure SQL Database using a layered architecture (Bronze, Silver, Gold).

---

## Architecture

The pipeline follows a multi-layer data architecture:

* **Bronze Layer**: Raw data ingestion from CSV files into ADLS Gen2
* **Silver Layer**: Data cleaning, transformation, and deduplication using ADF Dataflows
* **Gold Layer**: Processed and structured data loaded into Azure SQL Database for reporting

---

## Tools & Technologies

* Azure Data Factory (ADF)
* Azure Data Lake Storage Gen2 (ADLS)
* Azure SQL Database
* Azure Key Vault
* Power BI

---

## Data Flow

1. Source data (accounts, customers, loans, transactions) is ingested into ADLS (Bronze layer)
2. ADF pipelines are used to orchestrate data movement
3. Dataflows are applied for transformation, cleansing, and schema mapping
4. SCD Type 1 & Type 2 logic is implemented for historical data tracking
5. Processed data is loaded into Azure SQL Database (Gold layer)
6. Data is visualized using Power BI dashboards

---

## Key Features

* Built end-to-end ETL pipeline using Azure Data Factory
* Implemented Bronze, Silver, Gold architecture
* Used ADF Dataflows for data transformation and cleansing
* Implemented SCD Type 1 & Type 2 logic
* Built parameterized pipelines for reusability
* Scheduled pipelines for automated execution
* Secured credentials using Azure Key Vault

---

## Project Structure

/adf-pipelines/
/dataflows/
/adls-data/
/sql-scripts/
/architecture-diagram/

---

## Screenshots

(Add screenshots here)

* ADF Pipeline Design
* Dataflow Transformation
* Pipeline Trigger / Schedule
* Azure SQL Output Tables

---

## Learnings

* Hands-on experience with Azure Data Factory pipelines and Dataflows
* Understanding of ETL process and data transformation techniques
* Experience in implementing SCD Type 1 & Type 2
* Knowledge of data pipeline orchestration and scheduling

---

## Conclusion

This project demonstrates the ability to build scalable and automated ETL pipelines using Azure Data Factory, following industry-standard data engineering practices.
