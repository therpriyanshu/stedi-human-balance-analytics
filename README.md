# STEDI Human Balance Analytics

## Project Overview

This project implements a data lake solution for the STEDI Human Balance Analytics application using AWS services. The pipeline processes raw sensor and customer data through Landing, Trusted, and Curated layers to prepare high-quality datasets for machine learning.

## Technologies Used

- AWS S3
- AWS Athena
- AWS Glue
- AWS Glue Data Catalog
- SQL
- PySpark

## Project Workflow

1. Upload raw JSON data to Amazon S3.
2. Create external tables in Athena.
3. Build AWS Glue ETL jobs to transform the data.
4. Store processed data in Trusted and Curated layers.
5. Validate the output using Athena queries.

## Data Pipeline

- Landing → Raw customer, accelerometer, and step trainer data
- Trusted → Filtered and validated records
- Curated → Clean datasets prepared for analytics and machine learning

## Project Structure

```
sql/
dataset/
screenshots/
README.md
```

## Outcome

The pipeline successfully transforms raw data into curated datasets that can be used for analytics while ensuring customer consent requirements are respected.
