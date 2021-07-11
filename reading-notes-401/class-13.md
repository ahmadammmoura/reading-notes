## What is Socket.IO?

###### Socket.IO was created in 2010. It was developed to use open connections to facilitate realtime communication, still a relatively new phenomenon at the time.

###### Socket.IO allows bi-directional communication between client and server. Bi-directional communications are enabled when a client has Socket.IO in the browser, and a server has also integrated the Socket.IO package. While data can be sent in a number of forms, JSON is the simplest.

###### To establish the connection, and to exchange data between client and server, Socket.IO uses Engine.IO. This is a lower-level implementation used under the hood. Engine.IO is used for the server implementation and Engine.IO-client is used for the client.

![img](https://images.ctfassets.net/ee3ypdtck0rk/1Lj7lbqX54WCiHI2uVVL3x/fcf8b0a411fd25bef518f929af11f1a3/socketio-engioneio-interaction.png)

## Socket.IO – In action


###### A popular way to demonstrate the two-way communication Socket.IO provides is a basic chat app (we talk about some other use cases below). With sockets, when the server receives a new message it will send it to the client and notify them, bypassing the need to send requests between client and server. A simple chat application shows how this works.

![img](https://images.ctfassets.net/ee3ypdtck0rk/27G4lHu2Vj0Cm0CUC2x5p7/0183903c567558ca5b145b3987317c2f/socket-io-two-way-communication.png)

### Review, Research, and Discussion 

* What is the benefit of transforming data into packets?
  - Packets are the basic units of communication over a TCP/IP network. Devices on a TCP/IP network divide data into small pieces, allowing the network to accommodate various bandwidths, to allow for multiple routes to a destination, and to retransmit the pieces of data which are interrupted or lost

* UDP is often refereed to as a connectionless protocol. Why is this?

  - UDP is a connectionless protocol. It is known as a datagram protocol because it is analogous to sending a letter where you don't acknowledge receipt. Examples of applications that use connectionless transport services are broadcasting and tftp .


* Can a socket server application have multiple socket connections?

  - Multiple connections on the same server can share the same server-side IP/Port pair as long as they are associated with different client-side IP/Port pairs, and the server would be able to handle as many clients as available system resources allow it to.

## terms 
* Observer Pattern => The observer pattern is a software design pattern in which an object, named the subject, maintains a list of its dependents, called observers, and notifies them automatically of any state changes, usually by calling one of their methods.
* Listener => The event listener code is a callback function that takes a parameter for the data and handles it. Node. js has an EventEmitter class that can be extended by a new class that we create to emit events that can be listened to by event listeners.
* event handler => js EventEmitter. Node. js allows us to create and handle custom events easily by using events module. Event module includes EventEmitter class which can be used to raise and handle custom events.
* Event Driven Programming => In computer programming, event-driven programming is a programming paradigm in which the flow of the program is determined by events such as user actions (mouse clicks, key presses), sensor outputs, or message passing from other programs or threads.

