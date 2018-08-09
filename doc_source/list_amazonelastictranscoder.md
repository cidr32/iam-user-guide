# Actions, Resources, and Condition Keys for Amazon Elastic Transcoder<a name="list_amazonelastictranscoder"></a>

Amazon Elastic Transcoder \(service prefix: `elastictranscoder`\) provides the following service\-specific resources, actions, and condition context keys for use in IAM permission policies\.

References:
+ Learn how to [configure this service](http://docs.aws.amazon.com/elastictranscoder/latest/developerguide/)\.
+ View a [list of the API operations available for this service](http://docs.aws.amazon.com/elastictranscoder/latest/developerguide/)\.
+ Learn how to protect this service and its resources by [using IAM](http://docs.aws.amazon.com/elastictranscoder/latest/developerguide/access-control.html) permission policies\.

**Topics**
+ [Actions Defined by Amazon Elastic Transcoder](#amazonelastictranscoder-actions-as-permissions)
+ [Resources Defined by Elastic Transcoder](#amazonelastictranscoder-resources-for-iam-policies)
+ [Condition Keys for Amazon Elastic Transcoder](#amazonelastictranscoder-policy-keys)

## Actions Defined by Amazon Elastic Transcoder<a name="amazonelastictranscoder-actions-as-permissions"></a>

You can specify the following actions in the `Action` element of an IAM policy statement\. By using policies, you define the permissions for anyone performing an operation in AWS\. When you use an action in a policy, you usually allow or deny access to the API operation or CLI command with the same name\. However, in some cases, a single action controls access to more than one operation\. Alternatively, some operations require several different actions\. For details about the columns in the following table, see [The Actions Table](reference_policies_actions-resources-contextkeys.md#actions_table)\.


****  
[\[See the AWS documentation website for more details\]](http://docs.aws.amazon.com/IAM/latest/UserGuide/list_amazonelastictranscoder.html)

## Resources Defined by Elastic Transcoder<a name="amazonelastictranscoder-resources-for-iam-policies"></a>

The following resource types are defined by this service and can be used in the `Resource` element of IAM permission policy statements\. Each action in the [Actions table](#amazonelastictranscoder-actions-as-permissions) identifies the resource types that can be specified with that action\. A resource type can also define which condition keys you can include in a policy\. These keys are displayed in the last column of the table\. For details about the columns in the following table, see [The Resource Types Table](reference_policies_actions-resources-contextkeys.md#resources_table)\.


****  

| Resource Types | ARN | Condition Keys | 
| --- | --- | --- | 
|   [ job ](http://docs.aws.amazon.com/elastictranscoder/latest/developerguide/operations-jobs.html)  |  arn:$\{Partition\}:elastictranscoder:$\{Region\}:$\{Account\}:job/$\{JobId\}  |  | 
|   [ pipeline ](http://docs.aws.amazon.com/elastictranscoder/latest/developerguide/operations-pipelines.html)  |  arn:$\{Partition\}:elastictranscoder:$\{Region\}:$\{Account\}:pipeline/$\{PipelineId\}  |  | 
|   [ preset ](http://docs.aws.amazon.com/elastictranscoder/latest/developerguide/operations-presets.html)  |  arn:$\{Partition\}:elastictranscoder:$\{Region\}:$\{Account\}:preset/$\{PresetId\}  |  | 

## Condition Keys for Amazon Elastic Transcoder<a name="amazonelastictranscoder-policy-keys"></a>

Elastic Transcoder has no service\-specific context keys that can be used in the `Condition` element of policy statements\. For the list of the global context keys that are available to all services, see [Available Keys for Conditions](reference_policies_condition-keys.html#AvailableKeys) in the *IAM Policy Reference*\.