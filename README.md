# 🎵 Spotify Analysis Project 📊

## 🌟 Project Overview
This project demonstrates how to analyze Spotify data using various AWS services. The data pipeline includes ingestion, transformation, and visualization using AWS Glue, S3, Athena, and QuickSight. The dataset was sourced from Kaggle and showcases the application of these AWS tools for data ETL (Extract, Transform, Load) and business intelligence.

## 🛠 Project Architecture
1. **S3 Staging Area**: 
   - 📁 Data is initially stored in a staging area on S3.
   
2. **AWS Glue**: 
   - 🔄 Used for ETL jobs to extract data from S3 and load it into the Data Warehouse (DW).
   
3. **S3 Data Warehouse**:
   - 🏢 Stores the transformed data.
   
4. **AWS Glue Crawler**:
   - 🧹 Creates metadata and tables from the data in the Data Warehouse.
   
5. **AWS Athena**:
   - 🔍 Performs SQL queries on the tables created by the Glue Crawler.
   
6. **AWS QuickSight**:
   - 📈 Provides visualization and business insights based on the queried data.

## 🔄 Workflow

1. **Dataset Acquisition**:
   - 📥 Downloaded a dataset from Kaggle for analysis.

2. **IAM User Creation**:
   - 👤 Created an IAM user to manage permissions and understand its role in securing access to AWS resources.

3. **S3 Bucket Setup**:
   - 🗂 Created an S3 bucket with folders for staging and the data warehouse.

4. **Data Ingestion**:
   - 🏗 Data was manually uploaded to the staging area. In a real-world scenario, data would come from databases or DynamoDB.

5. **Data Transformation**:
   - 🔧 Used AWS Glue Studio to visually create an ETL pipeline.
   - 📊 Joined multiple tables, removed unnecessary columns, and stored the resulting table in the S3 Data Warehouse.
   - 📝 Pipeline script can be viewed by clicking the "Script" button.

6. **IAM Role Creation**:
   - 🛡 Created an IAM role with permissions to allow AWS Glue to access S3 buckets.

7. **ETL Job Execution**:
   - ✅ Successfully ran the ETL job in AWS Glue. Data was transformed and stored in the destination bucket.

8. **Glue Crawler Setup**:
   - 📂 Created a crawler to catalog the data in the S3 Data Warehouse.
   - 🛠 Resolved IAM role permission issues and created tables in the Glue Data Catalog.

9. **Athena Querying**:
   - 🖥 Set up AWS Athena's query editor.
   - 🔍 Performed SQL queries to analyze and extract insights from the data.

10. **QuickSight Visualization**:
    - 📊 Configured AWS QuickSight for data visualization.
    - 📈 Created dashboards and visualizations to gain business insights.

## 🛠 Troubleshooting

- **Permission Issues**:
  - 🔒 Encountered and resolved IAM role permission issues for AWS Glue and the Glue Crawler.
  - ✔ Ensured appropriate policies were attached to allow necessary actions.

## 🚀 Conclusion
This project showcases an end-to-end process of data ingestion, transformation, and visualization using AWS services. The integration of AWS Glue for ETL, Athena for querying, and QuickSight for visualization provides a powerful solution for data analysis and insights.


