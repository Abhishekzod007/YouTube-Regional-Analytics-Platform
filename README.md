# YouTube-Regional-Analytics-Platform

In this project, we developed a highly scalable and cloud-powered platform for analyzing YouTube data using a range of AWS services including S3, Glue, Athena, Lambda, and QuickSight. The system is designed to handle data from multiple regions such as the USA, Canada, Russia, and others, allowing seamless data integration, processing, classification, and reporting. With serverless technologies and automated workflows, the platform provides efficient data transformation and insightful analytics without the need for extensive infrastructure management.

---

## Project Objectives

**Data Ingestion**  
Develop a reliable system to ingest data from multiple sources efficiently.

**ETL Pipeline**  
Handle raw data, clean it, and transform it into a structured format ready for analysis.

**Data Lake Architecture**  
Store data from various sources in a centralized repository that ensures consistency and easy access.

**Scalability**  
Design the architecture so it can grow seamlessly as the volume of data increases.

**Cloud-based Processing**  
Leverage cloud infrastructure to process large datasets that cannot be handled effectively on local machines.

**Reporting and Insights**  
Build interactive dashboards that provide answers to key questions and support data-driven decision-making.

---

## AWS Services Used

**Amazon S3**  
A highly scalable object storage service that ensures data availability, security, and high performance.

**AWS IAM (Identity and Access Management)**  
Securely manage permissions and access controls for AWS resources and services.

**Amazon QuickSight**  
A serverless, cloud-powered business intelligence service that offers machine learning insights and interactive dashboards.

**AWS Glue**  
A serverless data integration tool that helps discover, clean, enrich, and combine data for analytics and machine learning tasks.

**AWS Lambda**  
A serverless compute service that runs code without the need to provision or manage servers.

**AWS Athena**  
An interactive query service that enables SQL-based querying directly on data stored in Amazon S3 without additional data loading.

---

## Dataset Details

We used the **YouTube trending videos dataset from Kaggle**, which includes detailed statistics for popular videos over several months. The dataset contains:

- Daily trending videos (up to 200 per region)
- Metadata such as video title, channel name, publication date, tags, view counts, likes/dislikes, comments, and descriptions
- Region-specific files, with JSON mappings for video categories (`category_id` differs by location)

**Dataset Source:**  
[https://www.kaggle.com/datasets/datasnaek/youtube-new](https://www.kaggle.com/datasets/datasnaek/youtube-new)

---

## Key Takeaways

✔ Built a cloud-native analytics platform for large-scale YouTube data  
✔ Enabled secure data access and processing using AWS IAM  
✔ Designed an ETL pipeline using visual tools to merge multiple datasets without writing any code, making data transformation easier and more efficient  
✔ Used AWS Lambda to automatically convert datasets from CSV to Parquet format without manually coding the logic — whenever new files are added or removed, the Lambda function triggers and updates the S3 buckets accordingly  
✔ Implemented scalable storage with Amazon S3 to store raw and processed datasets  
✔ Allowed real-time querying with AWS Athena, providing fast insights without loading data into databases  
✔ Created visually rich dashboards using QuickSight for exploring trends, patterns, and video performance  
✔ Ensured scalability and fault tolerance by leveraging serverless services like Lambda and Glue, reducing infrastructure management and improving reliability


## Architecture Diagram

Below is the architecture diagram for the YouTube Regional Analytics Platform:


<img width="829" height="463" alt="image" src="https://github.com/user-attachments/assets/06b78ddc-3d89-4715-a67d-c0eebe15a4c1" />

