
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

There are other way to access VPC, mentioned a few in [[AWS Cloud Connectivity]]
**From Other AWS VPCs**
This is for connecting your VPC to _other_ VPCs, either in your own AWS account or in a different account.
- **VPC Peering:** This is a direct, 1-to-1 network connection between two VPCs. It makes them behave as if they are on the same private network.
- **AWS Transit Gateway (TGW):** This acts as a central "hub" or cloud router. Instead of creating many individual VPC Peering connections, you connect all your VPCs (and your on-premises VPN/DX connections) to a single Transit Gateway. It's the modern way to manage connectivity for complex, large-scale networks.
**From Other AWS Services (Privately)**
This is a very common and important one. Imagine your application in the VPC needs to get a file from S3.
- **Without an endpoint:** The packet would have to go _out_ your VPC (through a NAT Gateway, which uses the Internet Gateway) to the _public_ S3 endpoint, and then back.
- **With an endpoint:** You use **VPC Endpoints (powered by AWS PrivateLink)**. This creates a private, secure entry point _directly_ to an AWS service (like S3, DynamoDB, or others) from _within_ your VPC. All traffic stays on the private AWS backbone and never goes out to the public internet.

### Network Access Control Lists

Shorten for [[ACLs]]
ACL is a firewall that controls traffic, both inbound and outbound.
It controls the traffic at the subnet level.
The ACL checks and controls the packets.
If the packet is on the approve