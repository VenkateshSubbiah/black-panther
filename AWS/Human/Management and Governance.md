## AWS Auto Scaling

## AWS CloudFormation
Lets you create templates of the AWS services with its dependencies so that they can be provisioned, managed, replicated and version controlled. The cloud formation templates are stored as text files so that they can be easily tracked.
## AWS CloudTrail
A governance, compliance and audit for the account.
### Types
**Management events:** Add, delete, modify resources or IAM roles.
**Data events:** Events happening inside a resource. Eg. PutItem in S3.
**Insight events:** Detects unusual activities.
### Ways to record
-  *Event history* provides a viewable, searchable, downloadable, and immutable record of the past 90 days of **management events** in an AWS Region.
- *CloudTrail Lake* is a managed data lake for capturing, storing, accessing, and analyzing **user and API activity** on AWS for audit and security purposes.
- _Trails_ capture a record of AWS activities, delivering and storing these events in an Amazon S3 bucket, with optional delivery to [CloudWatch Logs](https://docs.aws.amazon.com/awscloudtrail/latest/userguide/send-cloudtrail-events-to-cloudwatch-logs.html) and [Amazon EventBridge](https://docs.aws.amazon.com/awscloudtrail/latest/userguide/cloudtrail-aws-service-specific-topics.html#cloudtrail-aws-service-specific-topics-eventbridge).
## Amazon CloudWatch
Gathers logs from all the AWS services.
- Metrics
- Log groups
- Live tail
- CloudWatch logs agent and Unified agent
- CloudWatch Events is now EventBridge
## AWS Command Line Interface (AWS CLI)

## AWS Compute Optimizer

## AWS Config
Records and audits the compliance and configuration changes in the AWS account. For compliance, rules can be setup.
## AWS Control Tower
Helps setup and govern multi-account AWS environments on AWS organizations. Controls (Guardrails) can be configured to the resources created within the AWS accounts managed by control tower. Also the default configuration can be defined while creating new AWS accounts.
## AWS Health Dashboard
Lists down the health of the AWS services. Publicly accessible. If you sign in, you get results that affect your account.
## AWS License Manager
Helps manager licenses (Microsoft, SAP, Oracle etc) in a single place.
## Amazon Managed Grafana
Amazon Managed Grafana is a fully managed and secure data visualization service that you can use to instantly query, correlate, and visualize operational metrics, logs, and traces from multiple sources.
## Amazon Managed Service for Prometheus
Amazon Managed Service for Prometheus is a serverless, Prometheus-compatible monitoring service for container metrics that makes it easier to securely monitor container environments at scale.
## AWS Management Console

## AWS Organizations

## AWS Proton
Automated infrastructure as code provisioning and deployment of serverless and container-based applications.
## AWS Service Catalog

## AWS Systems Manager

## AWS Trusted Advisor

## AWS Well-Architected Tool