
### AWS Cloud Different Databases Types

AWS offers more types of databases.
It is good to be aware of them, should you need to use them.

### [[AWS DocumentDB]]

Is a document-based database service.
It is a type of NoSQL database.
Support MongoDB.
Ideal for content management systems, user profiling, cataloging.

```json
{  
 name: "Jason",  
 age: "29",  
 city: "New York"  
 profession: "Accountant"  
}
```

### [[AWS Neptune]]

Is a graph database service.
Can be used to create graph from your data for various purposes.
It is great for financial records, supply chain systems, and other centralized digital records.
![[Pasted image 20251028135317.png]]
### [[AWS QLDB]] (AWS Quantum Ledger Database)

Is a ledger database service.
Provides historical data of all your application changes.
Great for financial records, supply chain systems, and other centralized digital records.
![[Pasted image 20251028135507.png]]

### [[AWS Managed Blockchain]]

AWS Managed Blockchain is a service that utilizes open-source frameworks to create or mange blockchain networks.
With a few clicks, you can join, create, and manage blockchain networks.
**Ethereum** and **Hyberledger Fabric** are popular open-source blockchain technologies.
![[Pasted image 20251028135827.png]]

### [[AWS ElastiCache]]

adds catching layers on top of a database.
Catching layer stores a part of data.
Accelerates application performance.
Improves the read times of databases requests.
Redis and MemCached are supported with AWS ElastiCache service.
![[Pasted image 20251028140250.png]]

### [[AWS DynamoDB Accelerator]] (DAX)

It is an in-memory cache service for AWS DynamoDB.
It improves read times for your non-relational data.
It improves response times from ms to mcros.
Is a fully managed, flexible and secure service.
![[Pasted image 20251028140601.png]]

### 