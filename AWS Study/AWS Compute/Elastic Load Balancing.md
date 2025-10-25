Traffic can be directed with Elastic Load Balancing.

### Elastic Load Balancing Service
This service distributes application traffic across services.
The [[Load Balancer]] is a single point of contact for incoming web traffic.
The single point of contact means that the traffic hits the [[Load Balancer]] first, spreading out the load between resources.
The balancer accepts requests and directs them to the stances.

It ensures that one resource won't get overloaded, and that the traffic is get out.
[[AWS EC2]] and [[Elastic Load Balancing]] are two different services that work well together.

> [!Info]
> ELB is built to support traffic without increasing hourly cost.
> ELB scales automatically.

### Load Allocation
