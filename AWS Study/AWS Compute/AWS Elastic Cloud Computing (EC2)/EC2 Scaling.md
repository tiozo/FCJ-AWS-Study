### [[AWS EC2]] Scaling

Scaling is about using what use need.
In addition, have flexibility to grow freely. (most likely infinite if you have unlimited money too !)
Designing a scalable architecture allow you to pay for the resources that you need at any given time. (When you need **more/less** volume to be precise)

### [[AWS EC2]] Auto Scaling
Servers can get more request than they can handle.
Too many request = timeout and outage on that instance/node.
Too least request = wasted money but you might want this to happens on some cases.
AWS EC2 Auto scaling allows you to add or remove EC2 instances automatically. 
It automates the capacity to the demand.
There are 2 approaches:
- Dynamic scaling: Responds to changing demand.