# Uber-GCP-ELT-pipeline

## Overview
This project implements an end-to-end data pipeline for processing and analyzing ecommerce customer data using Google Cloud services, Mage for ELT, and BigQuery for storage and querying.

## Architecture
![architecture](https://github.com/sahilbishnoi26/Uber-GCP-ELT-pipeline/blob/main/architecture.jpg)
- **Data Source**: Sample ecommerce customer data stored in a PostgreSQL database.
- **Extract & Load (ELT)**: Mage orchestrates data extraction from PostgreSQL and loads it into Google Cloud Storage (GCS) as Parquet files.
- **Data Transformation**: Mage processes and cleans the data before writing it to BigQuery.
- **Storage & Querying**: BigQuery serves as the data warehouse for analysis.
- **Visualization**: Google Looker Studio is used for dashboarding and insights.

## Tools & Technologies
- **Google Cloud Platform (GCP)**: Cloud Storage, BigQuery
- **Mage**: Open-source ELT tool for data orchestration
- **PostgreSQL**: Source database
- **Google Looker Studio**: Data visualization

## Data Model

TLC Trip Record Data Yellow and green taxi trip records include fields capturing pick-up and drop-off dates/times, pick-up and drop-off locations, trip distances, itemized fares, rate types, payment types, and driver-reported passenger counts.
![architecture](https://github.com/sahilbishnoi26/Uber-GCP-ELT-pipeline/blob/main/data_model.jpg)

## Setup & Execution
1. **Provision Resources**
   - Set up a Google Cloud project.
   - Enable Cloud Storage and BigQuery.
   - Create a service account with necessary permissions.

2. **Configure PostgreSQL**
   - Ensure the database is accessible.
   - Prepare customer transaction data.

3. **Set Up Mage**
   - Install and configure Mage.
   - Create a pipeline to extract data from PostgreSQL and load it into GCS.

4. **Transform and Load into BigQuery**
   - Define transformation steps in Mage.
   - Load processed data into BigQuery tables.

5. **Analyze and Visualize**
   - Use SQL queries in BigQuery for analysis.
   - Connect BigQuery to Looker Studio for reporting.

## Key Features
- Automated ELT pipeline with Mage
- Scalable data storage using BigQuery
- Efficient data transformation and cleansing
- Visualization with Looker Studio

## Future Improvements
- Implement real-time data ingestion
- Enhance transformations for deeper insights
- Optimize query performance in BigQuery

