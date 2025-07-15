# OnlineRetail-Sales
# Data Warehousing and Business Intelligence Assignment (DWBI)

This repository contains both parts of the Data Warehousing and Business Intelligence (DWBI) coursework. It demonstrates the full BI pipeline — from data extraction and transformation using **SSIS**, to analytical processing using **SSAS**, and reporting with **Power BI**.

---
## 📁 Contents

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
### 📂  Folder Structure

OnlineRetail-Sales/
│
├── Assignment_01_DataWarehouse/
│   ├── Documents/                 # Assignment 1 Report (PDF with steps, screenshots)
│   ├── SSIS_Package/              # SSIS packages (.dtsx, solution files)          
│   ├── Sources/                   # Original CSV/Text files used in ETL
│
├── Assignment_02_BI_Analytics/
│   ├── Cube/                      # SSAS SSDT cube project
│   ├── Document/                  # Assignment 2 Report (PDF with steps, screenshots)
│   ├── Excel_reports/             # OLAP Excel file (.xlsx)
│   ├── PowerBI_Reports/           # Power BI .pbix reports 
│
├── README.md

### 📦 Assignment 01 – Data Warehouse Design & ETL

This part focuses on data warehouse creation and ETL pipelines using **SSIS**.

#### 🔹 Features:
- Selected an **OLTP dataset** from an online retail domain.
- Designed a **star schema** dimensional model:
  - FactSales (with accumulating fact columns)
  - DimProduct, DimCustomer, DimDate
- Implemented **SSIS packages** for:
  - Loading from multiple sources (CSV and SQL tables)
  - Data cleansing and transformation
  - Handling **Slowly Changing Dimensions (SCD)**
  - Maintaining **accumulating fact table** logic with time tracking
- Documented with diagrams, ETL flows, and explanations.

📂 Folder: `Assignment_01_DataWarehouse`

---

### 📊 Assignment 02 – Business Intelligence & Analytics

This part builds on the data warehouse to implement analytical capabilities using **SSAS**, **Excel OLAP**, and **Power BI**.

#### 🔹 Features:
- Created an **SSAS cube** with:
  - Proper measures and dimensions
  - Hierarchies (e.g., Date hierarchy: Year → Quarter → Month)
- Demonstrated OLAP operations via **Excel**:
  - Roll-up, Drill-down, Slice, Dice, Pivot
- Developed four interactive **Power BI reports**:
  1. Matrix Report
  2. Cascading Slicers with Charts
  3. Drill-down Report
  4. Drill-through Report
- Published to Power BI Service and verified online access

📂 Folder: `Assignment_02_BI_Analytics`

---

## 🛠 Tools & Technologies

- Microsoft SQL Server
- SQL Server Integration Services (SSIS)
- SQL Server Analysis Services (SSAS)
- Excel (PowerPivot, PivotTables)
- Power BI Desktop + Power BI Service
- SQL, DAX

---

## 🧾 Documentation

Each assignment includes a PDF document under its respective folder, containing:
- Step-by-step process
- Screenshots of implementation
- ER diagrams and architecture
- Explanations of transformations, modeling, and decisions

---

## 👤 Author

- **Name**: Savindi Widyasekara    
- **Course**: BSc (Hons) in IT – Data Science  

---

Feel free to explore each folder to see how data was transformed from raw sources to a fully functional business intelligence solution.
