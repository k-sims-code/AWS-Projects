# Event Announcement System
 
This project is a data pipeline for processing csv files using services like S3, AWS Lamba, AWS Glue and Amazon Quicksight.

# Overview:
This project involves building a serverless data pipeline on AWS for processing csv files. The pipeline automates the ingestion, transformation, and visualization data. Csv files are uploaded to a raw data S3 bucket (csv-in-raw-form), triggering an AWS Lambda function to pre-process the data and store in the processed data bucket, (csv-in-processed-form). AWS Glue is then used for further ETL (Extract, Transform, Load) operation, and the final data is stores in the final data bucket, (csv-in-final-form). Finally, Amazon Quicksight is used to create interactives dashboards and reports for visualizing the final form.

# Data Ingestion:
Csv files are uploaded to an Amazon S3 bucket, which serves as the central storage for raw and processed data.

# Trigger and Transformation: 
An AWS Lambda function is automatically triggered to preprocess the data, such as filtering or formatting, and pass it to AWS Glue for detailed ETL operations.

# Data Storage:
Processed data is stored in S3 for scalable storage. 

# Visualization: 
Amazon Quicksight connects to the data source to create dynamic and interactive dashboards for visualization and reporting. 

# Services Used:  

# 1. Amazon S3 (Storage):
used for scalable storage of raw and processed data, providing event-driven architecture capabilities withS3 event notificions.

# 2. AWS Lambda (Compute):
Act as a serverless compute layer, automatically triggered to pre-process and clean csv filed upon upload to S3.

# 3. AWS Glue (ETL/Big Data):
Provides ETL capabilities to extract, transform, and load data into a usable format for analysis.

# 4. Amazon Quicksight (Analytics):
Offers interactive dasboards and reports for real-time data visualization.

# 5. IAM Roles and Policies (Permissions):
Ensures secure access to S3, Lambda, Glue, and Quicksight.
