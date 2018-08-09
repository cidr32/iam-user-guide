# Amazon EC2: Allows Starting or Stopping an EC2 Instance and Modifying a Security Group, Programmatically and in the Console<a name="reference_policies_examples_ec2_instance-securitygroup"></a>

This example shows how you might create a policy that allows starting or stopping a specific EC2 instance and modifying a specific security group\. This policy also provides the permissions necessary to complete this action on the console\. To use this policy, replace the red text in the example policy with your own information\.

```
{
    "Version": "2012-10-17",
    "Statement": [
        {
            "Action": [
                "ec2:DescribeInstances",
                "ec2:DescribeSecurityGroups",
                "ec2:DescribeSecurityGroupReferences",
                "ec2:DescribeStaleSecurityGroups"
            ],
            "Resource": "*",
            "Effect": "Allow"
        },
        {
            "Action": [
                "ec2:AuthorizeSecurityGroupEgress",
                "ec2:AuthorizeSecurityGroupIngress",
                "ec2:RevokeSecurityGroupEgress",
                "ec2:RevokeSecurityGroupIngress",
                "ec2:StartInstances",
                "ec2:StopInstances"
            ],
            "Resource": [
                "arn:aws:ec2:*:*:instance/i-<INSTANCE-ID>",
                "arn:aws:ec2:*:*:security-group/sg-<SECURITY-GROUP-ID>"
            ],
            "Effect": "Allow"
        }
    ]
}
```