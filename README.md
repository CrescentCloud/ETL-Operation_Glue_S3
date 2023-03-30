# ETL-Operation_Glue_S3_Athena_AWS QuickSight
### Overview:
Perform an ETL operation on CSV Data using AWS Glue residing on S3 Bucket, run crawler and create a glue catalog for querying using Athena and finally create visualization using Quicksight  

![glue drawioc](https://user-images.githubusercontent.com/53235392/228801786-5850a30a-dcd5-4fff-a242-c5ef8815310f.png)

## Task Details
Sign in to AWS Management Console

01. Upload CSV file to a Bucket on S3

02. Create a Glue crawler

03. Create IAM role to be used by crawler

04. Create a Glue Job

05. Run the crawler, to create a table

06. Use Athena to query the tables or to create views out of tables.

07. Use Athena Tables to create visualization using QuickSight

### Glue:
Glue is a fully managed extract, transform and load service that makes it simple and cost effective to categorize data.

And glue is completely serverless. You don't have to manage any infrastructure yourself. 

Glue has five components : 

→ First one is Central metadata repository, which is known as AWS Glue Data Catalog. 

→ Second is Glue Crawlers that scans data and populate the data catalog.

→ Third one is ETL Engine that automatically Generates Python or scala code for all of your transformations or the data enrichment process.

→ The fourth one is the Glue Triggers. Which acts as scheduler for all your jobs. You can trigger any crawler or job on completion of another job.

→ The last one is Glue Workflows by which you can orchestrate the different steps of your ETL jobs meta Glue Crawlers.

Crawler is responsible for scan data. Data could be in S3 or DynamoDB or any relational DB. And after scanning the data, it creates a metadata tables in Central Glue data Catalog.<br>
The table that is created in the data catalog can be used by other AWS services such as Athena, Redshift, Spectrum and ETL Jobs. 

### Three major use case of Athena

→ Analyze unstructured, semi-structured, and structured data stored in Amazon S3. Examples include CSV, JSON, or columnar data formats such as Apache Parquet and Apache ORC. 

→ Athena integrates with Amazon QuickSight for easy data visualization. You can use Athena to generate reports or to explore data with business intelligence. 

→ Athena integrates with the AWS Glue Data Catalog, which offers a persistent metadata store for your data in Amazon S3. 

### AWS QuickSight

Amazon QuickSight is a fully managed , fast, cloud-powered business intelligence service. It lets you easily create and publish interactive dashboards that include machine learning (ML) insights and delivers to everyone in your organization


## Steps to Follow
1.	Create a bucket to S3 and upload CSV data to the bucket
3.	Create IAM role to be used by crawler
5.	Create a glue crawler by AWS glue service	
7.	Crawler will go and extract the data from the S3 bucket and create table in Glue Data Catalogue. These tables access by Athena from where we can run the Athena query
9.	Create another folder to S3 where Athena will keep save the query
10.	Run a few queries to test Athena is successfully able to query the database 	
11.	Load Data from Athena to Qucksight to Create Visualization
12.	QuckSight will help create diffrent types Visualization as per own Choice  



