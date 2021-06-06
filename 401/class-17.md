# Review, Research, and Discussion

1. Describe “The Cloud”

A cloud is basically servers that can be accessed over the internet, along with their software and database. By using cloud computing; users and companies don't have to manage the physical server themselves or run software applications on their own machines. 

2. What is a container (as it relates to computers and servers)?

 are packages of software that contain all of the necessary elements to run in any environment. In this way, containers virtualize the operating system and run anywhere, from a private data center to the public cloud or even on a developer's personal laptop.

3. What is auto-scaling?

is a method used in cloud computing that dynamically adjusts the amount of computational resources in a server farm - typically measured by the number of active servers - automatically based on the load on the farm. 

4. What is bandwidth?

is the maximum rate of data transfer across a given path. Bandwidth may be characterized as network bandwidth, data bandwidth, or digital bandwidth.

5. How do cloud providers compute service costs?

They start by calculating costs for network hardware, network infrastructure maintenance, and labor. These expenses are added together and then divided by the number of rack units a business will need for its IaaS cloud.

# Vocabulary Terms
**Server Instances:** An instance is a single copy of the software running on a single physical or virtual server. If you run two copies of the software on the same physical or virtual server, that counts as two instances. When you run two copies of the software on two different physical or virtual servers, that also counts as two instances.

**Containers:** are packages of software that contain all of the necessary elements to run in any environment. In this way, containers virtualize the operating system and run anywhere, from a private data center to the public cloud or even on a developer's personal laptop.

**Cloud Services:** are services available via a remote cloud computing server rather than an on-site server. These scalable solutions are managed by a third party and provide users with access to computing services such as analytics or networking via the internet.

**Cloud Architecture:** refers to the various components in terms of databases, software capabilities, applications, etc. engineered to leverage the power of cloud resources to solve business problems. Cloud architecture defines the components as well as the relationships between them.

**AWS:** Amazon Web Services is a subsidiary of Amazon providing on-demand cloud computing platforms and APIs to individuals, companies, and governments, on a metered pay-as-you-go basis.

**EC2/Beanstalk vs Heroku:**  EC2/Beanstalk is an Infrastructure as a Service product (IaaS), while Heroku is a Platform as a Service (PaaS) product. The main difference is that Heroku’s pricing takes exponential price jumps as one adds common additional features, e.g., auto-scaling, where-as AWS pricing is fairly linear. On the other hand, Heroku is generally simpler to get up and running as AWS has a fairly steep initial learning curve.

# Preparation Materials

## AWS S3:
Amazon Simple Storage Service (Amazon S3) is an object storage service that offers industry-leading scalability, data availability, security, and performance. Amazon S3 provides easy-to-use management features so you can organize your data and configure finely-tuned access controls to meet your specific business, organizational, and compliance requirements. 

**Benefits**
1. Industry-leading performance, scalability, availability, and durability.
2. Wide range of cost-effective storage classes.
3. Unmatched security, compliance, and audit capabilities.
4. Easily manage data and access controls.
5. Query-in-place and process on-request.
6. Most supported cloud storage service.

**Use cases**
1. Backup and restore
2. Disaster recovery (DR)
3. Archive
4. Data lakes and big data analytics
5. Hybrid cloud storage
6. Cloud-native applications

## AWS Lambda:
AWS Lambda is a serverless computing service provided by Amazon Web Services (AWS). Users of AWS Lambda create functions, self-contained applications written in one of the supported languages and runtimes, and upload them to AWS Lambda, which executes those functions in an efficient and flexible manner.

**NOTE:**
The concept of “serverless” computing refers to not needing to maintain your own servers to run these functions. AWS Lambda is a fully managed service that takes care of all the infrastructure for you. 

**Benefits**
1. No servers to manage
2. Continuous scaling
3. Cost optimized with millisecond metering
4. Consistent performance at any scale
5. Pay per use

**Disadvantages**
1. Cold start time
2. Function limits
3. Not always cost-effective
4. Limited number of supported runtimes


**Use cases**
1. Data processing
2. Real-time file processing
3. Real-time stream processing
4. Machine learning
5. Backends
6. Web applications
7. IoT backends
8. Mobile backends

# Content Delivery Network (CDN)

![cdn](https://softloom.com/wp-content/uploads/2019/04/cmn_en_fig_services_network_cdn_01.png)

is a geographically distributed group of servers that work together to provide fast delivery of Internet content. A CDN allows for the fast transfer of data needed for loading Internet content including HTML pages, javascript files, stylesheets, images, and videos.

it reduces the distances between the users and server providing the content, by implementing content delivery network endpoints in as many locations possible.