# Knowlege check

1. You're setting up an Amazon SQS queue as an event source to a Lambda function that takes an average of 3 minutes to process each message. Select the most appropriate configuration options as a starting point.

* Set the batch size to 4 or lower.
* Set the visibility timeout on the queue to 6x the function timeout.
* configure a dead-letter queue

2. Which of these statements about AWS Step Functions States Languague are true?

* Task and Parallel states can have a field named Retry. An individual retrier
represents certain number of retries.
* You can use a Retry or Catch field to handle timeouts.
* The Amazon States Language defines a set of built-in strings that name 
well-known errors, all beginning with the States. prefix.
* The reserved name States. All is a wildcard that matches any error name.

3. Match the X-Ray feature on the left to the scenario on the right

* Costomers have reported issues using a service, and you need a quick
sense of status.
  * Service graph
* You've identified failures at an integration point and want to review
individual requests.
  * Traces
* You need a more granular breackout of the work done in a request to resolve
the issues.
  * Subsegments
* You want to be able to group traces across application operations to compare performance
  * Annotations