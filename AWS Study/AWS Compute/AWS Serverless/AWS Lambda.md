### Serverless Cloud Compute - AWS Lambda

AWS Lambda is a serverless compute service.
"Think about code, no server needed."

### How does it works ?

High level concept:
1. Deploy your code to Lambda
2. Make the code ready to trigger an event
3. The code only runs when triggered
4. Pay only when your code is running

Examples: 
1. EC2 is like renting a room to stay 24/7 which maybe more than you need and is fixed size. (May or may not comes with utilities)
2. Serverless is like booking a hotel/homestay, based on demand (least people or many people) for how many times that's predefined. (Will comes with all utilities)

### What is AWS Lambda?

Serverless computing helps abstract the infrastructure in the cloud.
As a result, it reduces costs and can help to increase innovation.
AWS Lambda can be used to:
- Build and deploy apps
- Monitor and maintain apps

Back-End Code

Lambda can run Back-End code.

Here are some popular Back-End languages that [lambda supports](https://docs.aws.amazon.com/lambda/latest/dg/lambda-runtimes.html)
- **Node.js** 
- **Python** 
- **Java**
- **Kotlin**
- **C#**

>[!Tips]
>Use ARM for better cost optimizations, as the cost of ARM is much cheaper than x86.

