#🚀 Databricks Data Lakehouse Project
Designed & Implemented by Hamza Albetar
##🎯 Project Purpose

This project demonstrates a complete Data Engineering pipeline built on Databricks using PySpark and Delta Lake.
It integrates data from:

CRM System

ERP System

and transforms raw CSV files into analytics-ready tables following the Medallion Architecture.

#🧱 Architecture
##🥉 Bronze Layer – Raw Data

Ingest CSV files as Delta tables

No business transformation

Source of truth preservation

##🥈 Silver Layer – Clean & Integrated

Data cleansing

Schema standardization

Domain integration

Tables:

Silver.crm_cust_info

Silver.crm_prd_info

Silver.crm_sales_details

Silver.erp_cust_az12

Silver.erp_loc_z101

Silver.erp_az_prd_a1v2

##🥇 Gold Layer – Analytics Model

Gold.dim_cust

Gold.dim_prd

Gold.fact_sales

Built using Star Schema for BI workloads.

#🛠 Technologies

Databricks

PySpark

Delta Lake

GitHub

SQL Analytics

#⚙ Execution Flow

Run Bronze notebooks

Run Silver notebooks

Run Gold notebooks

Validate results

Current mode: Manual Job Execution

#✅ Data Quality Rules

No null business keys

Unique IDs

Positive amounts

Referential integrity
