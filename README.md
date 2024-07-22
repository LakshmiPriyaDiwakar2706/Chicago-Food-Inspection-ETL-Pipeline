# Chicago Food Inspections ETL Pipeline

## Project Overview

This project demonstrates the creation of an ETL (Extract, Transform, Load) pipeline to fetch real-time food inspections data from the Chicago Data Portal. The pipeline processes the data by dropping unnecessary columns and then loads it into an Amazon S3 bucket using Apache Airflow. The infrastructure includes an EC2 instance and an S3 bucket, both set up on AWS.

## Project Steps

1. **Extract**: Fetch real-time food inspections data using the Chicago Data Portal API.
2. **Transform**: Clean the data by dropping unnecessary columns.
3. **Load**: Store the processed data in an S3 bucket using Apache Airflow.

## Architecture

The architecture of the ETL pipeline includes:
- **AWS EC2 Instance**: Used to host the Airflow instance.
- **AWS S3 Bucket**: Used for storing the processed data.

## Setup and Execution

### Prerequisites

- AWS account with permissions to create EC2 instances and S3 buckets.
- Python installed on your local machine.
- Apache Airflow installed.

### Steps

1. **Create an EC2 Instance**:
   - Launch an EC2 instance on AWS.
   - Install necessary dependencies (Python, Airflow, AWS CLI) on the instance.

2. **Set Up S3 Bucket**:
   - Create an S3 bucket on AWS to store the processed data.

3. **Configure Apache Airflow**:
   - Install Apache Airflow on the EC2 instance.
   - Set up Airflow to use the S3 bucket as a storage location.

4. **Develop the ETL Pipeline**:
   - Write a Python script to fetch data from the Chicago Data Portal API.
   - Transform the data by dropping unnecessary columns.
   - Load the transformed data into the S3 bucket using an Airflow DAG (Directed Acyclic Graph).

## Results
- DAG Run Status
The DAG runs successfully as shown in the screenshot below:
 [DAG Job run status](https://github.com/LakshmiPriyaDiwakar2706/Chicago-Food-Inspection-ETL-Pipeline/blob/main/DAG.png)


- S3 Bucket Contents
The processed data is successfully loaded into the S3 bucket:
  [S3 bucket Content](https://github.com/LakshmiPriyaDiwakar2706/Chicago-Food-Inspection-ETL-Pipeline/blob/main/S3%20Bucket.png)

