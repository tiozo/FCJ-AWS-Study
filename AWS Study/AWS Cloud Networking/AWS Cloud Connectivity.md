### AWS Virtual Private Cloud - [[AWS VPC]]

VPC is a service that lets you isolate your AWS resources in a isolated network.
Is the boundaries created around the resources let AWS restrict the network traffic.
In addition, it allows to include sections of the AWS cloud that you want in the isolated network.
Resources can be organized in subnets.
A subnet is a section in the VPC that contain specific resources.

### [[Internet Gateway]]

Public traffic can be allowed to your VPC.
The traffic is allowed by an Interface Gateway.
![[Pasted image 20251028103809.png]]An Internet Gateway is a door between the VPC and the internet.
The traffic enters the VPC through the Internet Gateway.
Without the Internet Gateway, you cannot access the resources in the VPC.

### [[Virtual Private Gateway]]

A Virtual Private Gateway is used to access private resources in the VPC.
It has extra layer of protection.
The Virtual Private Gateway encrypts the internet traffic keeping it protected.
It is a component that allows the encrypted traffic enter the VPC.
![[Pasted image 20251028104035.png]]

The Virtual Private Gateway allows you to make a Virtual Private Network (VPN) between the VPC and private network.
It only allows traffic from approved networks.
Many businesses use VPNs to ensure that their traffic and data are secure.