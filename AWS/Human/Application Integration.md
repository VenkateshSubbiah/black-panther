## Amazon AppFlow
Enables to securely exchange data between SAAS products (Salesforce, Zendesk) and AWS services (S3, Redshift, etc).
## AWS AppSync
Enables developers connect apps and services to data and events from serverless GraphQl and Pub/Sub APIs.
## Amazon EventBridge
Helps connect AWS services, SAAS and applications through events. Thereby making the components loosely coupled.
**Buses:** Multiple source to multiple targets.
**Pipes:** Single source to single target. Has advanced transformation capabilities before delivering the events.
## Amazon MQ
Managed message broker service. Supports Apache ActiveMQ and RabbitMQ. Message broker allows apps, components to communicate using various programming languages, OS and formal messaging protocols.
Old apps that uses message brokers can be migrated to Amazon MQ. New apps can use SQS or SNS.
## Amazon Simple Notification Service (Amazon SNS)
Message delivery service in publisher-subscriber pattern. Topics can be created in SNS and the subscribers can subscribe to the topics.
### Features
- Subscriber types
	- Application to application - SQS, Lambda, Kinesis firehose, HTTP endpoints.
	- Application to person - SMS, Mail, Mobile push notifications.
- Topic types
	- Standard - No ordering or deduplication of messages. All types of subscribers can subscribe.
	- FIFO Topic - Ensures strict ordering to define message groups and for deduplication. Only SQS FIFO queues can subscribe to this topic.
- Message filtering - Subscribers can get selective messages only based on filters.
### Fanout pattern
When messages needs to be sent to multiple SQS queues from an application, its better to send to SNS first and then the SQS queues can subscribe to the SNS topic. This way the SQS is decoupled from the app and can add any number of SQS queues in future. Also there is possibility the app crashes while it sent the messages to only some of the SQS queues.
![[Pasted image 20240811191341.png]]
## Amazon Simple Queue Service (Amazon SQS)
Queue service for decoupling. Mostly used for single consumer.
- Message visibility timeout
- Long polling
- FIFO queues
## AWS Step Functions
With step functions, one can create workflows (state machine) to,
- Build distributed applications
- Orchestrate microservices
- Create pipelines
Can visualize workflows. Integrates with AWS services like lambda, glue and EC2. The state machine is called workflow and each step in workflow is called step.
### Features
![[Pasted image 20240812044534.png]]
### Types of service integration
 - Standard
	 - Long-running, auditable workflows that show execution history and visualized.
	 - Steps are executed exactly once.
	 - Can run upto 1 year.
 - Express
	 - High-event-rate workflows. Eg. Streaming data processing and IOT data ingestion .
	 - Steps are executed at least once.
	 - Can run upto 5 minutes.
## Others
- [Differences between Amazon SQS, Amazon MQ, and Amazon SNS](https://docs.aws.amazon.com/AWSSimpleQueueService/latest/SQSDeveloperGuide/welcome.html#sqs-difference-from-amazon-mq-sns)