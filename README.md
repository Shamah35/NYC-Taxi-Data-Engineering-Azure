# NYC Taxi Data Engineering Project on Azure

## Project Overview

This project implements an end-to-end data engineering pipeline using Microsoft Azure services to ingest, store, transform and process NYC Taxi Trip Record data.

The project uses a Medallion Architecture consisting of Bronze, Silver and Gold layers.

## Technologies Used

- Azure Data Factory
- Azure Data Lake Storage Gen2
- Azure Databricks
- PySpark
- Python
- GitHub

## Data Source

NYC Taxi and Limousine Commission (TLC)

https://www.nyc.gov/site/tlc/about/tlc-trip-record-data.page

## Architecture

NYC TLC Trip Record Data
        |
        v
Azure Data Factory
        |
        v
Bronze Layer
(Raw Data)
        |
        v
Azure Databricks
        |
        v
Silver Layer
(Cleaned and Transformed Data)
        |
        v
Azure Databricks
        |
        v
Gold Layer
(Analytics-Ready Data)

## Project Implementation

### 1. Data Ingestion
Azure Data Factory is used to orchestrate the ingestion of NYC TLC trip data into Azure Data Lake Storage Gen2.

### 2. Bronze Layer
Raw source data is stored in the Bronze layer.

### 3. Silver Layer
Azure Databricks and PySpark are used to clean and transform the ingested data.

### 4. Gold Layer
Processed data is written into the Gold layer for downstream analytics.

## Storage Structure

- Bronze
  - trip2023data
  - trip_type
  - trip_zone

- Silver
  - trip2023data
  - trip_type
  - trip_zone

- Gold
  - trip_data
  - trip_type
  - trip_zone

## Project Structure

- data-factory/
- databricks/
- architecture/
- screenshots/
- README.md

## Screenshots

Project screenshots are available in the screenshots folder.

## Key Learning Outcomes

- Building data pipelines using Azure Data Factory.
- Working with Azure Data Lake Storage Gen2.
- Implementing Medallion Architecture.
- Transforming data using PySpark in Databricks.
- Managing cloud-based data engineering workflows.

## Author

Shamah Munemo

## Acknowledgements

NYC Taxi and Limousine Commission for providing public trip record data.
