# Amazon DynamoDB: Allows Access to a Specific Table<a name="reference_policies_examples_dynamodb_specific-table"></a>

This example shows how you might create a policy that allows full access to a DynamoDB table with the specified name\. This policy provides the permissions necessary to complete this action using the AWS API or AWS CLI only\. To use this policy, replace the red text in the example policy with your own information\.

**Important**  
This policy allows all actions that can be performed on a DynamoDB table\. To review these actions, see [DynamoDB API Permissions: Actions, Resources, and Conditions Reference](http://docs.aws.amazon.com/amazondynamodb/latest/developerguide/api-permissions-reference.html) in the* Amazon DynamoDB Developer Guide*\. You could provide the same permissions by listing each individual action\. However, if you use the wildcard \(`*`\) in the `Action` element, such as `"dynamodb:List*"`, then you don't have to update your policy if DynamoDB adds a new List action\. 

This policy allows actions only on DynamoDB tables that exist with the specified name\. To allow your users `Read` access to everything in DynamoDB, you can also attach the [AmazonDynamoDBReadOnlyAccess](https://console.aws.amazon.com/iam/home#policies/arn:aws:iam::aws:policy/AmazonDynamoDBReadOnlyAccess) AWS managed policy\.

```
{
    "Version": "2012-10-17",
    "Statement": [
        {
            "Sid": "ListAndDescribe",
            "Effect": "Allow",
            "Action": [
                "dynamodb:List*",
                "dynamodb:DescribeReservedCapacity*",
                "dynamodb:DescribeLimits",
                "dynamodb:DescribeTimeToLive"
            ],
            "Resource": "*"
        },
        {
            "Sid": "SpecificTable",
            "Effect": "Allow",
            "Action": [
                "dynamodb:BatchGet*",
                "dynamodb:DescribeStream",
                "dynamodb:DescribeTable",
                "dynamodb:Get*",
                "dynamodb:Query",
                "dynamodb:Scan",
                "dynamodb:BatchWrite*",
                "dynamodb:CreateTable",
                "dynamodb:Delete*",
                "dynamodb:Update*",
                "dynamodb:PutItem"
            ],
            "Resource": "arn:aws:dynamodb:*:*:table/<TABLE-NAME>"
        }
    ]
}
```