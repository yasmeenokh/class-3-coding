# Review, Research, and Discussion

1. What is the benefit of transforming data into packets?

Packets are intended to transfer data reliably and efficiently. Instead of transferring a large file as a single block of data, sending smaller packets helps ensure each section is transmitted successfully. If a packet is not received or is "dropped," only the dropped packet needs to be resent.

2. UDP is often referred to as a connectionless protocol. Why is this?

 No connection needs to be established between the source and destination before you transmit data. UDP does not have a mechanism to make sure that the payload is not corrupted. As a result, the application must take care of data integrity all by itself.

**UDP** (User Datagram Protocol) is a communications protocol that is primarily used for establishing low-latency and loss-tolerating connections between applications on the internet. It speeds up transmissions by enabling the transfer of data before an agreement is provided by the receiving party.

3. Can a socket server application have multiple socket connections?

A server socket listens on a single port. ... Multiple connections on the same server can share the same server-side IP/Port pair as long as they are associated with different client-side IP/Port pairs, and the server would be able to handle as many clients as available system resources allow it to.

4. Can a socket connection application be connected to multiple socket servers?
5. Can an application be both a socket server and a socket connection?

# Vocabulary Terms

**Observer Pattern:** is a software design pattern in which an object, named the subject, maintains a list of its dependents, called observers, and notifies them automatically of any state changes, usually by calling one of their methods.

**Listener:** An event listener is a procedure or function in a computer program that waits for an event to occur

**Event Handler:** scripts that are automatically executed when an event occurs. Event handlers are embedded in documents as attributes of HTML tags to which you assign JavaScript code to execute.

**Event Driven Programming:** s when a program is designed to respond to user engagement in various forms. It is known as a programming paradigm in which the flow of program execution is determined by “events.” Events are any user interaction, such as a click or key press, in response to prompt from the system.

**Event Loop:** continuously checks the call stack to see if there's any function that needs to run. While doing so, it adds any function call it finds to the call stack and executes each one in order.

**Event Queue:** s a repository where events from an application are held prior to being processed by a receiving program or system. Event queues are often used in the context of an enterprise messaging system.

**Call Stack:** is a mechanism for an interpreter (like the JavaScript interpreter in a web browser) to keep track of its place in a script that calls multiple functions — what function is currently being run and what functions are called from within that function, etc.

**Emit/Raise/Trigger:** in event-driven programming, emit sends a message to trigger a response and raise an event

**Subscribe:** The subscriber function defines how to obtain or generate values or messages to be published. To execute the observable you have created and begin receiving notifications, you call its subscribe() method, passing an observer. This is a JavaScript object that defines the handlers for the notifications you receive.

**database:**an organized collection of data, generally stored and accessed electronically from a computer system

# Preparation Materials

### OSI Model: 
**Layers:**
1. Application layer: which is used by network applications (like http/https), these protocols form application layer, which is the basis of the network services. 

2. presentation layer: which receives data from the application layer, in the form of a characters and numbers. presentation layer converts this data into a binary computer language. it reduces the amount of space needed to store data by compression; which helps transmitting the date faster. before compression the data is encrypted and in the server side it is decrypted.

3. session layer: sets up and manages connections (authentication, authorization)

***THESE THREE LAYERS ARE PERFORMED BY THE WEB BROWSER***

4. transport layer : controls the segmentation, flow control, error control. after segmentation each segment contains a source and a destination number. Flow control; controls the amount of data being transmitted. 

* it has two protocols: TCP which offers connection oriented transmission. and  UDP and which offers connectioless transmission.

![vs](http://www.homenethowto.com/wp-content/uploads/table-tcp-udp.png)

5. network layer : receives data form the transport layer. it's data units are called packets, it works on logical addressing , routing, and path determination.

6. Date link layer : receives data form the network layer. it is responsible for physical addressing. it controls how is data placed and received.

7. physical layer : converts the previous binary in signals, 


### WebSocket Vs Socket.IO

**WebSocket** is the communication Protocol that provides bidirectional communication between the Client and the Server over a TCP connection; WebSocket remains open all the time, so they allow real-time data transfer. When clients trigger the request to the server, it does not close the connection on receiving the response; it rather persists and waits for the Client or server to terminate the request.

**Socket.IO** is a library that enables real-time and full-duplex communication between the Client and the Web servers. It uses the WebSocket protocol to provide the interface. Generally, it is divided into two parts; both WebSocket vs Socket.io are event-driven libraries.