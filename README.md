# db-pipeline
This project shows how to design and build a complete end-to-end data pipeline that ingests data from multiple source systems and consolidates them into a single source of truth for analytics and reporting.

The pipeline extracts data from:

SQL Server

MySQL

Excel files

SAP (demo via exported data)

and loads them into a centralised SQL Server database hosted on Azure.

**The system supports:**

Incremental data loading (updates and deletes)

Near real-time processing using micro-batch scheduling

Data transformation and standardisation

Basic data quality checks

Audit logging and monitoring

Role-based access for analysts

Protection of sensitive (PII) data

All tools used in this project are free and open-source.

**Objectives**

Build a reliable and scalable data pipeline using Python and SQL

Implement a layered architecture (Raw → Staging → Mart)

Create a single trusted dataset for analysts

Handle updates and deletes from source systems

Demonstrate real-world data engineering practices

Keep infrastructure cost minimal

Architecture Overview

Sources → Raw Layer → Staging Layer → Mart Layer → Analytics

Sources: SQL Server, MySQL, Excel, SAP

Raw Layer: Stores extracted data in original format

Staging Layer: Cleans and standardises data

Mart Layer: Curated tables for reporting and analytics

Orchestration: Prefect (scheduled every minute)

Version Control: GitHub

Technology Stack

Python

SQL Server (destination)

Prefect (orchestration)

GitHub (version control)

Pandas / SQLAlchemy / PyODBC

Optional: dbt Core
