# Actions, Resources, and Condition Keys for AWS Key Management Service<a name="list_awskeymanagementservice"></a>

AWS Key Management Service \(service prefix: `kms`\) provides the following service\-specific resources, actions, and condition context keys for use in IAM permission policies\.

References:
+ Learn how to [configure this service](http://docs.aws.amazon.com/kms/latest/developerguide/)\.
+ View a [list of the API operations available for this service](http://docs.aws.amazon.com/kms/latest/APIReference/)\.
+ Learn how to protect this service and its resources by [using IAM](http://docs.aws.amazon.com/kms/latest/developerguide/control-access.html) permission policies\.

**Topics**
+ [Actions Defined by AWS Key Management Service](#awskeymanagementservice-actions-as-permissions)
+ [Resources Defined by KMS](#awskeymanagementservice-resources-for-iam-policies)
+ [Condition Keys for AWS Key Management Service](#awskeymanagementservice-policy-keys)

## Actions Defined by AWS Key Management Service<a name="awskeymanagementservice-actions-as-permissions"></a>

You can specify the following actions in the `Action` element of an IAM policy statement\. By using policies, you define the permissions for anyone performing an operation in AWS\. When you use an action in a policy, you usually allow or deny access to the API operation or CLI command with the same name\. However, in some cases, a single action controls access to more than one operation\. Alternatively, some operations require several different actions\. For details about the columns in the following table, see [The Actions Table](reference_policies_actions-resources-contextkeys.md#actions_table)\.


****  
[\[See the AWS documentation website for more details\]](http://docs.aws.amazon.com/IAM/latest/UserGuide/list_awskeymanagementservice.html)

## Resources Defined by KMS<a name="awskeymanagementservice-resources-for-iam-policies"></a>

The following resource types are defined by this service and can be used in the `Resource` element of IAM permission policy statements\. Each action in the [Actions table](#awskeymanagementservice-actions-as-permissions) identifies the resource types that can be specified with that action\. A resource type can also define which condition keys you can include in a policy\. These keys are displayed in the last column of the table\. For details about the columns in the following table, see [The Resource Types Table](reference_policies_actions-resources-contextkeys.md#resources_table)\.


****  

| Resource Types | ARN | Condition Keys | 
| --- | --- | --- | 
|   [ alias ](http://docs.aws.amazon.com/kms/latest/developerguide/programming-aliases.html)  |  arn:$\{Partition\}:kms:$\{Region\}:$\{Account\}:alias/$\{Alias\}  |  | 
|   [ key ](http://docs.aws.amazon.com/kms/latest/developerguide/concepts.html#master_keys)  |  arn:$\{Partition\}:kms:$\{Region\}:$\{Account\}:key/$\{KeyId\}  |  | 

## Condition Keys for AWS Key Management Service<a name="awskeymanagementservice-policy-keys"></a>

AWS Key Management Service defines the following condition keys that can be used in the `Condition` element of an IAM policy\. You can use these keys to further refine the conditions under which the policy statement applies\. For details about the columns in the following table, see [The Condition Keys Table](reference_policies_actions-resources-contextkeys.md#context_keys_table)\.

To view the global condition keys that are available to all services, see [Available Global Condition Keys](reference_policies_condition-keys.html#AvailableKeys) in the *IAM Policy Reference*\.


****  

| Condition Keys | Description | Type | 
| --- | --- | --- | 
|   [ kms:BypassPolicyLockoutSafetyCheck ](http://docs.aws.amazon.com/kms/latest/developerguide/policy-conditions.html#conditions-kms-bypass-policy-lockout-safety-check)  | Controls access to the CreateKey and PutKeyPolicy operations based on the value of the BypassPolicyLockoutSafetyCheck parameter in the request\. | Bool | 
|   [ kms:CallerAccount ](http://docs.aws.amazon.com/kms/latest/developerguide/policy-conditions.html#conditions-kms-caller-account)  | Controls access to specified AWS KMS operations based on the AWS account ID of the caller\. You can use this condition to allow or deny access to to all IAM users and roles in an AWS account in a single policy statement\. | String | 
|   [ kms:EncryptionContextKeys ](http://docs.aws.amazon.com/kms/latest/developerguide/policy-conditions.html#conditions-kms-encryption-context-keys)  | Controls access based on the presence of specified keys in the encryption context\. The encryption context is an optional element in a cryptographic operation\. | String | 
|   [ kms:ExpirationModel ](http://docs.aws.amazon.com/kms/latest/developerguide/policy-conditions.html#conditions-kms-expiration-model)  | Controls access to the ImportKeyMaterial operation based on the value of the ExpirationModel parameter in the request\. | String | 
|   [ kms:GrantConstraintType ](http://docs.aws.amazon.com/kms/latest/developerguide/policy-conditions.html#conditions-kms-grant-constraint-type)  | Controls access to the CreateGrant operation based on the grant constraint in the request\. | String | 
|   [ kms:GrantIsForAWSResource ](http://docs.aws.amazon.com/kms/latest/developerguide/policy-conditions.html#conditions-kms-grant-is-for-aws-resource)  | Controls access to the CreateGrant operation when the request comes from a specified AWS service\. | Bool | 
|   [ kms:GrantOperations ](http://docs.aws.amazon.com/kms/latest/developerguide/policy-conditions.html#conditions-kms-grant-operations)  | Controls access to the CreateGrant operation based on the operations in the grant\. | String | 
|   [ kms:GranteePrincipal ](http://docs.aws.amazon.com/kms/latest/developerguide/policy-conditions.html#conditions-kms-grantee-principal)  | Controls access to the CreateGrant operation based on the grantee principal in the grant\. | String | 
|   [ kms:KeyOrigin ](http://docs.aws.amazon.com/kms/latest/developerguide/policy-conditions.html#conditions-kms-key-origin)  | Controls access to the CreateKey operation based on the value of the Origin parameter in the request\. The Origin parameter determines whether AWS KMS generates cryptographic material for the key or imports it\. | String | 
|   [ kms:ReEncryptOnSameKey ](http://docs.aws.amazon.com/kms/latest/developerguide/policy-conditions.html#conditions-kms-reencrypt-on-same-key)  | Controls access to the ReEncrypt operation when it uses the same customer master key that was used for the Encrypt operation\. | Bool | 
|   [ kms:RetiringPrincipal ](http://docs.aws.amazon.com/kms/latest/developerguide/policy-conditions.html#conditions-kms-retiring-principal)  | Controls access to the CreateGrant operation based on the retiring principal in the grant\. | String | 
|   [ kms:ValidTo ](http://docs.aws.amazon.com/kms/latest/developerguide/policy-conditions.html#conditions-kms-valid-to)  | Controls access to the ImportKeyMaterial operation based on the value of the ValidTo parameter in the request\. You can use this condition key to allow users to import key material only when it expires by the specified date\. | Numeric | 
|   [ kms:ViaService ](http://docs.aws.amazon.com/kms/latest/developerguide/policy-conditions.html#conditions-kms-via-service)  | Controls access when a request made on the principal's behalf comes from a specified AWS service\. | String | 
|   [ kms:WrappingAlgorithm ](http://docs.aws.amazon.com/kms/latest/developerguide/policy-conditions.html#conditions-kms-wrapping-algorithm)  | Controls access to the GetParametersForImport operation based on the value of the WrappingAlgorithm parameter in the request\. | String | 
|   [ kms:WrappingKeySpec ](http://docs.aws.amazon.com/kms/latest/developerguide/policy-conditions.html#conditions-kms-wrapping-key-spec)  | Controls access to the GetParametersForImport operation based on the value of the WrappingKeySpec parameter in the request\. | String | 