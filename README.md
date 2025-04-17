# ETL-Data-Pipeline-On-Google-Cloud
### Problem Statement
#### The objective of this project is to design and implement a robust ETL (Extract, Transform, Load) data pipeline on Google Cloud Platform. The pipeline will extract employee data from multiple sources, apply secure data masking to protect sensitive information, and load the processed data into BigQuery for storage and analysis. Furthermore, the project includes the development of a secure, user-friendly dashboard to visualize the employee data, ensuring compliance with data privacy and security standards

### Requirements
#### 1. Data Extraction: Extract Employee data from multiple data sources such as databases, CSV files, or APIs
#### 2. Data Masking: Identify sensitive information within the employee data, such as social security numbers, salary details, and personal contact information
#### 3. Data Loading into BigQuery: Design a process to securely load and extract the data and mask employee data into BigQuery by using Dataflow or Python custom coding, or Airflow
#### 4. Dashboard visualization: Develop a web-based dashboard using appropriate visualization tools. (e.g., Google Data Studio, Tableau, or any custom dashboard)


### Tech Stack
1. Python: For data extraction from source systems.
2. Cloud Storage: For storing raw and interim data.
3. Cloud Data Fusion - for transformation of data with no-code solution
4. BigQuery: For data storage and querying.
5. Looker Studio: For creating interactive visualizations.
6. Cloud Composer (Airflow): For workflow orchestration.

### Architecture
![image](https://github.com/user-attachments/assets/85973415-804f-44da-bb86-630a8b457f19)
1. Extraction: Python scripts extract data from sources and store it in Cloud Storage (raw bucket).
2. Transformation: Cloud Data Fusion processes raw data, masks sensitive information, and writes transformed data to Cloud Storage (transformed bucket) or BigQuery.
3. Loading: Transformed data is ingested into BigQuery for storage and analysis.
4. Visualization: Looker Studio queries BigQuery to generate dashboards.
5. Orchestration: Cloud Composer schedules and monitors the entire workflow.
