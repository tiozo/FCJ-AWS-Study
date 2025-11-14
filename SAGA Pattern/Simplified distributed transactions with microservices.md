[Original Links](https://temporal.io/blog/simplifying-distributed-transactions-microservices)

### Question for [[Distributed Systems]]

How to ensure reliability amid failures ?
How can you debug a problem that spans multiple services ?


### Orchestrating Microservices the Hard Way

- **Ephemeral State**: Process may end prematurely due to unexpected failures, leading to incomplete transactions or debugging nightmares.
- **Lack of Visibility**:  State is strewn across multiple services, making it difficult to understand progress and diagnose problems in the application.
- **Limited Reliability**: Service outages may cause interruptions, often requiring manual intervention and potentially leading to failures in other parts of the system.

### Conventional Approaches and Their Shortcomings

Teams has adopted various strategie