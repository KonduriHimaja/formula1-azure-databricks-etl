# Azure_databricks-project
# 🏎️ Formula 1 Data Engineering Project

## Overview

This project demonstrates the implementation of an end-to-end data engineering pipeline using Azure Databricks and the Medallion Architecture (Bronze, Silver, Gold) to process Formula 1 racing data.

The pipeline ingests raw Formula 1 datasets, performs data cleansing and transformations using PySpark, and creates analytics-ready datasets for reporting and business insights.

---

## Business Problem

Formula 1 generates large volumes of race-related data including:

* Driver information
* Constructor details
* Race schedules
* Lap times
* Race results
* Circuits information

The objective is to build a scalable data platform that:

* Ingests raw Formula 1 data
* Applies data quality validations
* Transforms and enriches datasets
* Creates curated analytical datasets
* Supports reporting and dashboarding

---

## Solution Architecture

Raw Data → Bronze Layer → Silver Layer → Gold Layer → Reporting

### Bronze Layer

* Stores raw source files
* Minimal transformations
* Historical data preservation

### Silver Layer

* Data cleansing
* Schema enforcement
* Data standardization
* Deduplication
* removin null values

### Gold Layer

* Business-ready datasets
* Aggregated metrics
* Reporting tables

#### Analytics layer 
 * creating driver standings and constructor standings for analysis

---

## Technology Stack

| Technology                   | Purpose               |
| ---------------------------- | --------------------- |
| Azure Databricks             | Data Processing       |
| Apache Spark                 | Distributed Computing |
| PySpark                      | ETL Development       |
| Delta Lake                   | Storage Format        |
| Azure Data Lake Storage Gen2 | Data Storage          |
| GitHub                       | Version Control       |


---

## Data Sources

Formula 1 datasets include:

* Drivers
* Constructors
* Circuits
* Races
* Results

Source Format:

* CSV
* JSON

---

## ETL Pipeline Workflow

### Step 1: Data Ingestion

* Read source files from ADLS
* Apply schema validation
* Store data in Bronze layer

### Step 2: Data Transformation

* Clean null values
* Standardize column names
* Remove duplicates
* Apply business rules

### Step 3: Data Enrichment

* Join driver, constructor and race data
* Generate derived columns
* Create analytical datasets

### Step 4: Data Aggregation

Generate:

* Driver standings
* Constructor standings
* Race statistics
* Performance metrics

### Step 5: Gold Layer Creation

Publish business-ready datasets for reporting.

---

## Key Data Engineering Concepts Implemented

### Data Lakehouse Architecture

* Bronze Layer
* Silver Layer
* Gold Layer


### Data Quality

* Schema Validation
* Null Checks
* Duplicate Removal
* Data Consistency Checks


## Sample Business Insights

### Driver Performance Analysis

* Total wins by driver
* Average finishing position
* Fastest laps

### Constructor Analysis

* Team standings
* Season performance
* Podium finishes

---

## How to Run

### Clone Repository

```bash
git clone https://github.com/KonduriHimaja/Formula1-Azure_databricks_ETL_Pipeline.git
```

### Configure Environment

Update configuration files:

```python
storage_account_name
container_name
bronze_path
silver_path
gold_path
```

### Execute Notebooks

Run in sequence:

1. Ingestion
2. Transformation
3. Aggregation
4. Analytics
---

## Skills Demonstrated

* Data Engineering
* Azure Databricks
* PySpark
* Delta Lake
* Data Modeling
* ETL Development
* Data Lakehouse Architecture
* Performance Optimization
* SQL Analytics

---

## Author

Himaja Konduri

Aspiring Data Engineer | Azure Databricks | PySpark | SQL | Data Engineering Projects

LinkedIn: https://www.linkedin.com/in/konduri-himaja/

GitHub: https://github.com/KonduriHimaja
