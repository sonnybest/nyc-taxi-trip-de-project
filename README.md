# Azure Lakehouse Data Engineering Project

## Overview

This project demonstrates the design and implementation of a modern Azure Lakehouse architecture using the Medallion Architecture (Bronze, Silver, and Gold layers). The solution ingests raw NYC Taxi trip data for the year 2025, applies scalable transformations using Databricks and Apache Spark, and delivers curated datasets for business intelligence and downstream analytics through Power BI.

The architecture is designed to support enterprise-grade data engineering requirements including scalability, data quality, governance, security, and analytical performance.

---

## Architecture
<img width="1635" height="962" alt="image" src="https://github.com/user-attachments/assets/e388afea-d1f6-4886-95ce-067c08bee3dc" />


### Data Flow

Source Systems → Azure Data Factory → Bronze Layer → Silver Layer → Gold Layer → Power BI

### Medallion Architecture

#### Bronze Layer (Raw Data)

Raw data is ingested from source systems and APIs through Azure Data Factory and stored in Azure Data Lake Storage Gen2 using the Parquet format.

**Key Features**

* Immutable raw data storage
* Historical data retention
* Data lineage preservation
* Cost-efficient storage

#### Silver Layer (Validated Data)

Data is transformed using Databricks and Apache Spark. This layer applies business rules and data quality standards.

**Transformations**

* Data cleansing
* Deduplication
* Schema validation
* Null handling
* Data standardization
* Data enrichment

#### Gold Layer (Business-Ready Data)

Curated datasets are published using Delta Lake and optimized for reporting and analytics.

**Key Features**

* Star schema modeling
* Aggregated business metrics
* ACID transactions
* Schema enforcement
* Time travel
* High-performance analytical queries

---

## Technology Stack

| Category           | Technology                   |
| ------------------ | ---------------------------- |
| Orchestration      | Azure Data Factory           |
| Storage            | Azure Data Lake Storage Gen2 |
| Processing         | Databricks                   |
| Compute Engine     | Apache Spark                 |
| Data Format        | Parquet                      |
| Lakehouse Storage  | Delta Lake                   |
| Security           | Microsoft Entra ID           |
| Secrets Management | Azure Key Vault              |
| Reporting          | Power BI                     |

---

## Security & Governance

The platform incorporates enterprise security best practices:

* Role-Based Access Control (RBAC)
* Managed Identities
* Secret Management with Azure Key Vault
* Secure Authentication via Microsoft Entra ID
* Data Access Governance

---

## Key Engineering Concepts Demonstrated

* Lakehouse Architecture
* Medallion Architecture
* Distributed Data Processing
* ETL / ELT Design Patterns
* Data Modeling
* Data Quality Frameworks
* Data Governance
* Incremental Data Processing
* Enterprise Reporting

---

## Business Value

This solution transforms raw operational data into trusted analytical assets, enabling:

* Faster decision-making
* Improved data quality
* Scalable analytics
* Secure data access
* Self-service reporting
* Reduced operational complexity

---

## Skills Demonstrated

Azure Data Factory • Databricks • Apache Spark • Delta Lake • Azure Data Lake Storage Gen2 • Power BI • Data Modeling • ETL/ELT • Data Warehousing • Lakehouse Architecture • Medallion Architecture • Data Governance
