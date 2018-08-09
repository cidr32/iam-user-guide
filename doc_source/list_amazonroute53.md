# Actions, Resources, and Condition Keys for Amazon Route 53<a name="list_amazonroute53"></a>

Amazon Route 53 \(service prefix: `route53`\) provides the following service\-specific resources, actions, and condition context keys for use in IAM permission policies\.

References:
+ Learn how to [configure this service](http://docs.aws.amazon.com/Route53/latest/DeveloperGuide/)\.
+ View a [list of the API operations available for this service](http://docs.aws.amazon.com/Route53/latest/APIReference/)\.
+ Learn how to protect this service and its resources by [using IAM](http://docs.aws.amazon.com/Route53/latest/DeveloperGuide/auth-and-access-control.html) permission policies\.

**Topics**
+ [Actions Defined by Amazon Route 53](#amazonroute53-actions-as-permissions)
+ [Resources Defined by Route 53](#amazonroute53-resources-for-iam-policies)
+ [Condition Keys for Amazon Route 53](#amazonroute53-policy-keys)

## Actions Defined by Amazon Route 53<a name="amazonroute53-actions-as-permissions"></a>

You can specify the following actions in the `Action` element of an IAM policy statement\. By using policies, you define the permissions for anyone performing an operation in AWS\. When you use an action in a policy, you usually allow or deny access to the API operation or CLI command with the same name\. However, in some cases, a single action controls access to more than one operation\. Alternatively, some operations require several different actions\. For details about the columns in the following table, see [The Actions Table](reference_policies_actions-resources-contextkeys.md#actions_table)\.


****  
[\[See the AWS documentation website for more details\]](http://docs.aws.amazon.com/IAM/latest/UserGuide/list_amazonroute53.html)

## Resources Defined by Route 53<a name="amazonroute53-resources-for-iam-policies"></a>

The following resource types are defined by this service and can be used in the `Resource` element of IAM permission policy statements\. Each action in the [Actions table](#amazonroute53-actions-as-permissions) identifies the resource types that can be specified with that action\. A resource type can also define which condition keys you can include in a policy\. These keys are displayed in the last column of the table\. For details about the columns in the following table, see [The Resource Types Table](reference_policies_actions-resources-contextkeys.md#resources_table)\.


****  

| Resource Types | ARN | Condition Keys | 
| --- | --- | --- | 
|   [ change ](http://docs.aws.amazon.com/Route53/latest/APIReference/API_Change.html)  |  arn:$\{Partition\}:route53:::change/$\{Id\}  |  | 
|   [ delegationset ](http://docs.aws.amazon.com/Route53/latest/DeveloperGuide/route-53-concepts.html#route-53-concepts-reusable-delegation-set)  |  arn:$\{Partition\}:route53:::delegationset/$\{Id\}  |  | 
|   [ healthcheck ](http://docs.aws.amazon.com/Route53/latest/DeveloperGuide/route-53-concepts.html#route-53-concepts-health-check)  |  arn:$\{Partition\}:route53:::healthcheck/$\{Id\}  |  | 
|   [ hostedzone ](http://docs.aws.amazon.com/Route53/latest/DeveloperGuide/route-53-concepts.html#route-53-concepts-hosted-zone)  |  arn:$\{Partition\}:route53:::hostedzone/$\{Id\}  |  | 
|   [ trafficpolicy ](http://docs.aws.amazon.com/Route53/latest/DeveloperGuide/traffic-policies.html)  |  arn:$\{Partition\}:route53:::trafficpolicy/$\{Id\}  |  | 
|   [ trafficpolicyinstance ](http://docs.aws.amazon.com/Route53/latest/DeveloperGuide/traffic-policy-records.html)  |  arn:$\{Partition\}:route53:::trafficpolicyinstance/$\{Id\}  |  | 
|   [ queryloggingconfig ](http://docs.aws.amazon.com/Route53/latest/DeveloperGuide/query-logs.html)  |  arn:$\{Partition\}:route53:::queryloggingconfig/$\{Id\}  |  | 

## Condition Keys for Amazon Route 53<a name="amazonroute53-policy-keys"></a>

Route 53 has no service\-specific context keys that can be used in the `Condition` element of policy statements\. For the list of the global context keys that are available to all services, see [Available Keys for Conditions](reference_policies_condition-keys.html#AvailableKeys) in the *IAM Policy Reference*\.