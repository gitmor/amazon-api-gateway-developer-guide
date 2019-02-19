# Document History<a name="history"></a>

The following table describes the important changes to the documentation since the last release of Amazon API Gateway\. For notification about updates to this documentation, you can subscribe to an RSS feed by choosing the RSS button in the top menu panel\.
+ **Latest documentation update:** September 6, 2018

| Change | Description | Date | 
| --- |--- |--- |
| [Active AWS X\-Ray integration](#history) | You can now use AWS X\-Ray to trace and analyze latencies in user requests as they travel through your APIs to the underlying services\. For more information, see [Trace API Gateway API Execution with AWS X\-Ray](https://docs.aws.amazon.com/apigateway/latest/developerguide/apigateway-xray.html)\.  | September 6, 2018 | 
| [Caching improvements](#history) | Only `GET` methods will have caching enabled by default when you enable caching for an API stage\. This helps to ensure the safety of your API\. You can enable caching for other methods by overriding method settings\. For more information, see [Enable API Caching to Enhance Responsiveness](https://docs.aws.amazon.com/apigateway/latest/developerguide/api-gateway-caching.html)\.  | August 20, 2018 | 
| [Service limits revised](#history) | Several limits have been revised: Increased number of APIs per account\. Increased API rate limits for Create/Import/Deploy APIs\. Corrected some rates from per minute to per second\. For more information, see [Limits](https://docs.aws.amazon.com/apigateway/latest/developerguide/limits.html)\.  | July 13, 2018 | 
| [Overriding API request and response parameters and headers](#history) | Added support for overriding request headers, query strings, and paths, as well as response headers and status codes\. For more information, see [Use a Mapping Template to Override an API's Request and Response Parameters and Headers](https://docs.aws.amazon.com/apigateway/latest/developerguide/apigateway-override-request-response-parameters.html)\. | July 12, 2018 | 
| [Method\-level throttling for usage plans](#history) | Added support for setting default per\-method throttling limits, as well as setting throttling limits for individual API methods in usage plan settings\. These settings are in addition to the existing account\-level throttling and default method\-level throttling limits that you can set in stage settings\. For more information, see [Throttle API Requests for Better Throughput](https://docs.aws.amazon.com/apigateway/latest/developerguide/api-gateway-request-throttling.html)\. | July 11, 2018 | 
| [API Gateway Developer Guide update notifications now available through RSS](#history) | The HTML version of the API Gateway Developer Guide now supports an RSS feed of updates that are documented on this **Document History** page\. The RSS feed includes updates made June 27, 2018, and later\. Previously announced updates are still available on this page\. Use the RSS button in the top menu panel to subscribe to the feed\. | June 27, 2018 | 

## Earlier Updates<a name="release-archive"></a>

The following table describes important changes in each release of the *API Gateway Developer Guide* before June 27, 2018\.


****  

| Change | Description | Date Changed | 
| --- | --- | --- | 
|  Private APIs  |  Added support for [private APIs](apigateway-private-apis.md), which you expose via [interface VPC endpoints](https://docs.aws.amazon.com/vpc/latest/userguide/vpce-interface.html)\. Traffic to your private APIs does not leave the Amazon network; it is isolated from the public internet\.  |  June 14, 2018  | 
|  Cross Account Lambda Authorizers and Integrations  |  Use an AWS Lambda function from a different AWS account as a Lambda authorizer function or as an API integration backend\. The other account can be in any region where Amazon API Gateway is available\. For more information, see [ Configure Cross\-Account Lambda Authorizer Using the API Gateway Console](apigateway-lambda-authorizer-cross-account-lambda-authorizer.md) and [Build an API Gateway API with Cross\-Account Lambda Proxy Integration](apigateway-cross-account-lambda-integrations.md)\.  |  April 2, 2018  | 
|  Resource Policies for APIs  |  Use API Gateway resource policies to enable users from a different AWS account to securely access your API or to allow the API to be invoked only from specified source IP address ranges or CIDR blocks\. For more information, see [Control Access to an API with Amazon API Gateway Resource Policies](apigateway-resource-policies.md)\.  |  April 2, 2018  | 
|  Tagging for API Gateway resources  |  Tag an API stage with up to 50 tags for cost allocation of API requests and caching in API Gateway\. For more information see [Set up Tags for an API Stage in API Gateway](set-up-tags.md)\.  |  December 19, 2017  | 
| Payload compression and decompression | Enable calling your API with compressed payloads using one of the supported content codings\. The compressed payloads are subject to mapping if a body\-mapping template is specified\. For more information, see [ Enable Payload Compression for an API ](api-gateway-gzip-compression-decompression.md)\.  | December 19, 2017 | 
| API key sourced from a custom authorizer | Return an API key from a custom authorizer to API Gateway to apply a usage plan for API methods that require the key\. For more information, see [Choose an API Key Source](api-gateway-api-key-source.md)\. | December 19, 2017 | 
| Authorization with OAuth 2 scopes | Enable authorization of method invocation by using OAuth 2 scopes with the COGNITO\_USER\_POOLS authorizer\. For more information, see [Use Amazon Cognito User Pools](apigateway-integrate-with-cognito.md)\. | December 14, 2017 | 
| Private Integration and VPC Link | Create an API with the API Gateway private integration to provide clients with access to HTTP/HTTPS resources in an Amazon VPC from outside of the VPC through a [VpcLink](https://docs.aws.amazon.com/apigateway/api-reference/resource/vpc-link/) resource\. For more information, see [Build an API with API Gateway Private Integration](getting-started-with-private-integration.md) and [Set up API Gateway Private Integrations](set-up-private-integration.md)\. | November 30, 2017 | 
| Deploy a Canary for API testing | Add a canary release to an existing API deployment to test a newer version of the API while keeping the current version in operation on the same stage\. You can set a percentage of stage traffic for the canary release and enable canary\-specific execution and access logged in separate CloudWatch Logs logs\. For more information, see [Set up an API Gateway Canary Release Deployment](canary-release.md)\. | November 28, 2017 | 
| Access Logging | Log client access to your API with data derived from [$context variables](api-gateway-mapping-template-reference.md#context-variable-reference) in a format of your choosing\. For more information, see [Set Up CloudWatch API Logging in API Gateway](set-up-logging.md)\. | November 21, 2017 | 
| Ruby SDK of an API | Generate a Ruby SDK for your API and use it to invoke your API methods\. For more information, see [Generate the Ruby SDK of an API](generate-ruby-sdk-of-an-api.md) and [Use a Ruby SDK Generated by API Gateway](how-to-call-sdk-ruby.md)\.  | November 20, 2017 | 
| Regional API endpoint | Specify a regional API endpoint to create an API for non\-mobile clients\. A non\-mobile client, such as an EC2 instance, runs in the same AWS Region where the API is deployed\. As with an edge\-optimized API, you can create a custom domain name for a regional API\. For more information, see [ Set up a Regional API in API Gateway ](create-regional-api.md) and [Set up a Custom Domain Name for a Regional API in API Gateway](apigateway-regional-api-custom-domain-create.md)\. | November 2, 2017 | 
| Custom request authorizer |  Use custom request authorizer to supply user\-authenticating information in request parameters to authorize API method calls\. The request parameters include headers and query string parameters as well as stage and context variables\. For more information, see [Use API Gateway Lambda Authorizers](apigateway-use-lambda-authorizer.md)\. | September 15, 2017 | 
| Customizing gateway responses |  Customize API Gateway\-generated gateway responses to API requests that failed to reach the integration backend\. A customized gateway message can provide the caller with API\-specific custom error messages, including returning needed CORS headers, or can transform the gateway response data to a format of an external exchange\. For more information, see [Set up Gateway Responses to Customize Error Responses](customize-gateway-responses.md)\. | June 6, 2017 | 
| Mapping Lambda custom error properties to method response headers |  Map individual custom error properties returned from Lambda to the method response header parameters using the integration\.response\.body parameter, relying API Gateway to deserialize the stringified custom error object at run time\. For more information, see [Handle Custom Lambda Errors in API Gateway](handle-errors-in-lambda-integration.md#handle-custom-errors-in-lambda-integration)\. | June 6, 2017 | 
| Throttling limits increase |  Increase the account\-level steady\-state request rate limit to 10,000 requests per second \(rps\) and the bust limit to 5000 concurrent requests\. For more information, see [Throttle API Requests for Better Throughput](api-gateway-request-throttling.md)\. | June 6, 2017 | 
| Validating method requests | Configure basic request validators on the API level or method levels so that API Gateway can validate incoming requests\. API Gateway verifies that required parameters are set and not blank, and verifies that the format of applicable payloads conforms to the configured model\. For more information, see [Enable Request Validation in API Gateway](api-gateway-method-request-validation.md)\. | April 11, 2017 | 
| Integrating with ACM | Use ACM Certificates for your API's custom domain names\. You can create a certificate in AWS Certificate Manager or import an existing PEM\-formatted certificate into ACM\. You then refer to the certificate's ARN when setting a custom domain name for your APIs\. For more information, see [Set up Custom Domain Name for an API in API Gateway](how-to-custom-domains.md)\. | March 9, 2017 | 
| Generating and calling a Java SDK of an API | Let API Gateway generate the Java SDK for your API and use the SDK to call the API in your Java client\. For more information, see [Use a Java SDK Generated by API Gateway](how-to-call-apigateway-generated-java-sdk.md)\. | January 13, 2017 | 
| Integrating with AWS Marketplace | Sell your API in a usage plan as a SaaS product through AWS Marketplace\. Use AWS Marketplace to extend the reach of your API\. Rely on AWS Marketplace for customer billing on your behalf\. Let API Gateway handle user authorization and usage metering\. For more information, see [Sell Your API as SaaS](sell-api-as-saas-on-aws-marketplace.md)\. | December 1, 2016 | 
| Enabling Documentation Support for your API | Add documentation for API entities in [DocumentationPart](https://docs.aws.amazon.com/apigateway/api-reference/resource/documentation-part/) resources in API Gateway\. Associate a snapshot of the collection DocumentationPart instances with an API stage to create a [DocumentationVersion](https://docs.aws.amazon.com/apigateway/api-reference/resource/documentation-version/)\. Publish API documentation by exporting a documentation version to an external file, such as a Swagger file\. For more information, see [Documenting an API Gateway API](api-gateway-documenting-api.md)\.  | December 1, 2016 | 
| Updated custom authorizer | A customer authorizer Lambda function now returns the caller's principal identifier\. The function also can return other information as key\-value pairs of the context map and an IAM policy\. For more information, see [Output from an Amazon API Gateway Lambda Authorizer](api-gateway-lambda-authorizer-output.md)\.  | December 1, 2016 | 
| Supporting binary payloads | Set [binaryMediaTypes](https://docs.aws.amazon.com/apigateway/api-reference/resource/rest-api/#binaryMediaTypes) on your API to support binary payloads of a request or response\. Set the contentHandling property on an [Integration](https://docs.aws.amazon.com/apigateway/api-reference/resource/integration/) or [IntegrationResponse](https://docs.aws.amazon.com/apigateway/api-reference/resource/integration-response/) to specify whether to handle a binary payload as the native binary blob, as a Base64\-enocded string, or as a passthrough without modifications\. For more information, see [Support Binary Payloads in API Gateway](api-gateway-payload-encodings.md)\.  | November 17, 2016 | 
| Enabling a proxy integration with an HTTP or Lambda backend through a proxy resource of an API\. | Create a proxy resource with a greedy path parameter of the form \{proxy\+\} and the catch\-all ANY method\. The proxy resource is integrated with an HTTP or Lambda backend using the HTTP or Lambda proxy integration, respectively\. For more information, see [Set up a Proxy Integration with a Proxy Resource](api-gateway-set-up-simple-proxy.md)\. | September 20, 2016 | 
| Extending selected APIs in API Gateway as product offerings for your customers by providing one or more usage plans\. | Create a usage plan in API Gateway to enable selected API clients to access specified API stages at agreed\-upon request rates and quotas\. For more information, see [Create and Use Usage Plans with API Keys](api-gateway-api-usage-plans.md)\. | August 11, 2016 | 
| Enabling method\-level authorization with a user pool in Amazon Cognito | Create a user pool in Amazon Cognito and use it as your own identity provider\. You can configure the user pool as a method\-level authorizer to grant access for users who are registered with the user pool\. For more information, see [Use Amazon Cognito User Pools](apigateway-integrate-with-cognito.md)\. | July 28, 2016 | 
| Enabling Amazon CloudWatch metrics and dimensions under the AWS/ApiGateway namespace\. | The API Gateway metrics are now standardized under the CloudWatch namespace of AWS/ApiGateway\. You can view them in both the API Gateway console and the Amazon CloudWatch console\. For more information, see [Amazon API Gateway Dimensions and Metrics](api-gateway-metrics-and-dimensions.md)\. | July 28, 2016 | 
| Enabling certificate rotation for a custom domain name |  Certificate rotation allows you to upload and renew an expiring certificate for a custom domain name\. For more information, see [Rotate a Certificate Imported into ACM](how-to-edge-optimized-custom-domain-name.md#how-to-rotate-custom-domain-certificate)\.  | April 27, 2016 | 
| Documenting changes for the updated Amazon API Gateway console\. | Learn how to create and set up an API using the updated API Gateway console\. For more information, see [Build an API Gateway API from an Example](api-gateway-create-api-from-example.md) and [Build an API with HTTP Custom Integration](api-gateway-create-api-step-by-step.md)\. | April 5, 2016 | 
| Enabling the Import API feature to create a new or update an existing API from external API definitions\. | With the Import API features, you can create a new API or update an existing one by uploading an external API definition expressed in Swagger 2\.0 with the API Gateway extensions\. For more information about the Import API, see [Import an API into API Gateway](api-gateway-import-api.md)\.  | April 5, 2016 | 
|  Exposing the $input\.body variable to access the raw payload as string and the $util\.parseJson\(\) function to turn a JSON string into a JSON object in a mapping template\. |  For more information about $input\.body and $util\.parseJson\(\), see [API Gateway Mapping Template Reference](api-gateway-mapping-template-reference.md)\. | April 5, 2016 | 
| Enabling client requests with method\-level cache invalidation, and improving request throttling management\.  | Flush API stage\-level cache and invalidate individual cache entry\. For more information, see [Flush the API Stage Cache in API Gateway](api-gateway-caching.md#flush-api-caching) and [Invalidate an API Gateway Cache Entry](api-gateway-caching.md#invalidate-method-caching)\. Improve the console experience for managing API request throttling\. For more information, see [Throttle API Requests for Better Throughput](api-gateway-request-throttling.md)\.  | March 25, 2016 | 
| Enabling and calling API Gateway API using custom authorization |  Create and configure an AWS Lambda function to implement custom authorization\. The function returns an IAM policy document that grants the Allow or Deny permissions to client requests of an API Gateway API\. For more information, see [Use API Gateway Lambda Authorizers](apigateway-use-lambda-authorizer.md)\.  | February 11, 2016 | 
| Importing and exporting API Gateway API using a Swagger definition file and extensions |  Create and update your API Gateway API using the Swagger specification with the API Gateway extensions\. Import the Swagger definitions using the API Gateway Importer\. Export an API Gateway API to a Swagger definition file using the API Gateway console or API Gateway Export API\. For more information, see [Import an API into API Gateway](api-gateway-import-api.md) and [Export an API](api-gateway-export-api.md)\.  | December 18, 2015 | 
| Mapping request or response body or body's JSON fields to request or response parameters\. | Map method request body or its JSON fields into integration request's path, query string, or headers\. Map integration response body or its JSON fields into request response's headers\. For more information, see [Amazon API Gateway API Request and Response Data Mapping Reference](request-response-data-mappings.md)\.  | December 18, 2015 | 
| Working with Stage Variables in Amazon API Gateway | Learn how to associate configuration attributes with a deployment stage of an API in Amazon API Gateway\. For more information, see [Set up Stage Variable for API Deployment](stage-variables.md)\. | November 5, 2015 | 
| How to: Enable CORS for a Method | It is now easier to enable cross\-origin resource sharing \(CORS\) for methods in Amazon API Gateway\. For more information, see [Enable CORS for a Resource](how-to-cors.md)\. | November 3, 2015 | 
| How to: Use Client Side SSL Authentication | Use Amazon API Gateway to generate SSL certificates that you can use to authenticate calls to your HTTP backend\. For more information, see [Use Client\-Side SSL Certificates for Authentication by the Backend](getting-started-client-side-ssl-authentication.md)\. | September 22, 2015 | 
| Mock integration of methods |  Learn how to [mock\-integrate an API with Amazon API Gateway](how-to-mock-integration.md)\. This feature enables developers to generate API responses from API Gateway directly without the need for a final integration backend beforehand\.  | September 1, 2015 | 
| Amazon Cognito Identity support | Amazon API Gateway has expanded the scope of the $context variable so that it now returns information about Amazon Cognito Identity when requests are signed with Amazon Cognito credentials\. In addition, we have added a $util variable for escaping characters in JavaScript and encoding URLs and strings\. For more information, see [API Gateway Mapping Template Reference](api-gateway-mapping-template-reference.md)\. | August 28, 2015 | 
| Swagger integration | Use the [Swagger import tool on GitHub](https://github.com/awslabs/aws-apigateway-swagger-importer) to import Swagger API definitions into Amazon API Gateway\. Learn more about [API Gateway Extensions to Swagger](api-gateway-swagger-extensions.md) to create and deploy APIs and methods using the import tool\. With the Swagger importer tool you can also update existing APIs\. | July 21, 2015 | 
| Mapping Template Reference |  Read about the `$input` parameter and its functions in the [API Gateway Mapping Template Reference](api-gateway-mapping-template-reference.md)\.  | July 18, 2015 | 
| Initial public release |  This is the initial public release of the *API Gateway Developer Guide*\.  | July 9, 2015 | 