#BaseConcepts 
In graph theory, the "frontier" typically refers to a set of nodes or vertices that are on the "boundary" or "edge" of a certain region or component of the graph. [[Explicit vs Implicit graphs#Frontier|Frontier Image]]

In other words, the frontier represents the "border" between the explored and unexplored parts of the graph. It's the set of nodes that are reachable in one step from the already visited nodes but haven't been visited themselves. The frontier is a concept often used in algorithms that traverse or search through graphs, such as breadth-first search or depth-first search.


## How to Trace the frontier
1. Starting with an empty frontier, we record all the calls to the frontier
	- To add or to get a path. We dedicate one line per call.
2. When the frontier is asked to add a path, we start the line with a **+** followed by the path that is being added.
3.  When the frontier is asked to return a path, we start with the line(s) with a **-** followed by the path(s) that is (are) being removed
4.  When using a priority queue, the path is followed by a comma and then the key.
5. The lines of the trace should match the following regular expression (case and space insensitive): ``^[+-][a-z]+(,\d+)?!?$`` 
## Tracing the Frontier Examples/Problems
	[[Tracing Frontiers#Example Tracing frontier in DFS|Tracing Frontier in DFS]]
	[[Tracing Frontiers#Example Tracing frontier in BFS|Tracing Frontier in BFS]]
	
	









