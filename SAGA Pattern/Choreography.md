
Decentralized communication. Each services listen for events and trigger subsequent steps by emitting new events. There's no central orchestrator; the flow emerges from interactions of individual services.

### Benefit
- **Decoupled services**: Each services operates independently
- **Scalability**: Event-driven system handle high loads efficiently.
- **Flexibility**: Adding new services doesn't require changing the workflow services.

#### Challenges
- **Debugging complexity**: Each services operate independent
- **Infrastructure setup**: Services require a robust message broker (Kafka, RabbitMQ) to connect all the dots.
- **Event Storms**: Poorly designed workflows can overwhelm the system with events.