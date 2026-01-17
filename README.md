# Reddit End-to-End ETL Data Pipeline

An end-to-end ETL data pipeline that extracts data from Reddit using its API, orchestrates workflows with Apache Airflow, and processes data using AWS services including S3, Glue, Athena, and Redshift.

This project demonstrates a production-style data engineering pipeline using modern cloud-native tools and best practices.

---

## Project Overview

The pipeline automates the ingestion of Reddit data, transforms raw JSON into analytics-ready datasets, and loads the data into a cloud data warehouse for querying and analysis.

---

## What This Project Does

- Extracts Reddit posts and metadata using the Reddit API
- Orchestrates ETL workflows with Apache Airflow and Celery
- Stores raw and processed data in Amazon S3
- Uses AWS Glue for data cataloging and transformations
- Queries transformed data using Amazon Athena
- Loads curated data into Amazon Redshift for analytics
- Enables downstream analysis and visualization

---

## Tech Stack

- **Orchestration:** Apache Airflow, Celery
- **Data Source:** Reddit API
- **Storage:** Amazon S3
- **Metadata Store:** PostgreSQL
- **ETL & Catalog:** AWS Glue
- **Query Engine:** Amazon Athena
- **Data Warehouse:** Amazon Redshift
- **Cloud Platform:** AWS

---

## Architecture

