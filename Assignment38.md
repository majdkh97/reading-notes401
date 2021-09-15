# Read38

## What is Amazon SNS?

**Amazon Simple Notification Service (Amazon SNS) is a fully managed messaging service for both application-to-application (A2A) and application-to-person (A2P) communication. The A2A pub/sub functionality provides topics for high-throughput, push-based, many-to-many messaging between distributed systems, microservices, and event-driven serverless applications. Using Amazon SNS topics, your publisher systems can fanout messages to a large number of subscriber systems including Amazon SQS queues, AWS Lambda functions and HTTPS endpoints, for parallel processing, and Amazon Kinesis Data Firehose. The A2P functionality enables you to send messages to users at scale via SMS, mobile push, and email.**

## Amazon SNS features

- Application-to-application messaging -> Application-to-application messaging supports subscribers such as Amazon Kinesis Data Firehose delivery streams, Lambda functions, Amazon SQS queues, HTTP/S endpoints, and AWS Event Fork Pipelines. For more information, see Using Amazon SNS for application-to-application (A2A) messaging.

- Application-to-person notifications -> Application-to-person notifications provide user notifications to subscribers such as mobile applications, mobile phone numbers, and email addresses. For more information, see Using Amazon SNS for application-to-person (A2P) messaging.

- Standard and FIFO topics -> Use a FIFO topic to ensure strict message ordering, to define message groups, and to prevent message duplication. Only Amazon SQS FIFO queues can subscribe to a FIFO topic. For more information, see Message ordering and deduplication (FIFO topics).
Use a standard topic when message delivery order and possible message duplication are not critical. All of the supported delivery protocols can subscribe to a standard topic.

- Message durability -> Amazon SNS uses a number of strategies that work together to provide message durability:

1. Published messages are stored across multiple, geographically separated servers and data centers.

2. If a subscribed endpoint isn't available, Amazon SNS runs a delivery retry policy.

3. To preserve any messages that aren't delivered before the delivery retry policy ends, you can create a dead-letter queue.

- Message archiving and analytics -> You can subscribe Kinesis Data Firehose delivery streams to SNS topics, which allow you to send notifications to additional archiving and analytics endpoints such as Amazon Simple Storage Service (Amazon S3) buckets, Amazon Redshift tables, and more.

- Message attributes -> Message attributes let you provide any arbitrary metadata about the message. Amazon SNS message attributes.

- Message filtering -> By default, each subscriber receives every message published to the topic. To receive a subset of the messages, a subscriber must assign a filter policy to the topic subscription. When the incoming message attributes match the filter policy attributes, the message is delivered to the subscribed endpoint. Otherwise, the message is filtered out. For more information, see Amazon SNS message filtering.

- Message security -> Server-side encryption protects the contents of messages that are stored in Amazon SNS topics, using encryption keys provided by AWS KMS. For more information, see Encryption at rest.
You can also establish a private connection between Amazon SNS and your virtual private cloud (VPC). for more information, see Internetwork traffic privacy.
