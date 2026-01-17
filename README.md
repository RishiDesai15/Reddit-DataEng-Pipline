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

Reddit API
↓
Apache Airflow (DAGs)
↓
Amazon S3 (Raw Data)
↓
AWS Glue (Transform & Catalog)
↓
Amazon Athena
↓
Amazon Redshift (Analytics)

---

## Pipeline Workflow

1. **Extract**
   - Fetch Reddit data via API using Airflow DAGs

2. **Transform**
   - Clean and normalize raw JSON data
   - Apply schema transformations using AWS Glue

3. **Load**
   - Store processed data in S3
   - Load analytics-ready data into Redshift

4. **Analyze**
   - Query data using Athena and Redshift

---

## Project Structure

reddit-etl-pipeline/
│
├── dags/ # Airflow DAGs
├── scripts/ # Extraction and transformation scripts
├── glue_jobs/ # AWS Glue ETL scripts
├── sql/ # Athena and Redshift queries
├── docker-compose.yml # Airflow and Celery setup
├── requirements.txt # Python dependencies
└── README.md

---

## Setup Instructions

### Prerequisites

- Python 3.9+
- Docker & Docker Compose
- AWS account
- Reddit API credentials

---

### Clone Repository

```bash
git clone https://github.com/your-username/reddit-etl-pipeline.git
cd reddit-etl-pipeline
