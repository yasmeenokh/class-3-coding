# Trees

## Common Terminology
**Root:** The root is the node at the beginning of the tree
**K:** A number that specifies the maximum number of children any node may have in a k-ary tree. In a binary tree, k = 2.
**Left:** A reference to one child node, in a binary tree
**Right:** A reference to the other child node, in a binary tree
**Edge:** The edge in a tree is the link between a parent and child node
**Leaf:** A leaf is a node that does not have any children
**Height:** The height of a tree is the number of edges from the root to the furthest leaf

![tree](https://reactgo.com/static/7f89ae4896c007403969537c52ea2103/27524/tree-datastructure-diagram.png)

## Traversals
1. Depth First: 
Depth first traversal is where we prioritize going through the depth (height) of the tree first.

2. Breadth First: 
Breadth first traversal iterates through the tree by going through each level of the tree node-by-node.

![vs](https://miro.medium.com/max/3648/1*VM84VPcCQe0gSy44l9S5yA.jpeg)

## Binary Tree Vs K-ary Trees
Trees can have any number of children per node, but Binary Trees restrict the number of children to two (hence our left and right children).
![k-ary](https://media.geeksforgeeks.org/wp-content/uploads/20200219144238/General-Tree-vs-Binary-Tree.png)

### Adding a node
During the traversal, we find the first node that does not have all it’s children filled, and insert the new node as a child. We fill the child slots from left to right.

## Binary Search Trees

![binary](https://www.gatevidyalay.com/wp-content/uploads/2018/07/Binary-Search-Tree-Example.png)

A Binary Search Tree (BST) is a type of tree that does have some structure attached to it. In a BST, nodes are organized in a manner where all values that are smaller than the root are placed to the left, and all values that are larger than the root are placed to the right.

### Searching a BST

Searching a BST can be done quickly, because all you do is compare the node you are searching for against the root of the tree or sub-tree. If the value is smaller, you only traverse the left side. If the value is larger, you only traverse the right side.


