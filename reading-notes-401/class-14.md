## Introduction to Messages Queues

###### Modern software and system architectures encourage the decoupling of different layers/services in an application's design. These services and/or layers can be web service APIs, database systems, cache proxy servers, serverless functions, etc. Communication between these elements is done by sending data in the form of messages from one point to another, oftentimes asynchronously. In this post, we will look at one of the tools that helps broker messages between the layers and services in these architectures and ensure that messages are transferred at a rate that can be handled by the intended destination service/layer.

### What are message queues?

###### A message queue is a component in a system's architecture that helps buffer and distribute asynchronous requests. As stated earlier, a message is sent in a request from one point to another; for example, from a front-end application to a back-end API. A message is a serialized data construct, mostly in XML or JSON format, and it contains all the information required to perform the requested operation.

![img](https://assets.website-files.com/606cafbbb933c2dd1c48e2ad/60aadc6aa2dde417b772e15c_Message_queues.png)

1. Message queues maintain an internal queue of messages that are distributed on schedule to the intended destination.
2. Messages that cannot be consumed fast enough line up in the queue until the destination service is ready to process more messages.
3. Message queues sit in between two services/layers that need to communicate with one another. The component that makes the request by adding a message to the queue is known as a message producer, while the component that picks up the messages from the queue and does the main processing is known as the message consumer.
4. A message queue arranges messages in a sequence to be delivered to the consumers who can then consume messages from the queue.


## Producers and consumers

###### Message producers create messages which are buffered by the message queue and delivered to the message consumers, who then perform the asynchronous processing on behalf of the producer. Think of this like making an order at a restaurant. You and your friends (message producers) place your orders (message requests) and deliver them to the waiter (message queue) who holds and delivers all the orders to the kitchen (message consumer), where the actual preparation of the meals you ordered takes place.

###### In an architecture that is designed to scale easily, producers and consumers run as separate processes and are often hosted on separate machines.


![img](https://assets.website-files.com/606cafbbb933c2dd1c48e2ad/60aadc9e02355b8e3f63b8b9_Producer_and_consumers.png)

###### Producers and consumers function as independent systems and the only contract that exists between them is the message format with which they are to communicate. The producer must send messages in the format (JSON or XML) and structure expected by the consumer as message queues do not perform message transformation.

###### Producers and consumers are decoupled and exist separately, but the producer has a dependency on the consumer. Most consumers are completely independent components that often only specialize in performing a single task, for example, an email service that receives email requests and its sole responsibility is to send emails to different addresses.

###### In a well-decoupled system, a consumer should know nothing about the producer and only depend on valid messages that the queue delivers to it.

### Advantages of using message queues

###### Now that we understand the responsibility of message queues and how they work with message producers and consumers, let's take a look at some of the advantages of using message queues.

1. Because producers and consumers are independent components, they can be implemented in different languages.

2. By hosting producers and consumers on separate machines and decoupling them, it is easy to scale each side of the message queue separately. You can add more consumers to speed up the rate of processing.

3. They bring about asynchronous processing which ensures that, unlike the typical request/response synchronous pattern, producers can carry on with other tasks after making the request and do not have to wait for a response to be received before doing any other work.

4. They can be used to implement asynchronous processing in a system that was built to be synchronous.


### Term
* Socket :
  - Socket programs are used to communicate between various processes usually running on different systems. It is mostly used to create a client-server environment. This post provides the various functions used to create the server and client program and an example program.

* WebSocket :
  - The WebSocket protocol enables interaction between a web browser (or other client application) and a web server with lower overhead than half-duplex alternatives such as HTTP polling, facilitating real-time data transfer from and to the server.

* Socket.io :
  - Socket.IO is a JavaScript library for realtime web applications. It enables realtime, bi-directional communication between web clients and servers. It has two parts: a client-side library that runs in the browser, and a server-side library for Node. js.

* Client :
- The Clients interface provides access to Client objects.

* Server :
  - The server side programming is the name given to all types of programs which run on the web server

* OSI Model :
- The OSI Model (Open Systems Interconnection Model) is a conceptual framework used to describe the functions of a networking system. The OSI model characterizes computing functions into a universal set of rules and requirements in order to support interoperability between different products and software.

* TCP Model :
  - TCP enables data to be transferred between applications and devices on a network and is uded in the TCP IP model. It is designed to break down a message, such as an email, into packets of data to ensure the message reaches its destination successfully and as quickly as possible.
