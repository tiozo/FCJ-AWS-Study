### Cloud Notification Service - [[AWS SNS]]

AWS Simple Notification is also called **AWS SNS**
SNS (Simple Notification Service) is a notification service.

### What is AWS SNS?

SNS is a cloud service for the mass delivery of messages.
It is a fully managed publish-subscribe messaging and mobile communication service.
It can be event-driven, with automated services responding to triggers.
Distributed systems and micro services can be decoupled with messaging between them through AWS SNS.
Application-to-person messaging to users is possible with SMS, mobile push, and email.

### Message Endpoints

AWS SNS can publish messages to many different endpoints:
- HTTP and HTTPS
- Email and Email-JSON
- AWS SQS
- Applications
- AWS Lambda
- SMS (depending on region)

### The Difference between SQS and SNS

SNS is a notification system, which pushes messages to its subscribers.
SQS is a queuing system, and the receivers have to pull the messages to be processed and deleted from the queue.
SNS and SQS can works well together.