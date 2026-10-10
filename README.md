# MS_SQL_Server_Project
I designed and built an end-to-end Enterprise Data Warehouse using MS SQL Server. I consolidated raw CRM and ERP datasets by building a 3-layer Medallion Architecture (Bronze, Silver, Gold) and transformed them into a performance-optimized Star Schema. Through this project, I gained deep hands-on experience in writing complex joins, crafting stored procedures, handling data quality validation, and designing analytical schemas

🚨 Problem Statement

As my business data grew across disparate source systems (CRM and ERP), it was stored in raw CSV files without a centralized system. This caused several challenges:

    Siloed & Raw Data: Data was scattered across different formats with quality issues, making it impossible to analyze directly.

    Lack of Historical & Structured Insight: Without a central data warehouse, stakeholders could not track key metrics regarding customer behavior, product performance, or sales trends.

    Absence of Standardized Analytics: There was no streamlined ETL process to clean, transform, and model the data for reliable business reporting.

🏗️ Project Architecture & Solution Overview

To solve the challenges of fragmented enterprise data, I architected and built an end-to-end data warehouse and analytics pipeline using MS SQL Server, meeting the following specifications:

    Multi-Source Ingestion: Ingested raw data from two distinct source systems (CRM and ERP CSV files).

    Data Cleansing & Quality: Resolved data quality issues, standardized formats, and normalized data prior to analysis.

    Modern Architecture Design: Built a scalable data warehouse following the Medallion Architecture (Bronze, Silver, Gold layers).

    Dimensional Modeling: Developed a user-friendly Star Schema (fact and dimension tables) optimized for analytical reporting.

    Business Insights: Delivered actionable SQL-based insights into customer behavior, product performance, and sales trends.

📂 How I Implemented It (Repository Breakdown)

To fulfill these requirements, I structured my project into a production-grade codebase:

    datasets/ (Source Layer):

        "I started by ingesting raw CRM and ERP data from CSV files. This represents the raw entry point of data into the ecosystem."

    scripts/ (The ETL Engine):

        bronze/: "Here, I wrote scripts to load raw data as-is into SQL Server staging tables with zero modifications to maintain audit history."

        silver/: "This is where the heavy lifting happens. I wrote T-SQL transformation scripts to handle string cleansing, standardizing formats, casting data types, and resolving null anomalies."

        gold/: "I designed a high-performance Star Schema, structuring fact and dimension tables optimized specifically for fast analytical queries and business reporting."

    tests/ (Data Quality & Validation):

        "I built automated test scripts to validate referential integrity, check for orphan keys, and ensure no data loss happened across the pipeline transitions."

    docs/ (Architecture & Governance):

        "I maintained comprehensive documentation including data catalogs, architecture diagrams, and naming conventions to ensure proper data governance."
