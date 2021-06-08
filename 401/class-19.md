# Review, Research, and Discussion

1. Describe the similarities between AWS API Gateway + Lambda functions and an ExpressJS Server

 both will handle http request endpoints, a request will be received from the use at a specific end point the method(in express or using lambda) then a handler will be called.
 
2. List the AWS Database offerings and talk about the pros and cons of each
**Amazon Relational Database**:  is a distributed relational database service by Amazon Web Services. It is a web service running "in the cloud" designed to simplify the setup, operation, and scaling of a relational database for use in applications.

**Amazon DynamoDB** is a fully managed proprietary NoSQL database service that supports key–value and document data structures and is offered by Amazon.com as part of the Amazon Web Services portfolio. DynamoDB exposes a similar data model to and derives its name from Dynamo, but has a different underlying implementation.

3. What’s the difference between a FIFO and a standard queue?

FIFO queues have essentially the same features as standard queues, but provide the added benefits of supporting ordering and exactly-once processing. FIFO queues provide additional features that help prevent unintentional duplicates from being sent by message producers or from being received by message consumers.

4. How can the server be assured a message was properly received?

A Message Authentication Code (MAC) is a tag attached to a message to ensure the integrity and authenticity of the message. It is derived by applying a MAC algorithm to a message in combination with a secret key.

# Vocabulary Terms

**Serverless API:** is a cloud computing execution model where the cloud provider dynamically manages the allocation and provisioning of servers. A serverless application runs in stateless compute containers that are event-triggered, ephemeral (may last for one invocation), and fully managed by the cloud provider.

**Triggers:** are what cause a function to run. A trigger defines how a function is invoked and a function must have exactly one trigger. Triggers have associated data, which is often provided as the payload of the function.

**Dynamo vs Mongo:**

***Amazon DynamoDB:*** is a fully managed proprietary NoSQL database service that supports key–value and document data structures and is offered by Amazon.com as part of the Amazon Web Services portfolio. DynamoDB exposes a similar data model to and derives its name from Dynamo, but has a different underlying implementation.

***MongoDB:*** is a source-available cross-platform document-oriented database program. Classified as a NoSQL database program, MongoDB uses JSON-like documents with optional schemas. MongoDB is developed by MongoDB Inc. and licensed under the Server Side Public License.

**Dynamoose vs Mongoose:**
***Dynamoose:*** is Sponsored by Dynobase, Dynobase helps you accelerate your DynamoDB workflow with code generation, faster data exploration, bookmarks and more.

***Mongoose:*** is a MongoDB object modeling tool designed to work in an asynchronous environment. Mongoose supports both promises and callbacks.

# Preview
## SQS and SNS Basics
 Simple Notification Service and Simple Queue Service.

 ![sqsVsSNS](https://res.cloudinary.com/practicaldev/image/fetch/s--0qV6AkDT--/c_imagga_scale,f_auto,fl_progressive,h_900,q_auto,w_1600/https://dw71fyauz7yz9.cloudfront.net/video-upload__c8bc44f83cd41222de8ae55b55c63ef2/thumbs-video-upload__c8bc44f83cd41222de8ae55b55c63ef2-00001.png)
 

 **SNS:** faster and more flexible, we send a message to many users at the same time, uses the push mechanism, publish and subscriber concept. it is a managed messaging service for system-to-system and application-to-person communications.

 **SQS:** send a message for one a user at a time, queue concept (FIFO), when a msg is sent it acts as a buffer message is stored on the queue, and after the user receives the message it it removes it from the queue, it uses the pull mechanism. it sends messages through web applications for communications over the internet.

**NOTE**
Pulling inherently introduces some latency in message delivery in SQS unlike SNS where messages are immediately pushed to subscribers.

