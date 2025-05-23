# End-to-End ELT Pipeline with Airbyte, Snowflake, and dbt

## Overview

This project demonstrates a modern ELT (Extract, Load, Transform) pipeline using Airbyte for ingestion, Snowflake for scalable data warehousing, and dbt for transformation and modeling. The goal was to build a reproducible data workflow capable of ingesting raw survey data, cleaning it, and producing ready-to-analyze views.

## Business Relevance

Modern organizations rely on clean, reliable, and well-modeled data to drive decisions. This project simulates a realistic use case where:

- Airbyte automates ingestion from external sources (e.g., CSVs, APIs)
- Snowflake serves as a cloud-native, scalable storage solution
- dbt transforms raw staging data into analysis-ready formats

Such pipelines are essential for:
- Building robust analytics stacks
- Enabling self-serve BI dashboards
- Supporting machine learning and forecasting workflows

## Tools & Technologies Used

- **Airbyte**: Open-source ELT platform for extracting and loading raw data
- **Snowflake**: Scalable cloud-based data warehouse
- **dbt (Data Build Tool)**: SQL-based transformation layer for analytics engineering
- **Miniconda**: For isolated environment setup
- **YAML & dbt profiles**: For credential and configuration management

## Problem Statement

How can we automate the ingestion and transformation of external datasets into an analytics-ready warehouse structure using a cloud-native ELT architecture?

## Approach

1. **Ingestion with Airbyte**
   - Configured source connectors for public survey data
   - Loaded into Snowflake with minimal manual setup

2. **Data Modeling with dbt**
   - Cleaned and renamed raw columns using SQL transformations
   - Created staging and final reporting views
   - Used Jinja templating to dynamically generate model logic

3. **Orchestration and Debugging**
   - Worked in a conda-based isolated environment
   - Verified connections and pipeline stability via CLI and logs

## Results

- Successfully ingested and transformed a structured dataset using best practices in ELT
- Produced a normalized view (`transform_survey`) with readable column names and clean types
- Demonstrated a clear separation between staging (raw) and transformed (reporting) layers

## Future Improvements

- Automate pipeline execution with a scheduler like Airflow or Prefect
- Add data validation tests using dbt test framework
- Expand to real-time sources (e.g., REST APIs, event data)

## Contact

If you're looking to design or scale modern data pipelines for analytics, BI, or machine learning, feel free to reach out:

**Email**: [mmgupta2@wisc.edu](mailto:mmgupta2@wisc.edu)  
**LinkedIn**: [linkedin.com/in/mihirmgupta](https://www.linkedin.com/in/mihirmgupta/)

