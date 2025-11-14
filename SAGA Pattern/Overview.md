[Original Series On SAGA Pattern](https://dev.to/federico_bevione/transactions-in-microservices-part-1-saga-patterns-with-choreography-and-orchestration-4an9)

### Distributed system

A system that are not placed within a single machine, could be different Server racks with on-premises, cloud or hybrid.
Provide a strong availability for each services within a microservices system.

Yet, this face an issue with consistency long for all the services that's are running on different spectrum of a system. A traditional database would fall short at this case. So Distributed Transaction step in.

### Distributed Transaction

This allow system to coordinate multiple services while handling failures gracefully. 
One of the approach called SAGA pattern, provide **Choreography** & **Orchestration**.

### Challenge of Distributed Transactions

1. **Partial Failure**: One service may fail when other succeed, leaving the system in inconsistent state.
2. **Data Consistency**: The final state must reflect the intended outcome, regardless of the individual failures.
3. **Complex workflows**: Coordinating multiple services in reliable and maintainable way.

### SAGA Pattern

Breaks a complex workflow into multi-step workflow, each step in the workflow is independent, perform on a specific that can be compensated (undone) if something goes wrong.

#### Approaches
