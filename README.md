# AWS Boto3 

What if the capabilities of your laptop no longer constrained you? Could you get an SMS when a city garbage truck camera spots a missing cat? All of them are possible with cloud technology. This repository will look at how to integrate Amazon Web Services (AWS) into your data workflow. We will focus on how to upload data to S3, AWS cloud storage.

- We’ll use triggers from your analysis to send text messages with AWS SNS.

- We will use Rekognition to detect objects in an image. And we will use Comprehend to decide if a piece of feedback is negative. 

- By the time we’re done, we will learn how to build a pipeline, subscribe people to it, and send them text messages when an image contains a bike!


## AWS SDK for Python (Boto3)
Get started quickly using AWS with boto3, the AWS SDK for Python. Boto3 makes it easy to integrate your Python application, library, or script with AWS services including Amazon S3, Amazon EC2, Amazon DynamoDB, and more.

to install boto3

```pip install boto3```

 ## Key Features

#### Resource APIs

Boto3 has two distinct levels of APIs. Client (or "low-level") APIs provide one-to-one mappings to the underlying HTTP API operations. Resource APIs hide explicit network calls but instead provide resource objects and collections to access attributes and perform actions. For example:

```
for i in ec2.instances.all():


    if i.state['Name'] == 'stopped':


        i.start()

