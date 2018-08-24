# ec2-start-stop script
Extremely simple script to batch power on or off ec2 instances

Add the instance id's and region to the script. Then just pass `start` or `stop` as a command line parameter. 

### Example IAM policy: 
```
{
    "Version": "2012-10-17",
    "Statement": [
        {
            "Sid": "VisualEditor0",
            "Effect": "Allow",
            "Action": [
                "ec2:DescribeInstances",
                "ec2:StartInstances",
                "ec2:StopInstances",
                "ec2:DescribeInstanceStatus"
            ],
            "Resource": "*"
        }
    ]
}
```
