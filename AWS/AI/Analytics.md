## Athena
- Lets you query the files stored directly in S3 buckets using ANSI SQL or python.
- Serverless. Only pay for queries run.
- Services,
	- Athena SQL
	- Apache Spark
[What is Amazon Athena?](https://docs.aws.amazon.com/athena/latest/ug/what-is.html)
[FAQ](https://aws.amazon.com/athena/faqs/?nc=sn&loc=6)

## Data Exchange
- Helps manage entitlements, grants and subscriptions of the data consumed from other org data or from AWS Marketplace.
**Data grant:** Permission/Grant created by sender to give access to data sets.
- **Data set:** Single unit of data that the provider publishes. Receiver gains access once the sender accepts the data grant. Supported data set types: Files, S3, API, Redshift, Lake formation (preview).
- **Data grant details:** Meta data of grant.
- **Recipient access details:** Receiver account ID and validity of grant.
**Data product:** Product published in AWS Marketplace.

Data sender can use,
- **AWS Data Exchange API** - To CRUD the data sets.
- **AWS Marketplace Catalog API** - To view and update data products.

## Data Pipeline
A service to automate the movement and transformation of data. **Maintenance mode.**
- Pipeline definition - Definition of logic and transformations.
- Pipeline - Schedules and runs tasks by creating EC2 instances.
- Task runner - Continuously polls and runs tasks. Waits for the previous tasks to get completed.

## EMR - Elastic MapReduce
Helps run and scale open source big data frameworks like
- Apache Hadoop
- Apache Spark
- Hive
- Presto
Can run on EC2, EKS, AWS Outposts or EMR Serverless.
Can be interacted through
- EMR Console
- EMR Studio
- EMR Notebooks

## Glue
Consolidates major data integration capabilities into single service. Include data discovery, modern ETL, ELT, cleansing, transforming, streaming and centralized cataloging in one service. Integrates with analytics services and Amazon S3 data lakes. 
Serverless.
### Glue data catalog 
Glue data crawler crawls on multiple data sources and writes the table metadata in Glue data catalog.
Amazon Athena, Amazon EMR, and Amazon Redshift Spectrum internally leverage the glue data catalog to do data discovery.
![[Pasted image 20240716202557.png]]

## Kinesis
Real time data collection and analysis service.

Amazon Kinesis Data Analytics for SQL Applications - [Deprecated]. Managed service for Apache flink is recommended instead.

Kinesis Data Streams
Kinesis Data Firehose
Kinesis Data Analytics
Kinesis Managed Streaming for Apache Kafka

## AWS Lake Formation
Central place to have all the data for analysis. Fully managed service. 
Fine grained access control capabilities - row level, column level and cell level. Adds on top of IAM permissions.
Built on top of Glue. 
Data is store in S3.
https://docs.aws.amazon.com/lake-formation/latest/dg/what-is-lake-formation.html

## Amazon Managed Streaming for Apache Kafka (Amazon MSK)
Kafka on AWS. Fully managed or serverless.
Consumers of MSK could be, 
- Kinesis data analytics
- AWS Glue - Streaming ETL jobs powered by Apache Spark streaming
- Lambda
- Custom consumers / applications

## Amazon OpenSearch Service
Lets you run the 'OpenSearch' in AWS.
1. Provisioned - still a managed service, automatically detecting and replacing failed nodes.
2. Serverless - Fully managed with auto scaling. Encrypted mode only but user can choose the key.
3. Provision and run the OpenSearch manually if you have a unique use case with the engine.
OpenSearch is an open source, distributed search and analytics engine. It can do the below functions using the log data
- Scalable fast and full text search
- App and infra monitoring
- Security events and alerting
- Health tracking
https://docs.aws.amazon.com/opensearch-service/latest/developerguide/what-is.html

## Amazon QuickSight
Cloud based business intelligence tool. Fully managed service. It can ingest data from various sources including AWS, on premise, spreadsheets and other data providers. It can analyse the data and present it in the desired format. It also has ML capabilities. Can be presented to various consumers in different modes including mobile, email or embedded in website.
https://docs.aws.amazon.com/quicksight/latest/user/welcome.html

## Amazon Redshift
- Its a data warehouse service which can store and handle data of the scale of peta bytes.
- Comes in serverless and provisioned mode.
- Leader Node controls the compute nodes to run the queries in parallel and returns back to the client. Leader node and computer nodes form the cluster.
- Redshift spectrum can help query the S3 directly without having to load the data into Redshift, if Redshift cluster is already provisioned and sql client is connected to the cluster.
https://docs.aws.amazon.com/redshift/