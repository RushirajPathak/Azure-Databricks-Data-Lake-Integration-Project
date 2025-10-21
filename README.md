# 🧠 Azure Databricks Data Lake Integration Project

## 📘 Overview
This project demonstrates a **complete end-to-end data engineering pipeline** using **Microsoft Azure Databricks** and **Azure Data Lake Storage (ADLS Gen2)**.  
It covers data ingestion, transformation, and visualization using Apache Spark (PySpark) in the Databricks environment.  
The workflow follows an ELT (Extract, Load, Transform) pattern and is implemented using Databricks notebooks integrated with Azure services.

---

## 🚀 Project Objectives
- Set up and configure **Azure Databricks Workspace & Cluster**  
- Create and connect to **Azure Data Lake Storage (ADLS Gen2)**  
- Ingest raw data (`sales.csv`) from a **source container**  
- Perform data cleaning and transformation using **PySpark**  
- Write transformed data back to a **destination container** in ADLS  
- Register the processed data as a **Delta Table** in Databricks  
- Query and visualize aggregated results directly within Databricks  

---

## 🏗️ Architecture Diagram
```text
Azure Portal
│
├── Resource Group (RG_DataLake)
│    ├── Storage Account (ADLS Gen2)
│    │     ├── Container: source
│    │     └── Container: destination
│    └── Databricks Workspace
│          ├── Cluster (Single Node)
│          ├── Notebook (PySpark code)
│          └── Metastore (Delta Table)
│
└── Visualization: Databricks Dashboards (Bar + Pie Charts)
