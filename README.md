# OnlineRetail-Sales
# Data Warehousing and Business Intelligence Assignment (DWBI)

This repository contains both parts of the Data Warehousing and Business Intelligence (DWBI) coursework. It demonstrates the full BI pipeline — from data extraction and transformation using **SSIS**, to analytical processing using **SSAS**, and reporting with **Power BI**.

---

## 📊 Dataset Description

The dataset used is the **Online Retail Dataset** from UCI/Kaggle, which contains transactional data from a UK-based online retail store. It includes customer purchases made between 2010 and 2011.

**Key Features:**
- `InvoiceNo`: Unique identifier for each transaction  
- `StockCode`: Product/item code  
- `Description`: Product description  
- `Quantity`: Number of items purchased  
- `InvoiceDate`: Date and time of transaction  
- `UnitPrice`: Price per item  
- `CustomerID`: Unique identifier for each customer  
- `Country`: Customer location

This dataset is suitable for analyzing **sales performance**, **customer behavior**, and **product trends** across time and geography.

---

## 📦 Part 1: ETL and Data Warehouse Design (SSIS)

**Tools Used:** SQL Server, SSIS, Excel/CSV  
- Extracted data from a CSV file and a SQL Server table (hybrid data sources).  
- Applied transformations (data cleaning, type conversions, derived columns).  
- Loaded data into a **star schema** in the data warehouse.  
- Designed:
  - **Slowly Changing Dimension (SCD)** for customer data  
  - **Accumulating Fact Table** for sales transactions  
- Created the following tables:
  - `DimProduct` – Product metadata
  - `DimCustomer` – Customer details and country
  - `DimDate` – Calendar-based breakdown
  - `FactSales` – Measures like Quantity, TotalAmount, etc.

📁 Folder: `/ETL_SSIS/`

---

## 📈 Part 2: OLAP and Reporting (SSAS & Power BI)

**Tools Used:** SSAS, Excel, Power BI  
- Built a **SSAS cube** with hierarchies and calculated measures  
- Conducted OLAP operations: **drill-down**, **slicing**, **filtering**  
- Connected Excel to the cube for pivot-based exploration  
- Created Power BI dashboards featuring:
  - **Matrix report** showing sales by product and country  
  - **Cascading slicers** for region and product  
  - **Drill-down** into monthly sales trends  
  - **Drill-through** into customer-level data

📁 Folder: `/SSAS_PowerBI/`

---

## 🗂️ Repository Structure

DWBI-Assignment/
├── ETL_SSIS/
│ ├── SSIS_Package.dtsx
│ └── SQL_Scripts/
├── SSAS_PowerBI/
│ ├── CubeProject/
│ └── PowerBIReports/
│ └── SalesDashboard.pbix
└── README.md

## ✅ Summary

This project demonstrates a complete BI solution, from:
- Data extraction (CSV + SQL Server)
- Warehouse design and ETL (SSIS)
- Analytical cube development (SSAS)
- Insightful visualization (Power BI)

It highlights technical skills in **data modeling**, **ETL processes**, and **business reporting**.
