
# Data Warehouse and Analytics Project

Welcome to the **Data Warehouse and Analytics Project** repository! 🚀  
This project demonstrates a comprehensive data warehousing and analytics solution, from building a data warehouse to generating actionable insights. Designed as a portfolio project, it highlights industry best practices in data engineering and analytics.

---
## 🏗️ Data Architecture

The data architecture for this project follows Medallion Architecture **Bronze**, **Silver**, and **Gold** layers:
![Data Architecture](docs/data_architecture.png)

1. **Bronze Layer**: Stores raw data as-is from the source systems. Data is ingested from CSV Files into SQL Server Database.
2. **Silver Layer**: This layer includes data cleansing, standardization, and normalization processes to prepare data for analysis.
3. **Gold Layer**: Houses business-ready data modeled into a star schema required for reporting and analytics.

---
## 📖 Project Overview

This project involves:

1. **Data Architecture**: Designing a Modern Data Warehouse Using Medallion Architecture **Bronze**, **Silver**, and **Gold** layers.
2. **ETL Pipelines**: Extracting, transforming, and loading data from source systems into the warehouse.
3. **Data Modeling**: Developing fact and dimension tables optimized for analytical queries.
4. **Analytics & Reporting**: Creating SQL-based reports and dashboards for actionable insights.

🎯 This repository is an excellent resource for professionals and students looking to showcase expertise in:
- SQL Development
- Data Architect
- Data Engineering  
- ETL Pipeline Developer  
- Data Modeling  
- Data Analytics  

---

## 🛠️ Important Links & Tools:

Everything is for Free!
- **[Datasets](datasets/):** Access to the project dataset (csv files).
- **[SQL Server Express](https://www.microsoft.com/en-us/sql-server/sql-server-downloads):** Lightweight server for hosting your SQL database.
- **[SQL Server Management Studio (SSMS)](https://learn.microsoft.com/en-us/sql/ssms/download-sql-server-management-studio-ssms?view=sql-server-ver16):** GUI for managing and interacting with databases.
- **[Git Repository](https://github.com/):** Set up a GitHub account and repository to manage, version, and collaborate on your code efficiently.
- **[DrawIO](https://www.drawio.com/):** Design data architecture, models, flows, and diagrams.
- **[Notion](https://www.notion.com/):** All-in-one tool for project management and organization.
- **[Notion Project Steps](https://thankful-pangolin-2ca.notion.site/SQL-Data-Warehouse-Project-16ed041640ef80489667cfe2f380b269?pvs=4):** Access to All Project Phases and Tasks.

---

## 🚀 Project Requirements

### Building the Data Warehouse (Data Engineering)

#### Objective
Develop a modern data warehouse using SQL Server to consolidate sales data, enabling analytical reporting and informed decision-making.

#### Specifications
- **Data Sources**: Import data from two source systems (ERP and CRM) provided as CSV files.
- **Data Quality**: Cleanse and resolve data quality issues prior to analysis.
- **Integration**: Combine both sources into a single, user-friendly data model designed for analytical queries.
- **Scope**: Focus on the latest dataset only; historization of data is not required.
- **Documentation**: Provide clear documentation of the data model to support both business stakeholders and analytics teams.

---

### BI: Analytics & Reporting (Data Analysis)

#### Objective
Develop SQL-based analytics to deliver detailed insights into:
- **Customer Behavior**
- **Product Performance**
- **Sales Trends**

These insights empower stakeholders with key business metrics, enabling strategic decision-making.  

For more details, refer to [docs/requirements.md](docs/requirements.md).

## 🚀 Getting Started

### Prerequisites
- SQL Server Express (free download)
- SQL Server Management Studio (SSMS)
- Basic knowledge of SQL and data warehousing concepts

### Quick Start
1. **Clone the repository**
   ```bash
   git clone https://github.com/dhanushshet14/sql-data-warehouse.git
   cd sql-data-warehouse
   ```

2. **Set up the database**
   - Run `scripts/init_database.sql` to create the initial database structure

3. **Load sample data**
   - Import CSV files from `datasets/` folders into your SQL Server instance
   - Execute bronze layer scripts to create raw data tables
   - Run silver layer transformations for data cleansing
   - Deploy gold layer star schema for analytics

4. **Explore the documentation**
   - Review data architecture diagrams in `docs/`
   - Check data catalog for field descriptions
   - Run quality tests from `tests/` folder

## 📂 Repository Structure
```
sql-data-warehouse/
│
├── datasets/                           # Raw datasets used for the project (ERP and CRM data)
│   ├── source_crm/                     # CRM system data files
│   │   ├── cust_info.csv              # Customer information
│   │   ├── prd_info.csv               # Product information
│   │   └── sales_details.csv          # Sales transaction details
│   └── source_erp/                     # ERP system data files
│       ├── CUST_AZ12.csv              # Customer data from ERP
│       ├── LOC_A101.csv               # Location data
│       └── PX_CAT_G1V2.csv            # Product category data
│
├── docs/                               # Project documentation and architecture details
│   ├── data_architecture.png          # Data architecture diagram
│   ├── data_catalog.md                # Catalog of datasets with field descriptions
│   ├── data_flow.png                  # Data flow diagram
│   ├── data_integration.png           # Data integration overview
│   ├── data_layers.pdf                # Medallion architecture layers documentation
│   ├── data_model.png                 # Star schema data model
│   ├── ETL.png                        # ETL process diagram
│   └── naming_conventions.md          # Naming guidelines for tables and columns
│
├── scripts/                            # SQL scripts for ETL and transformations
│   ├── bronze/                         # Scripts for raw data ingestion
│   │   ├── ddl_bronze.sql             # Bronze layer table definitions
│   │   └── proc_load_bronze.sql       # Bronze layer data loading procedures
│   ├── silver/                         # Scripts for data cleansing and transformation
│   │   ├── ddl_silver.sql             # Silver layer table definitions
│   │   └── proc_load_silver.sql       # Silver layer transformation procedures
│   ├── gold/                           # Scripts for analytical data models
│   │   └── ddl_gold.sql               # Gold layer star schema definitions
│   └── init_database.sql              # Database initialization script
│
├── tests/                              # Data quality and validation tests
│   ├── quality_checks_gold.sql        # Quality checks for gold layer
│   └── quality_checks_silver.sql      # Quality checks for silver layer
│
├── README.md                           # Project overview and instructions
├── LICENSE                             # MIT License
└── .$Archi.drawio.bkp                 # Architecture diagram backup
```
---


## 🛡️ License

This project is licensed under the [MIT License](LICENSE). You are free to use, modify, and share this project with proper attribution.
