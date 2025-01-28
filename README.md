# Weather Prediction Project
---
AWS and PySpark mllib introductory exploration project ingesting weather data from the OpenMeteo API that was migrated to Azure.
The purpose of this project was to create a Glue ETL pipeline to ingest historical weather data and forecasts for 25 worldwide cities from the 
OpenMeteo Weather API into an S3 bucket data lake while also processing and storing it in a medallion architecture utilizing parquet files.
After cleaning, analytical data was then brought to Athena to be stored in a Lake House architecture and utilized in a PowerBI dashboard visualization,
displaying generated weekly temperature forecasts as well as hourly real-time data and historical data. The forecasts were generated using a Linear Regression 
PySpark MLLib model trained on ingested historical weather data dating back to 2010.
The Jupyter notebooks stored here have been translated for usage in Azure Databricks but can be ran in an AWS Glue environment with minimal edits. 
