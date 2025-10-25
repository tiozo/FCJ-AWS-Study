### Monolithic Applications and Microservices
Applications are made of multiple components.
The components communicate with each other.
The communication can transmit data, fulfill requests, and keep the application running.

### Monolithic Application
An architecture with tightly coupled components can be called a monolithic application.
Components can be databases, servers, interfaces, and much more.
A monolithic application can be vulnerable if one of the components fails.
In the worst case this can cause the whole service to go down.

> [!Info]
> Instead of monolithic, your application can be designed with an approach called microservices.
> Microservices can help to keep your service available if one c