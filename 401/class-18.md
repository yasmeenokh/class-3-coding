# Review, Research, and Discussion

1. What are serverless functions?

Serverless computing is a cloud computing execution model in which the cloud provider allocates machine resources on demand, taking care of the servers on behalf of their customers.

2. If you were to create a system that emulated Lambda functions, how would you do it?

I will use an event driven functions, that needs to be executed only when needed or called for example in JavaScript I will use event listener to listen on certain event by the user and upon that event the function is run.

3. Describe how a CDN works

To minimize the distance between the visitors and your website’s server, a CDN stores a cached version of its content in multiple geographical locations (a.k.a., points of presence, or PoPs). Each PoP contains a number of caching servers responsible for content delivery to visitors within its proximity.

# Vocabulary Terms

**Serverless Functions:** is a programmatic function written by a software developer for a single purpose. It's then hosted and maintained on infrastructure by cloud computing companies. These companies take care of code maintenance and execution so that developers can deploy new code faster and easier.

**Cloud Storage:** Cloud storage is a model of computer data storage in which the digital data is stored in logical pools, said to be on "the cloud". The physical storage spans multiple servers, and the physical environment is typically owned and managed by a hosting company.

**CDN:** is a geographically distributed group of servers that work together to provide fast delivery of Internet content. A CDN allows for the fast transfer of data needed for loading Internet content including HTML pages, javascript files, stylesheets, images, and videos.

# Preview
### Amazon API Gateway
#### What is Amazon API Gateway?
Amazon API Gateway is a managed service that allows developers to define the HTTP endpoints of a REST API or a WebSocket API and connect those endpoints with the corresponding backend business logic. It also handles authentication, access control, monitoring, and tracing of API requests.

- Many Serverless applications use Amazon API Gateway, which conveniently replaces the API servers with a managed serverless solution.

#### How does API Gateway work?
* API Gateway sits between the backend services of your API and your API’s users, handling the HTTP requests to your API endpoints and routing them to the correct backends. It provides a set of tools that help you manage your API definitions and the mappings between endpoints and their respective backend services. It can also generate API references from your definitions and make them available to your users as API documentation.

### DynamoDB

#### What is DynamoDB?

**DynamoDB is a hosted NoSQL database offered by Amazon Web Services (AWS). It offers:**

* reliable performance even as it scales.
* a managed experience, so you won’t be SSH-ing into servers to upgrade the crypto libraries.
* a small, simple API allowing for simple key-value access as well as more advanced query patterns.
* DynamoDB is a particularly good fit for the following use cases:
* Applications with large amounts of data and strict latency requirements.
* As your amount of data scales, JOINs and advanced SQL operations can slow down your queries. With DynamoDB, your queries have predictable latency up to any size, including over 100 TBs!
* Serverless applications using AWS Lambda.
* AWS Lambda provides auto-scaling, stateless, ephemeral compute in response to event triggers. DynamoDB is accessible via an HTTP API and performs authentication & authorization via IAM roles, making it a perfect fit for * building Serverless applications.
* Data sets with simple, known access patterns.
* If you’re generating recommendations and serving them to users, DynamoDB’s simple key-value access patterns make it a fast, reliable choice.