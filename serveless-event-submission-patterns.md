# Knowledge check

1. The business has asked you to build a résumé submission service to connect to their job listing webpage. The service needs to integrate with their legacy system to match the submissions to existing candidates. Very high bursts of traffic are expected when a new job is posted, and you don't control the UI layer.  The order in which the resumes are processed is not critical. What serverless patterns make the most sense? Select all that apply.

Solution

*  Use An SQS queue to recelve and respond to requests comming through API Gateway.
*  Use a standard SQS queue as an event source for lambda.
*  Use a Lambda function to initiate a Step Functions flow that orchestrates 
the integration with the legacy system.



2. Match the scenario with the suggested method for handling status updates

* You have an internal service and need to minimize calls between client and service
  * Trusted Webhooks
* You have an app with rapidly changing, high volumes of data.
  * WebSockets with AWS AppSync
* You want to  implement a serveless approach with minimal rework to existing services.
  * Client polling
* You want a two-way, persistent connection between the client and the backing service.
  * WebSockets with API Gateway

3. Which of these scenarios points to using the claim check pattern?

* You have an API endpoint connected to an SQS queue that clients use to post
high-resolution video files for processing by a Lambda function.

4. Select the scenarios where you might select Kinesis Data Firehose for data processing.

* You want to ingest a very high volume of data and store it to Amazon Redshift.
* You want to ingest a very high volume of data, transform its format, and 
store it to Amazon S3.
* You want to simplify retry handling on streaming data, and order of records
in the stream is not critical.