# Amazon SQS Batch Actions<a name="sqs-batch-api-actions"></a>

To reduce costs or manipulate up to 10 messages with a single action, you can use the following actions:

+ `[SendMessageBatch](http://docs.aws.amazon.com/AWSSimpleQueueService/latest/APIReference/API_SendMessageBatch.html)`

+ `[DeleteMessageBatch](http://docs.aws.amazon.com/AWSSimpleQueueService/latest/APIReference/API_DeleteMessageBatch.html)`

+ `[ChangeMessageVisibilityBatch](http://docs.aws.amazon.com/AWSSimpleQueueService/latest/APIReference/API_ChangeMessageVisibilityBatch.html)`

You can take advantage of batch functionality using the Query API, or an AWS SDK that supports the Amazon SQS batch actions\.

**Note**  
The total size of all messages that you send in a single `SendMessageBatch` call can't exceed 262,144 bytes \(256 KB\)\.  
You can't set permissions for `SendMessageBatch`, `DeleteMessageBatch`, or `ChangeMessageVisibilityBatch` explicitly\. Setting permissions for `SendMessage`, `DeleteMessage`, or `ChangeMessageVisibility` sets permissions for the corresponding batch versions of the actions\.  
The Amazon SQS console doesn't support batch actions\.


+ [Enabling Client\-Side Buffering and Request Batching](sqs-client-side-buffering-request-batching.md)
+ [Increasing Throughput using Horizontal Scaling and Action Batching](sqs-throughput-horizontal-scaling-and-batching.md)