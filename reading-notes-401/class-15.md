## What is Event Driven Architecture (EDA)?

###### Most of the nodejs core modules like Http, fs, timers are built around event-driven architecture and we can, of course, use this architecture to our advantage in the code we write. and this concept of events in nodejs is very simple.

###### In nodejs, there are certain Objects called events emitters that emit named events as soon as something important happens in the app like a request hitting a server or a timer expiring, or a file finished to read. These events are picked up by and event listeners that we developers set up which will fire up callback functions that are attached to each listener. i.e, on one hand, we have event emitters, on the other hand, we have event listeners that will react by calling callbacks.

###### Let's briefly look at an example. So when we want to create a server, we use the create server method

```
 const server = http.createServer();

 server.on('request', (req, res) => {
  console.log('request receved');
  res.end('request receved');
 });

```

###### This 'server.on' is actually how we create a listener and in this case for the request event. So let's say we have our server running and a new request is made. The server acts as an emitter and will automatically emit an event called request each time that a request hits the server then the callback function attached to this listener will be called which will send some data back to the clients. It works this way because behind the scenes the server is an instance of the event-emitter class and this event-emitter logic is called the observer pattern in javascript and is quite a popular pattern. The idea is there is an observer, in this case, the event listener which keeps observing the subjects that will eventually emit the event that the listener is waiting for. So let's look at some examples.

###### To work with the built-in node events we need to require the events module and from that, we require the event emitter class.

```

   const EventEmitter = require('events');

   const myEmitter = new EventEmitter();

```

###### Event emitters can emit named events and we can then subscribe to these events by listening to these events and reacting accordingly just like setting an event listener on a button and listening for any click on the button. Let's emits an event called 'order'.


```
   const EventEmitter = require('events');

   const myEmitter = new EventEmitter();

   myEmitter.on('order', () => {
    console.log('order has been placed');
   })

   myEmitter.emit('order')

```


###### Here we emit a named event called 'order' and attached a listener to this event, and a callback function that will log 'order has been placed'.

###### We can also set up multiple listeners for the same events

```

   const EventEmitter = require('events');

   const myEmitter = new EventEmitter();

   myEmitter.on('order', () => {
    console.log('an order has been placed');
   });

   myEmitter.on('checkout', () => {
    console.log('payment has been made');
   });

   myEmitter.emit('order')
```

###### This is the observer pattern where

```
myEmitter.emit('order')
```

###### is the object that emits the event and

```
    myEmitter.on('order', () => {
    console.log('an order has been placed');
   });

    myEmitter.on('checkout', () => {
    console.log('payment has been made');
   });
```

###### are observers that observe the emitter and wait until the emitter emits an event.

###### We can also pass an additional argument to the events listeners

```

   const EventEmitter = require('events');

   const myEmitter = new EventEmitter();

   myEmitter.on('order', (itemNo) => {
    console.log(`an order has been placed on item ${itemNo}`);
   });


   myEmitter.emit('order', 10)

```
###### logging this to the console yields

```
 an order has been placed on item 10
```

###### Finally, you will also observe that multiple listeners for the same events are log synchronous one after the other that is their normal behavior. Next up we will look at streams in action feel free to check the documentation for more details about events in nodejs.

#### Review, Research, and Discussion

1. What’s the difference between a FIFO and a standard queue?
  * Standard queues provide at-least-once delivery, which means that each message is delivered at least once. FIFO queues provide exactly-once processing, which means that each message is delivered once and remains available until a consumer processes it and deletes it.
2. How can the server be assured a message was properly received?

3. What classic design pattern is best represented by event driven programming?
  * The singleton pattern is used to limit creation of a class to only one object. This is beneficial when one (and only one) object is needed to coordinate actions across the system. There are several examples of where only a single instance of a class should exist, including caches, thread pools, and registries.

4. How do you test an event driven system?

  * Basically, an event-driven application architecture is one in which services (aka functions) within an application input data and output data via messages that are stored in a message queue. This differs from a synchronous architecture, in which data is passed straight to a service by making a direct call.

  ### Term

  * FIFO Queue = > The operations of a queue make it a first-in-first-out (FIFO) data structure. In a FIFO data structure, the first element added to the queue will be the first one to be removed. ... A queue is an example of a linear data structure, or more abstractly a sequential collection.
  * Pub/Sub = > Pub/Sub enables you to create systems of event producers and consumers, called publishers and subscribers. Publishers communicate with subscribers asynchronously by broadcasting events, rather than by synchronous remote procedure calls (RPCs).