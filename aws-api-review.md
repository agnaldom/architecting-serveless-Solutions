# AWS API Gateway Self-check

1. Wich of these are feature of Amazon API Gateway?

* provides built-in CloudWatch monitoring
* Incorporates a CloudFront distribuition.
* Allows you to generate SDKs.
* Triggers Lambda functions synchronously.
* Allows you to run multiple version of an API.

2. Which API Gateway endpoint type would you use for public-facing
global web application?

* Edge-optimized

3. Match the scenario to its suggested authorizarion option.

* IAM authorizes:
  * Internal service with limited consumers
  * requests signed with AWS Sig V4
* Lambda authorizes
  * authorizations based on info in request header
  * existing OATH strategy
* Cognito authorizers
  * public mobile application
  * user registration and sign-in directly in the application

4. Which of the following statements are true?

* You can grant permission to invoke an API with execute-API
* Resource policies can restrict access by account.
* You can grant permission to manager an API with apigateway.

5. Put these API throttling options in the order in which they
would be applied to a request.

* 1 Per client, per method limits ser for an API stage in a usage plan
* 2 Per client limits set in a usage plan
* 3 Default method limits set in API stoge settings
* 4 The account level limit

6. Which of the following statements about API Gateway is FALSE?

* When you test from the console, no logs are written to CLoudWatch, and 
the API executions are only simulated.

7. Match the API Gateway information found in CloudWatch to its description.

* Details about who accessed your API
  * Access Logs
* Time between API Gateway receiving a request and returning a response.
  * Latency metric
* Time batween API Gateway relaying a request to the backend
and receiving a response.
  * Integration Latency metric
* Number of requests served from the backend in a given period,
when API caching is enable.
  * CacheMissCount
* Number of requests served from the API cache in a given period.
  * CacheHitcount