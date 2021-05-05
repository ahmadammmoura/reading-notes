# Introduction :

### How the Web Works ?
### You can find the answer of this question in this infographic photo :


![img](https://infographiclist.files.wordpress.com/2012/11/howdoesinternetwork_4fdf33a6a527b.jpg)


# What is REST?

![vv](https://api.zestard.com/wp-content/uploads/2015/12/What-is-Rest-API-02-1.jpg)


### Learn about how to design web services using the REST paradigm
## REpresentational State Transfer
### REST, or REpresentational State Transfer, is an architectural style for providing standards between computer systems on the web, making it easier for systems to communicate with each other. REST-compliant systems, often called RESTful systems, are characterized by how they are stateless and separate the concerns of client and server. We will go into what these terms mean and why they are beneficial characteristics for services on the Web.

## Separation of Client and Server
### In the REST architectural style, the implementation of the client and the implementation of the server can be done independently without each knowing about the other. This means that the code on the client side can be changed at any time without affecting the operation of the server, and the code on the server side can be changed without affecting the operation of the client.

### As long as each side knows what format of messages to send to the other, they can be kept modular and separate. Separating the user interface concerns from the data storage concerns, we improve the flexibility of the interface across platforms and improve scalability by simplifying the server components. Additionally, the separation allows each component the ability to evolve independently.

### By using a REST interface, different clients hit the same REST endpoints, perform the same actions, and receive the same responses.

## Statelessness
### Systems that follow the REST paradigm are stateless, meaning that the server does not need to know anything about what state the client is in and vice versa. In this way, both the server and the client can understand any message received, even without seeing previous messages. This constraint of statelessness is enforced through the use of resources, rather than commands. Resources are the nouns of the Web - they describe any object, document, or thing that you may need to store or send to other services.

### Because REST systems interact through standard operations on resources, they do not rely on the implementation of interfaces.

### These constraints help RESTful applications achieve reliability, quick performance, and scalability, as components that can be managed, updated, and reused without affecting the system as a whole, even during operation of the system.

### Now, we’ll explore how the communication between the client and server actually happens when we are implementing a RESTful interface.

## Communication between Client and Server
### In the REST architecture, clients send requests to retrieve or modify resources, and servers send responses to these requests. Let’s take a look at the standard ways to make requests and send responses.

## Making Requests
### REST requires that a client make a request to the server in order to retrieve or modify data on the server. A request generally consists of:

### an HTTP verb, which defines what kind of operation to perform
### a header, which allows the client to pass along information about the request
### a path to a resource
### an optional message body containing data
### HTTP Verbs

## There are 4 basic HTTP verbs we use in requests to interact with resources in a REST system:

# GET — retrieve a specific resource (by id) or a collection of resources
# POST — create a new resource
# PUT — update a specific resource (by id)
# DELETE — remove a specific resource by id
### You can learn more about these HTTP verbs in the following Codecademy article:

## What is CRUD?
### Headers and Accept parameters
### In the header of the request, the client sends the type of content that it is able to receive from the server. This is called the Accept field, and it ensures that the server does not send data that cannot be understood or processed by the client. The options for types of content are MIME Types (or Multipurpose Internet Mail Extensions, which you can read more about in the MDN Web Docs.

