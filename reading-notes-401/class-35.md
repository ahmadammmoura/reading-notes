## What is a graph?

###### A graph is a non-linear data structure that helps us describe entities and it's relationships to other entities.

###### For example, you may use the graph data structure to represent friends in a social media website.

![img](https://res.cloudinary.com/practicaldev/image/fetch/s--qs2XpdKK--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://dev-to-uploads.s3.amazonaws.com/uploads/articles/u64qqu9pbx6vxtozssev.png)

###### Graphs are very useful because they can describe a great deal of problems we have in the real world.

###### But before we move on, we have to break down the graph even more.

### Essential Terminology

![img](https://res.cloudinary.com/practicaldev/image/fetch/s--uZMgTEcI--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://dev-to-uploads.s3.amazonaws.com/uploads/articles/gnscwjgmf8pyl8vtqi3h.png)

###### A graph (V,E) is made out of two parts:

* Collection of Vertices (V): Your basic node (i.e user, place, event, etc...)
* Collection of Edges (E): They represent the relationships between nodes. In mathematical terms, they can be represented by coordinates of two nodes (u,v).

###### We can represent the graph above by:

```
V = {0, 1, 2, 3, 4}
E = {
     (0,1), (0,4), (1,0), 
         (1,2), (1,3), (1,4),
     (2,1), (2,3),
     (3,1), (3,2), (3,4),
     (4,0), (4,1), (4,3),
    }
G = {V, E} // A graph is a collection of vertices and edges

```


#### Types of Graphs
###### While researching, I've come across many different types of graphs, but to save you time I've narrowed it down to two basic types:

1. Directed Graph
2. Simple Graph


### Directed Graphs

![image](https://res.cloudinary.com/practicaldev/image/fetch/s--AElmaZJ7--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://dev-to-uploads.s3.amazonaws.com/uploads/articles/n5b4ioiirehbu07ibmqi.png)

###### A graph where all edges are directed from one vertex to another vertex is called a directed graph.

###### The connections are not bidirectional, meaning that if we have a connection from A to B, that doesn't mean we have a connection from B to A.

###### But you might ask "Why will we use something like this?"

###### Well, there are many use cases for directed graphs, here are a few:

* Twitter: When you follow someone, that's a direct connection, the other person doesn't need to follow you.
* Flights: You might be able to fly from Paris to London, but there's no guarantee that you can fly from London to Paris.
* Road Networks: Some roads are one-way, others are two-way, you get the gist.

### Simple Graphs

![image](https://res.cloudinary.com/practicaldev/image/fetch/s--76lNEN0K--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://dev-to-uploads.s3.amazonaws.com/uploads/articles/vpfxivuldiskkusmo8sc.png)

###### Graphs that are always two-way connections are called simple graphs. Our first example (at the beginning of the post) was a simple graph (also called undirected graphs).

###### PS. Through out this post, whenever I say graphs, I'm gonna mean simple graphs.

### Weighted Graphs

![images](https://res.cloudinary.com/practicaldev/image/fetch/s--6Z5aM5ex--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://dev-to-uploads.s3.amazonaws.com/uploads/articles/2g7av86cqgsegtg9ahra.png)

###### So far we assume that every edge is equal to each other. Unfortunately, life doesn't work that way, the distance between France and Germany is shorter than France and the USA. This is why we add a weight to each edge. A graph with weighted edges is called a weighted graph.

