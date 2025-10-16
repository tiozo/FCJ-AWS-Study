Known as [[AWS IAM]].
Help mange AWS resources and services.

IAM features are: 
- AWS account root user.
- IAM Users
- IAM Policy
- IAM Groups
- IAM roles
- Multi-factor authentication (MFA)

### AWS Account root user 

Created on first start of my AWS account.
Accessed via AWS account credentials.
Have full control over the resources and AWS services.
Good practices: 
- Avoid using Root on daily tasks
- Use it to create IAM with permissions to create other users (Should follow Least Privileges Principle to maintain security over AWS resources).
- Use it for root user-specific tasks.

![[Pasted image 20251016101148.png]]
*Image created by Amazon Web Services*

### IAM [[Users]]

IAM user represents an entity (could be a person or an application) that interact with AWS resources/services.
IAM user is made of credentials and a name.
It is created without permissions by default.
Root user can grant permissions to the IAM User (Can use admin policy or IAM Read/Write policy)
It is recommended to have an account for each individual "Entity".

### [[IAM Policies]]

IAM policies are documents.
They deny or allow permissions to AWS resources and services.
Customize user access to AWS resources and services.
You can give only those permissions that each user needs.
IAM Policy (Json) Examples
![[Pasted image 20251016101931.png]]
*Image created by Amazon Web Services*
### [[IAM Groups]]

A collections of IAM users is called IAM group.
IAM policy is assigned to group will grant every entity in the group to have the permissions defined within that policy.

![[Pasted image 20251016101607.png]]
*Image created by Amazon Web Services*
### [[IAM roles]]

An temporary access to services or resources.
Before an IAM role can be given, IAM user, service, or application must have permission to switch roles.
It is best for cases where temporary access needs to be given.

### [[MFA]]
Is a multi-step authentication.
Provide more authentication form.
An extra layer of security.