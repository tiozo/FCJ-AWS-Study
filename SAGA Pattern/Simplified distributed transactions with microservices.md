[Original Links](https://temporal.io/blog/simplifying-distributed-transactions-microservices)

### Question for [[Distributed Systems]]

How to ensure reliability amid failures ?
How can you debug a problem that spans multiple services ?


### Orchestrating Microservices the Hard Way

- **Ephemeral State**: Process may end prematurely due to unexpected failures, leading to incomplete transactions or debugging nightmares.
- **Lack of Visibility**:  State is strewn across multiple services, making it difficult to understand progress and diagnose problems in the application.
- **Limited Reliability**: Service outages may cause interruptions, often requiring manual intervention and potentially leading to failures in other parts of the system.

### Conventional Approaches and Their Shortcomings

Teams has adopted various strategies to address these problems. 
- **Stateful Service**: Each service maintains it own database to track state. While this ensures data isn't lost, it introduces multiple state machines that must be managed and synchronized, adding complexity to the system.
- Event Stores or Messaging Systems: Tools such as Kafka can provide protection against service outages by decoupling the service that produces a message from the service that consumes it. However, further reduce lack of visibility in the overall system, especially after adding dead letter queues to deal with failures.

### Orchestrating Microservices the Durable Way

Temporal access this problem via Workflow.
(A set of predefined business logic using a standard programming language.)

- **Eliminate **Ephemeral****: Temporal workflow's automatically
- **Gain visibility into Execution*Temporal's Event history record ;
