# Medallion-Architecture-Pipeline
Transform raw data into actionable insights! Full Azure pipeline project with ADF, Databricks, Delta Lake, and Power BI dashboards for real-time &amp; batch analytics.

## Step 1: Project Overview
**Objective:**  
Build a data pipeline that takes raw sales data, cleans and organizes it, and turns it into useful insights. Use Azure Data Factory, Databricks, and Delta Lake to process the data, and create interactive Power BI dashboards to help businesses make smart decisions.

**Skills Demonstrated:**  
- Azure Data Factory (ETL pipelines, incremental load)  
- Azure Databricks + PySpark (data transformation, Delta Lake)  
- Azure Synapse Analytics (Gold layer, analytical tables)  
- Power BI dashboards

## Step 2: Data Architecture
- Followed **Medallion Architecture** (Bronze → Silver → Gold) 
- ![Architecture Diagram](https://raw.githubusercontent.com/alpesh502/Medallion-Architecture-Pipeline/main/Architecture_diagram.png)


## Step 3: Data Sources
- Batch Data: CSV files (sales, products, customers)
- Datasets: [dataset_sample.csv](data/dataset_sample.csv)


## Step 4: Azure Setup
- Azure Free Account, Storage Account (ADLS Gen2), Databricks Workspace  
- Service Principal for secure access
- ![Azure Setup](https://raw.githubusercontent.com/alpesh502/Medallion-Architecture-Pipeline/main/AzureSetup.png)

## Step 5: Data Ingestion (Bronze Layer)
- ADF pipelines to copy raw data → ADLS Gen2  
- Parameterized pipelines for incremental loads
- ![Pipeline Overview](https://github.com/alpesh502/Medallion-Architecture-Pipeline/blob/main/Azure_data_pipeline.png)

## Step 6: Data Transformation (Silver Layer)
- Databricks notebooks for cleaning, joining, and transforming data  
- Stored Delta tables
- ![Bronze to Silver Transformation](https://raw.githubusercontent.com/alpesh502/Medallion-Architecture-Pipeline/main/transformation(bronze_to_silver).png)

## Step 7: Aggregation (Gold Layer)
- Synapse Analytics for aggregated tables  
- External tables using OPENROWSET()
- 

