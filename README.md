# MS_SQL_Server_Project
I designed and built an end-to-end Enterprise Data Warehouse using MS SQL Server. I consolidated raw CRM and ERP datasets by building a 3-layer Medallion Architecture (Bronze, Silver, Gold) and transformed them into a performance-optimized Star Schema. Through this project, I gained deep hands-on experience in writing complex joins, crafting stored procedures, handling data quality validation, and designing analytical schemas

Problem Statement

As my business data grew across disparate source systems (CRM and ERP), it was stored in raw CSV files without a centralized system. This caused several challenges:

    Siloed & Raw Data: Data was scattered across different formats with quality issues, making it impossible to analyze directly.

    Lack of Historical & Structured Insight: Without a central data warehouse, stakeholders could not track key metrics regarding customer behavior, product performance, or sales trends.

    Absence of Standardized Analytics: There was no streamlined ETL process to clean, transform, and model the data for reliable business reporting.

🎯 Project Requirements

To solve these data challenges, I set out to build a modern analytics solution with the following specifications:

    Multi-Source Ingestion: Ingest raw data from two distinct source systems (CRM and ERP CSV files).

    Data Cleansing & Quality: Resolve data quality issues, standardize formats, and normalize data prior to analysis.

    Modern Architecture Design: Build a scalable data warehouse using MS SQL Server following the Medallion Architecture (Bronze, Silver, Gold layers).

    Dimensional Modeling: Develop a user-friendly Star Schema (fact and dimension tables) optimized for analytical reporting.

    Business Insights: Deliver actionable SQL-based insights into customer behavior, product performance, and sales trends.

💡 Solution

To fulfill these requirements, I built an end-to-end data warehouse and analytics pipeline:

    Implemented a 3-Layer Medallion Architecture:

        Bronze Layer: I ingested raw CRM and ERP CSV data directly into MS SQL Server as-is to preserve source integrity.

        Silver Layer: I developed SQL transformation scripts to clean, standardize, and fix data quality issues.

        Gold Layer: I modeled the clean data into a star schema (fact and dimension tables) tailored for high-performance reporting.

    Automated ETL & Quality Pipelines: I wrote modular SQL scripts for extracting, transforming, and loading data across all layers, complemented by automated SQL testing scripts to ensure data integrity.
