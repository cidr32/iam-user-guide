# Actions, Resources, and Condition Keys for Amazon CloudFront<a name="list_amazoncloudfront"></a>

Amazon CloudFront \(service prefix: `cloudfront`\) provides the following service\-specific resources, actions, and condition context keys for use in IAM permission policies\.

References:
+ Learn how to [configure this service](http://docs.aws.amazon.com/AmazonCloudFront/latest/DeveloperGuide/)\.
+ View a [list of the API operations available for this service](http://docs.aws.amazon.com/AmazonCloudFront/latest/APIReference/)\.
+ Learn how to protect this service and its resources by [using IAM](http://docs.aws.amazon.com/AmazonCloudFront/latest/DeveloperGuide/auth-and-access-control.html) permission policies\.

**Topics**
+ [Actions Defined by Amazon CloudFront](#amazoncloudfront-actions-as-permissions)
+ [Resources Defined by CloudFront](#amazoncloudfront-resources-for-iam-policies)
+ [Condition Keys for Amazon CloudFront](#amazoncloudfront-policy-keys)

## Actions Defined by Amazon CloudFront<a name="amazoncloudfront-actions-as-permissions"></a>

You can specify the following actions in the `Action` element of an IAM policy statement\. By using policies, you define the permissions for anyone performing an operation in AWS\. When you use an action in a policy, you usually allow or deny access to the API operation or CLI command with the same name\. However, in some cases, a single action controls access to more than one operation\. Alternatively, some operations require several different actions\. For details about the columns in the following table, see [The Actions Table](reference_policies_actions-resources-contextkeys.md#actions_table)\.


****  

| Actions | Description | Access Level | Resource Types \(\*required\) | Condition Keys | Dependent Actions | 
| --- | --- | --- | --- | --- | --- | 
|   [ CreateCloudFrontOriginAccessIdentity ](http://docs.aws.amazon.com/AmazonCloudFront/latest/APIReference/API_CreateCloudFrontOriginAccessIdentity.html)  | This action creates a new CloudFront origin access identity \(POST /2016\-11\-25/origin\-access\-identity/cloudfront\)\. | Write |  |  |  | 
|   [ CreateDistribution ](http://docs.aws.amazon.com/AmazonCloudFront/latest/APIReference/API_CreateDistribution.html)  | This action creates a new web distribution \(POST /2016\-11\-25/distribution\)\. | Write |  |  |  | 
|   [ CreateDistributionWithTags ](http://docs.aws.amazon.com/AmazonCloudFront/latest/APIReference/API_CreateDistributionWithTags.html)  | This action creates a new web distribution with tags \(POST /2016\-11\-25/distribution?WithTags\)\. | Tagging |  |  |  | 
|   [ CreateInvalidation ](http://docs.aws.amazon.com/AmazonCloudFront/latest/APIReference/API_CreateInvalidation.html)  | This action creates a new invalidation batch request \(POST /2016\-11\-25/distribution/<DISTRIBUTION\_ID>/invalidation\)\. | Write |  |  |  | 
|   [ CreateStreamingDistribution ](http://docs.aws.amazon.com/AmazonCloudFront/latest/APIReference/API_CreateStreamingDistribution.html)  | This action creates a new RTMP distribution \(POST /2016\-11\-25/streaming\-distribution\)\. | Write |  |  |  | 
|   [ CreateStreamingDistributionWithTags ](http://docs.aws.amazon.com/AmazonCloudFront/latest/APIReference/API_CreateStreamingDistributionWithTags.html)  | This action creates a new RTMP distribution with tags \(POST /2016\-11\-25/streaming\-distribution?WithTags\)\. | Tagging |  |  |  | 
|   [ DeleteCloudFrontOriginAccessIdentity ](http://docs.aws.amazon.com/AmazonCloudFront/latest/APIReference/API_DeleteCloudFrontOriginAccessIdentity.html)  | This action deletes a CloudFront origin access identity \(DELETE /2016\-11\-25/origin\-access\-identity/cloudfront/<OAI\_ID>\)\. | Write |  |  |  | 
|   [ DeleteDistribution ](http://docs.aws.amazon.com/AmazonCloudFront/latest/APIReference/API_DeleteDistribution.html)  | This action deletes a web distribution \(DELETE /2016\-11\-25/distribution/<DISTRIBUTION\_ID>\)\. | Write |  |  |  | 
|   [ DeleteStreamingDistribution ](http://docs.aws.amazon.com/AmazonCloudFront/latest/APIReference/API_DeleteStreamingDistribution.html)  | This action deletes an RTMP distribution \(DELETE /2016\-11\-25/streaming\-distribution/<DISTRIBUTION\_ID>\)\. | Write |  |  |  | 
|   [ GetCloudFrontOriginAccessIdentity ](http://docs.aws.amazon.com/AmazonCloudFront/latest/APIReference/API_GetCloudFrontOriginAccessIdentity.html)  | Get the information about a CloudFront origin access identity \(GET /2016\-11\-25/origin\-access\-identity/cloudfront/<OAI\_ID>\)\. | Read |  |  |  | 
|   [ GetCloudFrontOriginAccessIdentityConfig ](http://docs.aws.amazon.com/AmazonCloudFront/latest/APIReference/API_GetCloudFrontOriginAccessIdentityConfig.html)  | Get the configuration information about a Cloudfront origin access identity \(GET /2016\-11\-25/origin\-access\-identity/cloudfront/<OAI\_ID>/config\)\. | Read |  |  |  | 
|   [ GetDistribution ](http://docs.aws.amazon.com/AmazonCloudFront/latest/APIReference/API_GetDistribution.html)  | Get the information about a web distribution \(GET /2016\-11\-25/distribution/<DISTRIBUTION\_ID>\)\. | Read |  |  |  | 
|   [ GetDistributionConfig ](http://docs.aws.amazon.com/AmazonCloudFront/latest/APIReference/API_GetDistributionConfig.html)  | Get the configuration information about a distribution \(GET /2016\-11\-25/distribution/<DISTRIBUTION\_ID>/config\)\. | Read |  |  |  | 
|   [ GetInvalidation ](http://docs.aws.amazon.com/AmazonCloudFront/latest/APIReference/API_GetInvalidation.html)  | Get the information about an invalidation \(GET /2016\-11\-25/distribution/<DISTRIBUTION\_ID>/invalidation/<INVALIDATION\_ID>\)\. | Read |  |  |  | 
|   [ GetStreamingDistribution ](http://docs.aws.amazon.com/AmazonCloudFront/latest/APIReference/API_GetStreamingDistribution.html)  | Get the information about an RTMP distribution \(GET /2016\-11\-25/streaming\-distribution/<DISTRIBUTION\_ID>\)\. | Read |  |  |  | 
|   [ GetStreamingDistributionConfig ](http://docs.aws.amazon.com/AmazonCloudFront/latest/APIReference/API_GetStreamingDistributionConfig.html)  | Get the configuration information about a streaming distribution \(GET /2016\-11\-25/streaming\-distribution/<DISTRIBUTION\_ID>/config\)\. | Read |  |  |  | 
|   [ ListCloudFrontOriginAccessIdentities ](http://docs.aws.amazon.com/AmazonCloudFront/latest/APIReference/API_ListCloudFrontOriginAccessIdentities.html)  | List your CloudFront origin access identities \(GET /2016\-11\-25/origin\-access\-identity/cloudfront?Marker=<MARKER>&MaxItems=<MAX\_ITEMS>\)\. | List |  |  |  | 
|   [ ListDistributions ](http://docs.aws.amazon.com/AmazonCloudFront/latest/APIReference/API_ListDistributions.html)  | List the distributions associated with your AWS account \(GET /2016\-11\-25/distribution?Marker=<MARKER>&MaxItems=<MAX\_ITEMS>\)\. | List |  |  |  | 
|   [ ListDistributionsByWebACLId ](http://docs.aws.amazon.com/AmazonCloudFront/latest/APIReference/API_ListDistributionsByWebACLId.html)  | List the distributions associated with your AWS account with given AWS WAF web ACL \(GET /2016\-11\-25/distributionsByWebACLId/<WEB\_ACL\_ID>?Marker=<MARKER>&MaxItems=<MAX\_ITEMS>\)\. | List |  |  |  | 
|   [ ListInvalidations ](http://docs.aws.amazon.com/AmazonCloudFront/latest/APIReference/API_ListInvalidations.html)  | List your invalidation batches \(GET /2016\-11\-25/distribution/<DISTRIBUTION\_ID>/invalidation?Marker=<MARKER>&MaxItems=<MAX\_ITEMS>\)\. | List |  |  |  | 
|   [ ListStreamingDistributions ](http://docs.aws.amazon.com/AmazonCloudFront/latest/APIReference/API_ListStreamingDistributions.html)  | List your RTMP distributions \(GET /2016\-11\-25/streaming\-distribution?Marker=<MARKER>&MaxItems=<MAX\_ITEMS>\)\. | List |  |  |  | 
|   [ ListTagsForResource ](http://docs.aws.amazon.com/AmazonCloudFront/latest/APIReference/API_ListTagsForResource.html)  | List tags for a CloudFront resource \(GET /2016\-11\-25/tagging?Resource=<RESOURCE>\)\. | Read |  |  |  | 
|   [ TagResource ](http://docs.aws.amazon.com/AmazonCloudFront/latest/APIReference/API_TagResource.html)  | Add tags to a CloudFront resource \(POST /2016\-11\-25/tagging?Operation=Tag?Resource=<RESOURCE>\)\. | Tagging |  |  |  | 
|   [ UntagResource ](http://docs.aws.amazon.com/AmazonCloudFront/latest/APIReference/API_UntagResource.html)  | Remove tags from a CloudFront resource \(POST /2016\-11\-25/tagging?Operation=Untag?Resource=<RESOURCE>\)\. | Tagging |  |  |  | 
|   [ UpdateCloudFrontOriginAccessIdentity ](http://docs.aws.amazon.com/AmazonCloudFront/latest/APIReference/API_UpdateCloudFrontOriginAccessIdentity.html)  | This action sets the configuration for a CloudFront origin access identity \(PUT /2016\-11\-25/origin\-access\-identity/cloudfront/<OAI\_ID>/config\)\. | Write |  |  |  | 
|   [ UpdateDistribution ](http://docs.aws.amazon.com/AmazonCloudFront/latest/APIReference/API_UpdateDistribution.html)  | This action updates the configuration for a web distribution \(PUT /2016\-11\-25/distribution/<DISTRIBUTION\_ID>/config\)\. | Write |  |  |  | 
|   [ UpdateStreamingDistribution ](http://docs.aws.amazon.com/AmazonCloudFront/latest/APIReference/API_UpdateStreamingDistribution.html)  | This action updates the configuration for an RTMP distribution \(PUT /2016\-11\-25/streaming\-distribution/<DISTRIBUTION\_ID>/config\)\. | Write |  |  |  | 

## Resources Defined by CloudFront<a name="amazoncloudfront-resources-for-iam-policies"></a>

Amazon CloudFront has no service\-defined resources that can be used as the `Resource` element of an IAM policy statement\.

## Condition Keys for Amazon CloudFront<a name="amazoncloudfront-policy-keys"></a>

CloudFront has no service\-specific context keys that can be used in the `Condition` element of policy statements\. For the list of the global context keys that are available to all services, see [Available Keys for Conditions](reference_policies_condition-keys.html#AvailableKeys) in the *IAM Policy Reference*\.