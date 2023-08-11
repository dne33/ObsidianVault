#Graphs
# Explicit vs Implicit graphs
### Explicit Graphs
An explicit graphs nodes (vertices) and arcs (edges) are readily available. They are read from the input and stored in a data structure such as an adjacency list or matrix.
	The entire graph is in memory.
	The complexity of algorithms are measured in terms of the number of vertices &/or edges.

### Implicit Graphs
In implicit graphs a procedure *outgoing_arcs*  (or neighbours) is defined that given a node, returns the set of directed arcs that connect the node to other nodes.
	The graph is generated on the fly.
	The complexity of algorithms are measured in terms of the depth of a goal node and the *average branching factor* (average number of outgoing arcs).

# Searching Graphs
Generic Search Algorithm:
	Given graph, start nodes and goal nodes, incrementally explore paths from the start nodes.

Maintain a **frontier** of the paths that have been explored from the starting node(s)

As search proceeds the **Frontier** is updated and the graph is explored until a goal node is encountered.

The order in which paths are removed and added to the frontier defines the **Search Strategy**
#### Frontier
![[Pasted image 20230722125935.png|300]]