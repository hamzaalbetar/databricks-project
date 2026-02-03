🚀 Databricks Data Lakehouse Project
 Designed & Implemented by Hamza Albetar
🎯 Project Purpose

This project implements an end-to-end Data Engineering pipeline on Databricks using PySpark and Delta Lake.
It integrates data from two enterprise systems:

📁 CRM System

📁 ERP System

The goal is to transform raw CSV files into structured, analytics-ready tables following the Medallion Architecture (Bronze → Silver → Gold).

🧱 Architecture Overview

🥉 Bronze Layer – Raw Ingestion

Read original CSV files

Store as Delta tables

No transformations

Preserve source data as single source of truth

🥈 Silver Layer – Cleansed & Integrated

Data cleaning & normalization

Schema standardization

Integration between CRM and ERP domains

📌 Silver Tables

Silver_crm_cust_info

Silver_crm_prd_info

Silver_crm_sales_details

Silver_erp_cust_az12

Silver_erp_loc_a101

Silver_erp_px_cat_g1v2

🥇 Gold Layer – Dimensional Model

Gold.dim_customers

Gold.dim_products

Gold.fact_sales

Built using Star Schema to support analytics and BI workloads.

🛠 Technologies Used

Databricks

Apache Spark – PySpark

Delta Lake

GitHub

SQL Analytics

⚙ Pipeline Execution

Execution order:

Bronze notebooks

Silver notebooks

Gold notebooks

Validation stage

🟡 Current mode: Manual Databricks Job

✅ Data Quality Rules

No null values in business keys

Unique customer & product IDs

Positive sales amounts

Referential integrity between fact and dimensions

📦 Project Outcome

Unified enterprise Data Lakehouse

Clean Delta architecture

Analytics-ready model

Ready foundation for BI & ML

