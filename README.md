# Home Sales Analysis Project

## Overview
This project analyzes home sales data using PySpark SQL functions. Various queries provide insights, with optimizations like caching and partitioning for performance enhancement.

## Project Files and Process
- **Home_Sales.ipynb**: Jupyter Notebook containing PySpark code for analysis.

## Data Acquisition
- **Read Data from AWS S3 Bucket**: The home sales data is retrieved from an AWS S3 bucket.
- The `home_sales_revised.csv` is then added to Spark and read into a Spark DataFrame for further analysis.

## Analysis
Utilizing SparkSQL to answer key questions:
- Average price for a four-bedroom house sold annually.
- Average price of a three-bedroom, three-bathroom home each year.
- Average price of homes meeting specific criteria.
- Average price per "view" rating for homes >= $350,000, with runtime comparison.

## Optimization, Performance Evaluation, and Memory Management
- **Table Caching**: `home_sales` table cached for performance.
- **Partitioning**: Data partitioned by `date_built` for faster querying.
- **Cached Query Execution**: Runtime comparison of cached and uncached queries.
- **Parquet Query Execution**: Runtime comparison on parquet data.
- **Table Uncaching**: Uncaching for memory management.

## Summary
This project showcases PySpark's efficiency in analyzing large datasets. Through SparkSQL functions and optimizations like caching and partitioning, valuable insights are derived from home sales data.
