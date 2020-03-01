# AWS DynamoDB Self-check

1. Which of the following are true of DynamoDB tables?

* Read and write capacity are managed independently.
* All item must have a partition key. The unique primary key
includes a partition key and optional sort key.
* Tables can scale to any data volume.

2. Local secondary indexes can only be defined at the time
of base table creation - they cannot be deleted without deleting 
the base table. True ou false?

* True

3. With of following workload characteristics might be a good fit 
for DynamoDB?

* Tha data is "hot"- serving real-time, transactional, operational,
interactive uses.
* The session states for your application need to be stored off of
your instances.
* The data must be stored in a highly available, durable, and highly scalable manner.

4.  Which of the following statements about DynamoDB Strems is FALSE?

* DynamoDB Streams is compatible by default with the Kinessis Client Library.

5. Which statements about consistency are true?

* Strongly consistent reads can be made via VPC endpoint.
* Local and global secondary indexes both support eventually consistent reads.
* DynamoDB Accelerator (DAX) passes strongly consistent read through but does not 
cache them.

6. Which of the following is a commonly recommended serverless pattern for 
aging out DynamoDB data to a cold storage tier?

* Enable DynamoDB Streams and use TTL to expire old items. A Lambda funcions is 
triggered on the change and writes the deleted item data into S3 via Kinesis Firehose.

7. Which of the following are parameters to DynamoDB Auto Scaling?

* Minimum capacity
* Maximum Capacity
* Target utilization
