![image](https://github.com/user-attachments/assets/b5006368-aa91-4dcd-84b0-80bedce6577d)

![image](https://github.com/user-attachments/assets/9d2ea859-162b-45a4-9cec-f8442e19121a)

Business License Data Pipeline Using AWS
 1. Data Ingestion with S3
![image](https://github.com/user-attachments/assets/afd62055-0990-47d7-9828-59ae0cd07448)

Raw CSV files containing business license information are stored in Amazon S3 using a structured folder hierarchy. This serves as the entry point for the ETL pipeline and enables scalable, organized data tracking.
2. Metadata Discovery with AWS Glue Crawler
![image](https://github.com/user-attachments/assets/1f4b2ed5-8feb-48ca-b78d-425f4f2a88ca)
Glue Crawlers scan the dataset in S3, extract schema information, and register metadata into AWS Glue Data Catalog. This prepares the data for querying and downstream processing.
Glue Crawlers scan the dataset in S3, extract schema information, and register metadata into AWS Glue Data Catalog. This prepares the data for querying and downstream processing.
![image](https://github.com/user-attachments/assets/dae74e54-6db6-4cea-b260-a637cb5b94bf)
Using AWS Glue DataBrew, the dataset is profiled to detect schema mismatches, null values, and duplicates. This quality check ensures the data is ready for transformation.

4. Data Cleaning with Glue DataBrew Jobs
5. ![image](https://github.com/user-attachments/assets/2f8b363b-edbe-4372-85d5-38f12f60178e)

Data is cleaned using transformation recipes that handle missing values, correct data types, and standardize fields. The cleaned version is saved back to S3.
5. Data Cataloging with Glue Data Catalog
![image](https://github.com/user-attachments/assets/3ece0161-1173-42da-9f8b-9b362379ffc3)
Transformed and structured data is cataloged for use with Athena or Redshift. This step ensures easy access, schema management, and consistent querying.
6. Data Summarization with Glue ETL Jobs
![image](https://github.com/user-attachments/assets/61d89158-433a-4b52-8a7c-3a04f543aa8f)
WS Glue ETL jobs perform calculations like total permits, dominant business types, and seasonal trends. Summarized data is stored in S3 and ready for dashboards.

7. Data Security with KMS, S3 Versioning & Replication
8. ![image](https://github.com/user-attachments/assets/7780fa81-8aa0-4621-8f44-16c11dc01bc3)
Encryption (SSE-KMS), version control, and replication policies protect the dataset. Lifecycle rules automate cost-effective archiving to Glacier.
9. Monitoring with CloudTrail & CloudWatch
10.11. ![image](https://github.com/user-attachments/assets/5db11378-62e8-4a08-b76a-039d1320704f)
CloudTrail tracks user actions while CloudWatch monitors performance metrics. Alerts help detect anomalies and ensure operational transparency.

**Group Project**

Project Title:
Business License Data Analysis on AWS

Objective:
The goal is to design a detailed and sustainable data solution on AWS and organize the business license data for the City of Vancouver using S3, Glue, Athena, and QuickSight services. It will be able to process the data for ingestion, transformation, cleaning, and querying to generate insights that will help companies in making business decisions and policies.

Dataset:
The first data source is Business-Licenses.csv that includes license numbers, business names, date of the issue, date of expiration, business type, and location of the businesses. This data is available in an Amazon S3 bucket and is analyzed using AWS services for different analytical purposes.

Methodology:
Data Ingestion:

The dataset is stored in an Amazon S3 bucket for archiving, with folder taxonomy rules for the indexing of the bucket to enable simple retrieval. AWS Glue Crawlers help understand the dataset and create a catalog to make the data easily accessible for other AWS services.

Data Profiling:

DataBrew in AWS Glue is used for data preparation in which it helps in detecting the missing values, duplicate records, or wrong data types. Many functions in DataBrew mean that further cleansing and structuring of the dataset has been performed before proceeding to further analysis.

Data Transformation:

Thus, the AWS ETL jobs utilize the Glue functionality to perform the data transformation tasks like calculating business critical measures, dealing with the missing values and even formatting date columns. It is then written and stored back in S3 along with metadata for processing in analytical applications.

Data Querying and Reporting:

Users are then able to use Amazon Athena to query the cleaned and transformed data using SQL, for business trends, permit issuance, and market analysis. QuickSight is used to build real-time visuals for analysis of data so as to assist in the decision-making progress.


Data Security and Governance:

AWS KMS is used to encrypt the data at rest in order to protect the data storage in S3. Versioning is useful for maintaining multiple copies of data, replication, and lifecycle policies further help to enhance the durability and performance and also brings optimization of cost. CloudTrail is a service for monitoring of API activities while CloudWatch is used for monitoring the resource performance.

Data Monitoring and Optimization:

CloudWatch is used for monitoring of the system and CloudTrail helps in keeping logs for the operational utilization of the system. When there is a potential problem notifications are made through a buzzer.

Tools and Technologies:
Amazon S3 is used for storage of raw as well as processed data in a tabular form.

AWS Glue: This is another related product utilized in cataloging, transformation, as well as the conversion of the data into a format prepared for analysis.

Amazon Athena: Effective for analysis of files stored in S3 using SQL.

To enhance the current report generating methods, Amazon QuickSight is a tool used to make data analysis and reporting easy.

AWS KMS: KMS is used for encryption of data that is at rest.

AWS CloudTrail and AWS CloudWatch: For recording activities related to data and tracking its usage on the resources.

Deliverables:
S3 Bucket Structure: A managed structure of path that is used in storage and retrieval of business license data.

AWS Glue Data Catalog: Metadata of the dataset for efficient querying.

ETL Transformation Jobs: clear as well as changed information relating to the business license instruments.

Athena Queries: References to business trends, status of permits, and market conditions.

QuickSight Dashboards: This relates to business license graphics and analysis of trends.

Data security setting: KMS encrypt, version, replicate and enrol entity to utilize the most appropriate storage at lower cost and secure.

Supervision and Trace: CloudWatch and CloudTrail services to Log and Monitor various activities concerning the data into the cloud environment.
