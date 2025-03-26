![image](https://github.com/user-attachments/assets/b5006368-aa91-4dcd-84b0-80bedce6577d)

<img width="422" alt="image" src="https://github.com/user-attachments/assets/ffd49e68-011a-4cbf-a589-22729e210e21" />
Project Part 1
Descriptive Analysis
Project Description:
The Business License dataset has been cleaned, stored, secured, analyzed, and monitored using AWS services to achieve the Data Analysis Project (DAP). This structured approach helps to avoid problems connected with data quality, protection, as well as compliance and governance to support the decision-making process.

Project Title:
DAP Implementation: Business License Dataset
Objective:
To further analyse business licenses collected in their raw form and process them to constitute protection, efficiency, and supervision in order to support the analysis of the economy and business sectors.

Dataset:
It also has business license data of Vancouver that includes the business type, business location, details of the business unit occupied, and the business status.

Methodology:

Data Acquisition: Since business license data is acquired in large volumes, it is structured in a way that it can be stored in Amazon's S3 for easy tracking and retrieval. AWS Glue Crawlers scan the external data store and extract metadata, and store it in AWS Glue Data Catalog.

Data Profiling & Cleaning: Missing information, duplicate records, or a different data schema is detected and corrected by AWS Glue DataBrew. The directory with the cleaned data is located in S3.

Data Catalog: AWS Glue Data Catalog stores structured metadata information, enabling the entire dataset to be posted to be queried through Amazon Athena and Redshift.

AWS Glue ETL transforms records for business license intoa  structured format for data analysis among the companies.

Data cleansing: AWS Glue DataBrew prepares raw data that resides in amazon S3 in the format of Parquet and CSV. As mentioned earlier, while other query tools mostly allow the extraction of data for analysis, Amazon Athena is designed to copy data and give statistical information immediately in the process.
Data Security: Encryption through AWS KMS, S3 versioning, replication, and lifecycle are implemented to maintain data integrity, while S3’s multi-region storage optimizes its cost.

: Data Governance: AWS Glue ETL pipelines clean the data, validating records by removing any data that is not compliant with the standards that have been set.

Logging and Data Collection: The two important features of AWS cloud-based management and governance tools are AWS CloudTrail, for logging activities, security tracking, and managing data operations.

Tools and Technologies:

AWS Glue DataBrew, Amazon S3, Amazon Athena, AWS Glue Crawlers, AWS Glue ETL, AWS KMS, AWS CloudTrail, AWS CloudWatch, Amazon Redshift

Deliverables:

A set of integrated tables in the form of CSV files is available at Amazon S3-compatible storage for later analysis.

On the interactive dashboard and report, business trends.

Security measures ensuring data protection

Automated data validation pipelines

Comprehensive documentation and presentation for stakeholders


Project part 2

Descriptive Analysis	 

Project Description:	 
In the context of the Business License dataset, the DAP comprises of cleaning, storing, securing, monitoring and analyzing semi-structured business data in the AWS environment. These steps help in creating more structured data to guarantee reliable and secure information needed for making informed decisions.

Project Title:	 
DAP Implementation: Business License Dataset

Objective:	 
To utilize raw data coming from the business license data and elaborate it by applying efficiency in data processing, security solutions & monitoring for contributive economic and business sector analysis.

Dataset:	 
The business licenses provided refer to the Business Improvement Area licenses of Vancouver with attributes like the type of business, its address, unit, and current status.

Methodology:	 
1. Data Preprocessing: AWS Glue DataBrew processes raw data in the first stage, and the final data is stored in S3 with the help of Parquet and CSV formats. Statistical analysis can be carried out through querying with the help of Amazon Athena.
2. Data Security: Data security is also maintained using AWS KMS and S3 versioning and replication, and adding extra S3 lifecycle policies to optimize cost.
3. Data Governance: In AWS Glue ETL jobs, data validations and filter-out characteristics failing this validation are performed automatically.
4. Data Monitoring: Both AWS CloudTrail and CloudWatch are used for logging, tracking, and the chain of operation.

Tools and Technologies:	 
- AWS Glue DataBrew, Amazon S3, Amazon Athena, AWS KMS, AWS CloudTrail, AWS CloudWatch

Deliverables:	 
An analyzed data structure suitable for storage in AWS S3
Information that is presented in the form of dynamic and updated business reports and dashboards
Proper measures were taken to secure the data
Automated data validation pipelines
Comprehensive documentation and presentation for stakeholders

