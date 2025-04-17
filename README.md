# ETL-Data-Pipeline-On-Google-Cloud
### Problem Statement
#### The objective of this project is to design and implement a robust ETL (Extract, Transform, Load) data pipeline on Google Cloud Platform. The pipeline will extract employee data from multiple sources, apply secure data masking to protect sensitive information, and load the processed data into BigQuery for storage and analysis. 

### Requirements
#### 1. Data Extraction: Extract Employee data from multiple data sources such as databases, CSV files, or APIs
#### 2. Data Masking: Identify sensitive information within the employee data, such as social security numbers, salary details, and personal contact information
#### 3. Data Loading into BigQuery: Design a process to securely load and extract the data and mask employee data into BigQuery by using Dataflow or Python custom coding, or Airflow



### Tech Stack
1. Python: For data extraction from source systems.
2. Cloud Storage: For storing raw and interim data.
3. Cloud Data Fusion - for transformation of data with no-code solution
4. BigQuery: For data storage and querying.

### Architecture
1. Extraction: Python scripts extract data from sources and store it in Cloud Storage (raw bucket).
2. Transformation: Cloud Data Fusion processes raw data, masks sensitive information, and writes transformed data to Cloud Storage (transformed bucket) or BigQuery.
3. Loading: Transformed data is ingested into BigQuery for storage and analysis.
