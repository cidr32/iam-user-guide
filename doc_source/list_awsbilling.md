# Actions, Resources, and Condition Keys for AWS Billing<a name="list_awsbilling"></a>

AWS Billing \(service prefix: `aws-portal`\) provides the following service\-specific resources, actions, and condition context keys for use in IAM permission policies\.

References:
+ Learn how to [configure this service](http://docs.aws.amazon.com/awsaccountbilling/latest/aboutv2/)\.
+ View a [list of the API operations available for this service](http://docs.aws.amazon.com/awsaccountbilling/latest/aboutv2/)\.
+ Learn how to protect this service and its resources by [using IAM](http://docs.aws.amazon.com/awsaccountbilling/latest/aboutv2/grantaccess.html) permission policies\.

**Topics**
+ [Actions Defined by AWS Billing](#awsbilling-actions-as-permissions)
+ [Resources Defined by Billing](#awsbilling-resources-for-iam-policies)
+ [Condition Keys for AWS Billing](#awsbilling-policy-keys)

## Actions Defined by AWS Billing<a name="awsbilling-actions-as-permissions"></a>

You can specify the following actions in the `Action` element of an IAM policy statement\. By using policies, you define the permissions for anyone performing an operation in AWS\. When you use an action in a policy, you usually allow or deny access to the API operation or CLI command with the same name\. However, in some cases, a single action controls access to more than one operation\. Alternatively, some operations require several different actions\. For details about the columns in the following table, see [The Actions Table](reference_policies_actions-resources-contextkeys.md#actions_table)\.


****  

| Actions | Description | Access Level | Resource Types \(\*required\) | Condition Keys | Dependent Actions | 
| --- | --- | --- | --- | --- | --- | 
|   [ ModifyAccount ](http://docs.aws.amazon.com/awsaccountbilling/latest/aboutv2/billing-permissions-ref.html#user-permissions)  | Allow or deny IAM users permission to modify Account Settings\. | Write |  |  |  | 
|   [ ModifyBilling ](http://docs.aws.amazon.com/awsaccountbilling/latest/aboutv2/billing-permissions-ref.html#user-permissions)  | Allow or deny IAM users permission to modify billing settings\. | Write |  |  |  | 
|   [ ModifyPaymentMethods ](http://docs.aws.amazon.com/awsaccountbilling/latest/aboutv2/billing-permissions-ref.html#user-permissions)  | Allow or deny IAM users permission to modify payment methods\. | Write |  |  |  | 
|   [ ViewAccount ](http://docs.aws.amazon.com/awsaccountbilling/latest/aboutv2/billing-permissions-ref.html#user-permissions)  | Allow or deny IAM users permission to view account settings\. | Read |  |  |  | 
|   [ ViewBilling ](http://docs.aws.amazon.com/awsaccountbilling/latest/aboutv2/billing-permissions-ref.html#user-permissions)  | Allow or deny IAM users permission to view billing pages in the console\. | Read |  |  |  | 
|   [ ViewPaymentMethods ](http://docs.aws.amazon.com/awsaccountbilling/latest/aboutv2/billing-permissions-ref.html#user-permissions)  | Allow or deny IAM users permission to view payment methods\. | Read |  |  |  | 
|   [ ViewUsage ](http://docs.aws.amazon.com/awsaccountbilling/latest/aboutv2/billing-permissions-ref.html#user-permissions)  | Allow or deny IAM users permission to view AWS usage reports\. | Read |  |  |  | 

## Resources Defined by Billing<a name="awsbilling-resources-for-iam-policies"></a>

AWS Billing has no service\-defined resources that can be used as the `Resource` element of an IAM policy statement\.

## Condition Keys for AWS Billing<a name="awsbilling-policy-keys"></a>

Billing has no service\-specific context keys that can be used in the `Condition` element of policy statements\. For the list of the global context keys that are available to all services, see [Available Keys for Conditions](reference_policies_condition-keys.html#AvailableKeys) in the *IAM Policy Reference*\.