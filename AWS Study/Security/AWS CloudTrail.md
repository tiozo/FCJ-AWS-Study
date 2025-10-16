### Cloud Action Logging Service - AWS CloudTrail

CloudTrail logs actions inside your AWS environment. 
It records API Calls on your account.
Can be used as a way to track all the cost that may not appear on Cost Explorer.

> [!Additional Notes]
Cost Explorer may only show generic information about which service is costing you or the information is hidden under multiple filter. CloudTrail will give you a full log, and from the logs you can research from the logs, which type of call will cost you money.


### [[CloudTrail]]

CloudTrail logs actions on your account as a trail.
Example of data logs:
- Identity
- Time
- IP address
- and much more.
CloudTrail gives a complete history of user activity and API calls on your resources.

> [!Warning]
> Using CloudTrail is free but the storage for all the logs may cost you money (S3 Charges) when creating a Trails.
> Delete for each Trail won't empty the correspond S3 used for logging activities.


### [[CloudTrail Events]] 

CloudTrail can be used to create events.
Events are set up to understand what has happened.
CloudTrail lets you filter and locates specific events.
Events can for example, tell us:
- What?
- Who?
- When?
- How?
The event gives situational insight.

### [[CloudTrail Insights]]

CloudTrail has feature called CloudTrail Insights. 
Insight let you detect unusual API activities on your account automatically.

> [!Read more]
> [CloudTrail Insight](http://docs.aws.amazon.com/awscloudtrail/latest/userguide/logging-insights-events-with-cloudtrail.html)

