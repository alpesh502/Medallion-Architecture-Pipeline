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
- **Dataset Folder:**  
- [View Dataset Files](https://github.com/alpesh502/Medallion-Architecture-Pipeline/tree/main/data)


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
- ![Synapse Analytics Gold Layer](https://raw.githubusercontent.com/alpesh502/Medallion-Architecture-Pipeline/main/Synapse_Analytics(Gold_Layer).png)

## Step 8: Project Conclusion

This project demonstrates how to build an end-to-end Azure Data Engineering pipeline using the Medallion Architecture (Bronze → Silver → Gold).

- In the **Bronze layer**, data was ingested from multiple sources into **Azure Data Lake Gen2** using **Azure Data Factory (ADF)**.  
- In the **Silver layer**, data was cleaned, joined, and transformed using **Azure Databricks** and **PySpark**.  
- In the **Gold layer**, the refined and aggregated data was stored in **Azure Synapse Analytics**, ready for advanced analytics or dashboard visualization.
- This project highlights the complete data flow from raw to processed data, ensuring **scalability, reliability, and performance** in the cloud using **Azure services**.
