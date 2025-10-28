
### [[Subnets]]

Subnet is a section of VPC.
The subnet allows you to group resources.
The grouping can have different security or operations needs.
You can have both public and private subnet. (up to 200 subnet by default)

### [[Public Subnets]]

Public Subnets have resources that the public can access.

### [[Private Subnets]]

Private subnets have resources that can only accessed through the private network.

```
Public and Private Subnets can communicate with each other through secure channels.
```

### Network Traffic in a VPC

Requested data are sent as a **Packet**.
A Packet is a package of data sent over a network or the internet.
It enters the VPC through an Internet Gateway. (Public Internet Traffic)

Before entering a Subnet it checks for permissions.
Checking permissions such as:
1. Who sent the Packet?
2. How will the Packet communicate with the resources in the Subnet

