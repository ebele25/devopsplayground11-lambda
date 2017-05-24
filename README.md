# Hands On Serverless Computing with Lambda

[Sample Site](http://static.meetup.ecs-digital.co.uk.s3-website-us-west-2.amazonaws.com/index.html) | [AWS Console](https://devopsplayground.signin.aws.amazon.com/console)

## Login

- __AWS Console:__ `https://devopsplayground.signin.aws.amazon.com/console`
- __Username:__ `<TBA>`
- __Password:__ `<TBA>`

The topics for this hands-on session will be AWS Lambda, function as a service (FaaS). During this Playground you will create a website hosted on AWS S3 using AWS Lambda and Amazon API Gateway to add dynamic functionality to the site.

![Steps](https://raw.githubusercontent.com/ForestTechnologiesLtd/devopsplayground11-lambda/master/diagrams/pg11-intro-steps.png)

Each step will be associated with a Lab to complete build on the previous lab to progress. A Completed lab website is a available for view from the link above 'Sample Site'. All labs have been tested with the `US Oregon` region.

## Labs

1. [Lab-001 - Build Static Website with s3 Bucket](doc/lab-001.md)
1. [Lab-002 - Sharing resources between s3 Buckets](doc/lab-002.md)
1. [Lab-003 - Web Services with Lambda](doc/lab-003.md)
1. [Lab-004 - Posting Data with Lambda](doc/lab-004.md)


## Prerequisites
- Login to AWS account
- Permissions to create S3 Buckets
- Permissions to write and execute lambda functions
- Permission to create API Gateway
- __Region:__ Oregon


## IAM Roles needed for Labs

If you attempt the labs in your own AWS account you will need to create the following roles:

- AWSS3FullAccess
- AWSLambdaFullAccess
- AmazonAPIGatewayAdministrator
- AWSLambdaExecute

![IAM Roles needed for Labs](https://raw.githubusercontent.com/ForestTechnologiesLtd/devopsplayground11-lambda/master/diagrams/pg11-iam-roles.png)

###  Safari : Enable the hidden Develop menu

Some labs will require having access to a javascript to see Browser errors like lab-002 for Cross Origin Resource Sharing. Safari has these development tools built-in however they need to be enabled.

#### Steps
1. Safari > Preferences
1. Check 'Show Develop menu in menu bar' (see image Safari Advanced Preferences red box)
1. Safari menu bar should now show as in 'Safari Menu Bar' image below

#### Image: Safari Advanced Preferences
![Safari Advanced Preferences Pane](https://raw.githubusercontent.com/ForestTechnologiesLtd/devopsplayground11-lambda/master/diagrams/safari_adv_pane.png)

#### Image: Safari Menu bar
![Safari Menu](https://raw.githubusercontent.com/ForestTechnologiesLtd/devopsplayground11-lambda/master/diagrams/safari_menu.png)


## Checkout code from GitHub

```bash
git clone https://github.com/ForestTechnologiesLtd/devopsplayground11-lambda.git
cd devopsplayground11-lambda
```


# What is Serverless ?

A computing model where the existence of servers are hidden from developers. Within AWS eco-system Lambda is only serverless service. The the purpose of these labs we will look at S3, Lambda, and API Gateway.

- __Storage__ - S3
- __Compute__ - Lambda
- __Database__ - DynamoDB, ElasticCache
- __API Proxy__ - API Gateway
- __Analytics__ - AWS Kinesis
- __Messaging & Queues__ - AWS SNS, SQS
- __State Management__ - AWS Step Functions
- __Diagnostics__ - AWS X-Ray
