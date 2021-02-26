# Graphs:

- a non-linear data structure that can be looked at as a collection of **vertices**(nodes), potentially connected by line segments known as **edges**
- common terminology when working w/ Graphs:
    * Vertex - "node", is a data object that can have zero or more adjacent vertices.
    * Edge - a connection between two nodes
    * Neighbor - the neighbors of a node are its adjacent nodes (are connected via an edge)
    * Degree - degree of a vertex is the number of edges connect to vertex

## Directed vs Undirected
- **Undirected graph**: a graph where each edge is undirected or bi-directional. Aka, the undirected graph does not move.
- **Directed graph**: also known as *Digraph*, a graph where every edge is directed. This type of graph HAS a direction, each node is directed at another node w/ a specific requirement of what node should be referenced next.

## Complete vs Connected vs Disconnected:
- **Complete graph** : when all nodes are connected to all other nodes
- **Connected graph** : a graph where all vertices/nodes have at least one edge
- **Disconnected graph** : a graph where some vertices may not have edges

## Acyclic vs Cyclic:
- **Acyclic graph** : directed graph without cycles. A cycle when a node can be traversed through and potentially end up back at itself.
- A directed acyclic graph is also called *DAG*. Can be represented as a *tree*

## Adjaceny Matrix
- is represented through a 2-dimensional array. If there are n vertices, then we are looking at n x n Boolean matrix.

