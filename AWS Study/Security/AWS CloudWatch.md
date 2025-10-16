### Cloud Monitoring and Management Service - AWS CloudWatch

CloudWatch lets you monitor your resources.
Is a web-based service.
Configure the service to monitor and set alarms based on your metrics.

> [!Additional Content]
 *Read more about [metrics](https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/working_with_metrics.html)*

### [[CloudWatch Alarms]]

Lets you create automatic alarms.
Configure the alarms as user's intend.
Alarms are triggered at threshold defined by user.
Alarms are used to <mark style="background-color: #a9f5eb;">control resources</mark>. For example, stop idle or near to inactive services.

> [!Additional content]
*Read more about [Alarms](https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/AlarmThatSendsEmail.html)*

### [[CloudWatch Dashboard]]

Can be accessed via browser.
Can add widget and view for each metrics under some form of visualization.
This will cost the storage.
Each widget can be modify to be used as a cost monitoring using basic math functions.

> [!Additional content]
> https://saviorab1.github.io/fcj-leftover/11-monitoring-with-cloudwatch/

>[!Warning]
>CloudWatch isn't a free service and will charge differently for each kind of metrics and volume used.
>Some Metric will require you to activate them by yourself and will cost you, differently base on what type of metric you used. 
>Metrics will be updated every minutes (Careful for charged on demand metrics)
>View more at: [CloudWatch Pricing](https://aws.amazon.com/cloudwatch/pricing/)
