# Review, Research, and Discussion

1. What does it mean that web sockets are bidirectional? Why is this useful?

HTTP relies on a client request to receive a response from the server for every exchange,
WebSockets allow for full-duplex bidirectional communication. This enables the server to send real-time updates asynchronously, without requiring the client to submit a request each time. In the context of networked AV and control systems, this allows devices to send and receive continuous streams of data to and from any point on the network.

2. Does socket.io use HTTP? Why?

Even when websockets can be used, the initial connection setup it done over HTTP. Also, a socket.io server will attach to an HTTP server so it can serve its own client code through /socket.io/socket.io.js.

3. What happens when a client emits an event?

if the server have a listener on that event it will provoke it and send the event emitted payload to the listener to use it.

4. What happens when a server emits an event?

send a message to all the connected clients. This code will notify when a user connects to the server.

5. What happens if a client “misses” an event?

the event will not be executed.

6. How can we mitigate this?

# Vocabulary Terms

-----------|-----------------------
Socket     | is one endpoint of a two-way communication link between two programs running on the network. A socket is bound to a port number so that the TCP layer can identify the application that data is destined to be sent to. An endpoint is a combination of an IP address and a port number.
Web Socket | s a computer communications protocol, providing full-duplex communication channels over a single TCP connection.
Socket.io  | is a JavaScript library for realtime web applications. It enables realtime, bi-directional communication between web clients and servers. It has two parts: a client-side library that runs in the browser, and a server-side library for Node.js. Both components have a nearly identical API. 
Client     |
Server     | is a computer that provides data to other computers. It may serve data to systems on a local area network (LAN) or a wide area network (WAN) over the Internet.
OSI Model  | (Open Systems Interconnection Model) is a conceptual framework used to describe the functions of a networking system. The OSI model characterizes computing functions into a universal set of rules and requirements in order to support interoperability between different products and software.
TCP Model  | It stands for Transmission Control Protocol/Internet Protocol. The TCP/IP model is a concise version of the OSI model. It contains four layers, unlike seven layers in the OSI model.
TCP        | is a transport protocol that is used on top of IP to ensure reliable transmission of packets. TCP includes mechanisms to solve many of the problems that arise from packet-based messaging, such as lost packets, out of order packets, duplicate packets, and corrupted packets.
UDP        | (User Datagram Protocol) is a communications protocol that is primarily used for establishing low-latency and loss-tolerating connections between applications on the internet. It speeds up transmissions by enabling the transfer of data before an agreement is provided by the receiving party.
Packets    | is a small segment of a larger message. Data sent over computer networks*, such as the Internet, is divided into packets. These packets are then recombined by the computer or device that receives them.


# Preparation Materials

Socket.io Chat example Sockets have traditionally been the solution around which most real-time chat systems are architected, providing a bi-directional communication channel between a client and a server

Rooms and Namespaces Rooms are part of namespaces where each namespace can be divided into several rooms and a very room handles a certain type of sockets (Join & Leave) it basically works by a socket (user) sends a join request to one of the available rooms and the server joins it in the room (it could need authentication or invitation depending on your application). Rooms are a server-only concept (client does not have access to the list of rooms it has joined).