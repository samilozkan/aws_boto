# AWS Boto3 

Get started quickly using AWS with boto3, the AWS SDK for Python. Boto3 makes it easy to integrate your Python application, library, or script with AWS services including Amazon S3, Amazon EC2, Amazon DynamoDB, and more.

to install boto3

```pip install boto3```

 ## Key Features

#### Resource APIs

Boto3 has two distinct levels of APIs. Client (or "low-level") APIs provide one-to-one mappings to the underlying HTTP API operations. Resource APIs hide explicit network calls but instead provide resource objects and collections to access attributes and perform actions. For example:

`for i in ec2.instances.all():

        if i.state['Name'] == 'stopped':
        
            i.start()`