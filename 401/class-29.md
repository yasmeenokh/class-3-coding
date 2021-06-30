# Graphs

## Definition
A graph is a non-linear data structure that can be looked at as a collection of vertices (or nodes) potentially connected by line segments named edges.

## Common Terminology

**Vertex**: A vertex, also called a “node”, is a data object that can have zero or more adjacent vertices.
**Edge**:  An edge is a connection between two nodes.
**Neighbor**: The neighbors of a node are its adjacent nodes, i.e., are connected via an edge.
**Degree**: The degree of a vertex is the number of edges connected to that vertex.

## Types 

**Direction Based**

1. **Undirected Graphs:**

### Definition:
An Undirected Graph is a graph where each edge is undirected or bi-directional. This means that the undirected graph does not move in any direction.

![undirected](https://algocoding.files.wordpress.com/2015/04/undirected_example.png)

2. **Directed Graphs (Digraph):**

### Definition:
A Directed Graph also called a Digraph is a graph where every edge is directed. Each node is directed at another node with a specific requirement of what node should be referenced next.

#### Subtypes

* **Acyclic:**
An acyclic graph is a directed graph without cycles. Also called a DAG. This can also be represented as what we know as a tree.

* **Cyclic:**
A cycle is when a node can be traversed through and potentially end up back at itself.

![AvsC](https://slidetodoc.com/presentation_image/328698c333378425f836f2808a1c878d/image-28.jpg)

**Connection or Completion Based**

1. **Complete**

### Definition:
A complete graph is when all nodes are connected to all other nodes.

![complete](https://media.geeksforgeeks.org/wp-content/uploads/4-109.png)

2. **Connected**

### Definition:
A connected graph is graph that has all of vertices/nodes have at least one edge. A Tree is a form of a connected graph.

![connected](https://www.tutorialspoint.com/discrete_mathematics/images/connected_graph.jpg)

3. **Disconnected**

### Definition:

A disconnected graph is a graph where some vertices may not have edges. It is complelty possible to have standalone nodes or edges (also known as islands) in a graph data structure.

![disconnected](https://upload.wikimedia.org/wikipedia/commons/thumb/6/6b/Unconnected-graph.svg/1072px-Unconnected-graph.svg.png)


### Graph Representation
**We represent graphs through:**

1. Adjacency Matrix: An Adjacency matrix is represented through a 2-dimensional array. If there are n vertices, then we are looking at an n x n Boolean matrix. 

**NOTE** 
a sparse graph is when there are very few connections. a dense graph is when there are many connections

2. Adjacency List: An adjacency list is a collection of linked lists or array that lists all of the other vertices that are connected.

### Weighted Graphs
A weighted graph is a graph with numbers assigned to its edges. These numbers are called weights. Within adjacency lists, you must include both the weight and the name of the adjacent vertex.

### Traversals

1. `Breadth First` 
Breadth first traversal is when you visit all the nodes that are closest to the root as possible. From there you traverse outwards, level by level, until you have visited all the vertices/nodes.

**NOTES**
1. If there are any disconnected nodes (such as islands) with the graph data structure, they will not be traversed.
2. Breadth-first only outputs the nodes that are connected in some relation to the root that you pass in.

2. `Depth First`
Similar to how the breadth-first uses a queue, we use a Stack for our depth-first traversal.


### Real World Uses of Graphs

**Here are just a few examples of graphs in use:**

1. GPS and Mapping
2. Driving Directions
3. Social Networks
4. Airline Traffic
5. Netflix uses graphs for suggestions of products



