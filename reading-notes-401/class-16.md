## What are Binary Trees?

![img](https://res.cloudinary.com/practicaldev/image/fetch/s--tzaN3vIP--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://images.fineartamerica.com/images-medium-large-5/upside-down-tree-marty-kugler.jpg)

###### A tree is a data structure that looks like an upside-down tree consisting of nodes. A binary tree is a structure of nodes that each point to no more than two children.

### The Physiology of a Tree

![img](https://i.giphy.com/media/cPg6XJTNxDlhQz8zen/giphy.gif)

###### A tree is a structure composed of nodes that each contains a value or data. The root is a single node located at the top of the tree. It is the start of the tree where nodes point to child nodes connected by branchlets called edges. A subtree, much like a clipping, is a subsection or part of a tree.

![img](https://i.giphy.com/media/TJglzdRKOELC3W12mZ/giphy.gif)

###### The root of this tree is the parent of two child nodes, each either a left or a right child. Two children or sub-trees of a shared parent are siblings. It's possible for a child to also be the parent of two other child nodes further down the branch.

![img](https://i.giphy.com/media/KezoursDTpXWUjG3PO/giphy.gif)

###### As we follow a branch down from a parent node, any other node located down that branch is its descendent. And if we follow a branch upwards from a child node, any node up that branch is an ancestor of the child node.

![img](https://res.cloudinary.com/practicaldev/image/fetch/s--u_8j_5JR--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://thepracticaldev.s3.amazonaws.com/i/xk1qnu5mdxow8a58zzow.png)

###### At the bottom or terminal of a branch is the leaf or external node, which has no children. Nodes that branch further to one or more child nodes are branch or internal nodes.


### Describing a Binary Tree

###### When we describe a binary tree, we can discuss its height or its depth.

![img](https://res.cloudinary.com/practicaldev/image/fetch/s--3-W7PVib--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://thepracticaldev.s3.amazonaws.com/i/6qwyiiz5i0zuufy2lhhg.png)

###### When we talk about a node's depth, we're specifying how many branches or levels down a node is from the root.

![img](https://i.giphy.com/media/MY1IngRAdaHVuNQbSu/giphy.gif)


###### However, when we talk about height, we can either describe the height of a node or the height of the tree. In both cases, we're describing the distance from an external node to the node or root.


### Binary Tree Identification

###### Binary trees can be structured differently and possess different kinds of characteristics or qualities.

![img](https://res.cloudinary.com/practicaldev/image/fetch/s--JPSEPSgm--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://thepracticaldev.s3.amazonaws.com/i/r2pju3fgkd5vguciusbo.png)

###### A full or strictly binary tree is structured so that every node possesses either two or no children.


![img](https://res.cloudinary.com/practicaldev/image/fetch/s--wWTgTWjD--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://thepracticaldev.s3.amazonaws.com/i/87vvozjt3vb4p94equv7.png)

###### A complete binary tree is a tree where nodes at every level but the last is required to have two children. On the last level, the children are positioned as far to the left as possible. So, complete binary tree nodes are connected from top to bottom, left to right.

![img](https://res.cloudinary.com/practicaldev/image/fetch/s--QHjI6oBx--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://thepracticaldev.s3.amazonaws.com/i/u9ybf23isl86jzdkei89.png)

###### A perfect binary tree is both full and complete. All the leaf nodes are located at the same depth, and all internal nodes have two children.

![img](https://i.giphy.com/media/iJgItT1WOBadn4NGle/giphy.gif)

###### A balanced binary tree describes a tree where two sibling subtrees don't differ in height by more than one level. If the difference in height is greater than that, then it is unbalanced.


![img](https://res.cloudinary.com/practicaldev/image/fetch/s--xorcLiJH--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://thepracticaldev.s3.amazonaws.com/i/fm989bdx4uhs98ey8qv6.png)

###### If every node in a tree has only one child, the structure is a degenerate or pathological tree, and is essentially a linked list.


### Why are Binary Trees Useful?

###### Like the family trees many of us are familiar with, trees are hierarchical and can represent structural relationships in the data. More technological examples and applications of trees can be the DOM or your file directory.

###### [Binary Search Trees (BSTs)](https://dev.to/jenshaw/binary-search-trees-are-the-best-gkk) are especially useful in algorithms because they are naturally sorted, which makes search, insertion, and deletion of values especially quick and efficient. This is definitely worth diving into in another blog post!