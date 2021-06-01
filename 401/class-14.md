# Review, Research, and Discussion

1. **What’s the difference between a FIFO and a standard queue?**
Standard queues guarantee that a message is delivered at least once and duplicates can be introduced into the queue. FIFO queues ensure a message is delivered exactly once and remains available until a consumer processes and deletes it; duplicates are not introduced into the queue.

2. **How can the server be assured a message was properly received?**
By using the message Queue to save the message until the user is connected and get the message

3. **What classic design pattern is best represented by event driven programming?**
An Event-Driven Architecture is a software architecture paradigm promoting the production, detection, consumption of, and reaction to events. Examples of events include the taking of a measurement, the pressing of a button, or the swiping of a credit card.

4. **How do you test an event driven system?**
Effective logging is critical in any application architecture, but when it comes to event-driven application architecture, it’s essential. Thus, the only way to really figure out what’s going on in terms of application behavior is to make sure that all information relevant to application performance is being logged, with timestamping being the no-brainer requirement.

# Vocabulary Terms

**FIFO Queue:** is a method for organizing the manipulation of a data structure (often, specifically a data buffer) where the oldest (first) entry, or "head" of the queue, is processed first.

![fifo](https://upload.wikimedia.org/wikipedia/commons/thumb/5/52/Data_Queue.svg/1200px-Data_Queue.svg.png)

**Pub/Sub:** is an asynchronous messaging service that decouples services that produce events from services that process events.it can be used as messaging-oriented middleware or event ingestion and delivery for streaming analytics pipelines.

# Preparation Materials

## SNS vs SQS Comparison
![vs](https://miro.medium.com/max/1004/1*mdUPKzrfJFuXa4d43KhKUQ.png)

When we have one event and you want to distributed to multiple users or receivers.

**SNS**: (Simple Notification Service) is a distributed publish-subscribe system. Messages are pushed to subscribers as and when they are sent by publishers to SNS. 

**SQS**: (Simple Queue Service) is distributed queuing system. Polling inherently introduces some latency in message delivery in SQS unlike SNS where messages are immediately pushed to subscribers.