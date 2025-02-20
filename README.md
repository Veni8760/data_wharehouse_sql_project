#🏢 Data Warehouse and Analytics Project 

The project is a data whare housing and analytics solution. Building a data warehouse to generate actionable insight. This project higlights industry practices in data engineering and analytics.

## 📚 Project Overview

This project involves:

1. **Data Architecture**: Designing a Modern Data Warehouse Using Medallion Architecture **Bronze**, **Silver**, and **Gold** layers.
2. **ETL Pipelines**: Extracting, transforming, and loading data from source systems into the warehouse.
3. **Data Modeling**: Developing fact and dimension tables optimized for analytical queries.
4. **Analytics & Reporting**: Creating SQL-based reports and dashboards for actionable insights.

## 🚀 Requiremnets

### Building a Data Warehouse 

### Goal

Build a data warehouse using SQL server to consolidate sales data, enabling  informed decision-making and analytical reporting

#### Specifications
- **Data Sources**: From two source systems (ERP and CRM) import data which are provided as CSV files.
- **Data Quality**: Cleanse and resolve data quality issues to analysis
- **Integration**: Combine both sources into single, user-friendly data model designed for analytical queries
- **Scope**: Focus on the latest dataset only: historization of data is not required.
- **Documentation**: Provide clear documentation of the data model to support both business stakeholders and analytics teams.

### BI: Reporting & Analytics

### Goal

Develop SQL-based analytics to deliver detailed insights into:
-**Customer Behaviour**
-**Product Performance**
-**Sales Trends**

These insights empower stakeholders with key business metrics, enabling strategic decision-making.

## 🏗️ Data Architecture  
This project follows the **Medallion Architecture** (Bronze, Silver, Gold layers) to ensure efficient **data processing, storage, and analytics**.

### **🔸 Bronze Layer (Raw Data)**
- Stores **raw data as-is** from source systems (CSV files).
- No transformations or processing applied.
- Acts as a **landing zone** for all source data.

### **⚪ Silver Layer (Transformed Data)**
- **Cleansed, standardized, and normalized** data.
- Data transformations applied to ensure **data quality**.
- Combines multiple sources (ERP & CRM) into a **structured format**.

### **🟡 Gold Layer (Business-Ready Data)**
- **Optimized for reporting and analytics**.
- Implements **Star Schema** with **Fact & Dimension tables**.
- Used for **BI reports, dashboards, and insights**.

## 🖥️ **Data Flow & Architecture Diagrams**
![Data Architecture](https://github.com/user-attachments/assets/65e2b1d1-879b-461f-81ae-ccb8ec154d47)
![DataMart Star Schema](https://github.com/user-attachments/assets/2c4bdaf6-d896-4fed-aaf7-f72621783b00)
![Data Flow](https://github.com/user-attachments/assets/e24d7a2f-718b-43f9-8f45-80a57d57e1ab)
![Integration_Model drawio (1)](https://github.com/user-attachments/assets/06ddb552-4248-4bdc-8660-50a5aa40496c)

---

## 📖 **Project Scope & Features**
### **✅ Data Engineering & Warehouse Development**
- Build a **Modern Data Warehouse** using **SQL Server**.
- Consolidate **ERP & CRM sales data** for analytics.
- Ensure **data quality** before analysis.
- Document the **data model** for stakeholders.

### **✅ ETL Pipelines**
- **Extract**: Load CSV data into the **SQL Server database**.
- **Transform**: Clean, standardize, and normalize the data.
- **Load**: Store **business-ready data** in optimized **fact & dimension tables**.

### **✅ Data Modeling**
- Uses **Star Schema** for fast analytical queries.
- Creates **Fact Tables (Sales, Orders, etc.)**.
- Develops **Dimension Tables (Customers, Products, Dates, etc.)**.

### **✅ Analytics & Reporting**
- Write **SQL queries** for **business insights**.
- Enable **ad-hoc reporting** for decision-making.

---

## 🛠️ **Tech Stack & Tools**
Everything used in this project is **free** and open-source.

| Tool | Purpose |
|------|---------|
| **SQL Server Express** | Lightweight database for hosting the Data Warehouse |
| **SQL Server Management Studio (SSMS)** | GUI tool for managing & querying SQL Server |
| **Git & GitHub** | Version control & collaboration |
| **DrawIO** | Creating Data Flow, Star Schema, and Integration diagrams |
| **Notion** | Project planning and documentation Here is the link to my notion https://www.notion.so/Data-Warehouse-Project-19eb17e7381b80e59f21c1d2341adaeb?pvs=4|
| **CSV Files** | Source data from ERP & CRM systems |

---

## 🚀 **Project Setup & Requirements**
### **1️⃣ Install Required Tools**
- [Download SQL Server Express](https://www.microsoft.com/en-us/sql-server/sql-server-downloads)
- [Download SQL Server Management Studio (SSMS)](https://aka.ms/ssmsfullsetup)
- [Install Git & Set Up GitHub](https://git-scm.com/downloads)
- Install **DrawIO** for **Data Flow diagrams**.
- Use **Notion** for documentation (optional).

### **2️⃣ Set Up Database & Tables**
- Create the **Data Warehouse (`DataWarehouse`)** in SQL Server.
- Run the **DDL scripts** to create tables.
- Load CSV data into the **Bronze Layer**.

### **3️⃣ Execute ETL Process**
- Run **SQL scripts** to **transform and clean data** (Silver Layer).
- Create **Fact & Dimension tables** in the **Gold Layer**.

### **4️⃣ Run Analytics & Queries**
- Use **SQL queries** to generate reports.
- Build **dashboards** using BI tools.
---

## 📂 **Project Structure**
```bash

data-warehouse-project/
│
├── datasets/                           # Raw datasets used for the project (ERP and CRM data)
│
├── docs/                               # Project documentation and architecture details and DraIO
│
├── scripts/                            # SQL scripts for ETL and transformations
│   ├── bronze/                         # Scripts for extracting and loading raw data
│   ├── silver/                         # Scripts for cleaning and transforming data
│   ├── gold/                           # Scripts for creating analytical models
│
├── tests/                              # Test scripts and quality files
│
├── README.md                           # Project overview and instructions
├── LICENSE                             # License information for the repository
├── .gitignore                          # Files and directories to be ignored by Git
└── requirements.txt                    # Dependencies and requirements for the project
