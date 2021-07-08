# Stacks and Queues.

![](https://4cawmi2va33i3w6dek1d7y1m-wpengine.netdna-ssl.com/wp-content/uploads/2018/07/Computer-science-fundamentals_6.1.png)

### Stacks :
### Definition :
###### a stack is a linear data structure that respects the principal of LIFO “Last In First Out” it means that the last element that was entered into the stack will be the first element to get out or the principal of FIFO “Fist In First Out”which means first in first out so the first element entered to the stack will be the first element that gets out, it’s used to model real world problems and it has tow main operations pop() which is used to get the first top element in the stack and push() which is used to add an element at the top of the stack along side with other operation like peek and ifEmpty that will discuss later.

### Why we use stacks ?
###### Stacks are used to solve many problems since it mimics the behaviour of many real world problems so it’s used as a model of those problems things like :

* the undo mechanism in the text editors .
* used in compilers in things like storing the recursive calls and in syntax checking.
* used in DFS (Depth First Search) algorithm in graphs.
* used in so many algorithms because it can model a lot of real world problems.


###### Mainly there is two ways to implement a stack either you use arrays or linked lists and in our example we will use linked lists.

`this data structure is already implemented in most of the languages and the implementation sometimes is different from one language to another one , but for the sake of understanding the mechanism of it, we will implement it with it’s operation.`

![](https://res.cloudinary.com/practicaldev/image/fetch/s--EqU39YY0--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://dev-to-uploads.s3.amazonaws.com/i/hrglmwtitdfyv98qwb7r.png)

#### Stacks and Complexity :
###### The following operations push , pop, peek,isFull,isEmpty all has a O(1) time complexity cause they all depends on a simple instructions but if we want to do something like search an element that will take O(n) time complexity since we have to pull every element and put it back in order to loop over all the elements.

### Queues :
### Definition :
###### A Queue is a linear data structure that models a real world queue with tow main operations dequeue and enqueue , the queue is similar to the stack but it has tow entry's for the operations one entry for enqueuing elements (from the end) and the other will be for dequeuing elements (from the front) so that the queue will follow the principal of FIFO (First In First Out) in a way that the first added element is the first accessed.

#### Why we use Queues ?
###### Queues can be used to model many real world problems like :

* waiting lines .
* request in web sites to know which client should be served.
* BFS (Breadth First Search) in graphs.
* keep track of the added elements.
* manage shared resources between some entities like CPU processes.
* asynchronous data transfer.