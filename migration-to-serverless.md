# Migration to Serveless

Migration questions to answer:

What does this application do, and how are its components organized?

How can you break your data needs up based on the command query responsibility (CQRS) pattern?

How does the application scale, and what components drive the capacity you need?

Do you have schedule-based tasks?

Do you have workers listening to a queue?

Where can you refactor or enhance functionality without impacting the current implementation?

**Aplication Load Balancer vs. API Gateway for directiong traffic to serveless targets**

  
           Aplication Load Balanecer          |   Amazon API Gateway
:____________________________________________ | ________________________________________:
| Easier to transitor existing computer stack | Good for build REST API and
| where you are already using an              | Ingrating with other services and
| Application Load Balancer                   | Lambda functions
______________________________________________________________________________________
| Supports authorization via OIDC-capable     | Suports authorization via AWS identity
| providers, include Amazon Cognito user      | and Access Management (IAM), Amazon
| pools                                       | Cognito, and Lambda authorizers
______________________________________________________________________________________
| Charged by the hour, based on Load          | Charged based on requests served
| Balancer Capacity Units                     | 
______________________________________________________________________________________
| May be more cost-effective for a steady     | May be more cost-effective for spiky
| stream of traffic                           | patterns
______________________________________________________________________________________
|                                             | Additional features for API Management:
|                                             |  
|                                             | * Export SDK fro clients
|                                             | * Use throttling and usage plans to control access
|                                             | * Maintain multiple versions of an API
|                                             | * Canary deployments
______________________________________________________________________________________



# Knowledge ckeck

Which of these reflect discussions that will help you select a good serverless migration strategy? Select all that apply. 

* "Let's talk about where we want to be as a development organization next
year and the skills we need out developers to grow to get there"
* "Let's look at what it would take to adopt a 'serverless first' strategy for new
features only".
* "Do we have any 'low-hanging fruit' like cron jobs or workers listengin to a
queue that we could experiment with?""
* "Who owns the data and who uses it?""
