
### Domain Name System - [[DNS]]

DNS is the service that lets someone access a website from their browser.
Works like a phone book (text - phone number, you read it and know who to call)
It connects the IP address to the domain name. 
![[Pasted image 20251028111228.png]]
### [[AWS Route 53]]

Route 53 is a DNS web service.
It routes end users to internet apps hosted in AWS.
Route 53 connects users and their requests to AWS resources and external resources.

```
Route 53 has a feature to manage DNS records.
You can register new and transfer domains with Route 53.
You can manage all of your domain names from Route 53.
```

### Use [[AWS Route 53]] and [[AWS CloudFront]]
![[Pasted image 20251028111815.png]]
The picture explained:
The company has 3 [[AWS EC2|EC2]] Instances in an Auto Scaling group.
The group is attached to an [[AWS Application Load Balancer|Application Load Balancer]].
1. User requests data from the website application.
2. Route 53 uses DNS resolution to identify the IP address.
3. The data is sent back to the user.
4. The user request is sent to the nearest Edge Location through CloudFront.
5. CloudFront connects to the Application Load Balancer.
6. The Load Balancer sends the packet to the EC2 instance.