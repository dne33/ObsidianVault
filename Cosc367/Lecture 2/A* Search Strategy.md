#Algorithms 
## Idea
-  Don't be as wasteful as [[LCFS]]
-  Don't be as greedy as Best-First Search
-  Estimate the cost of paths as if they could be extended to reach a goal in the best possible way
## Evaluation Function
**f(p) = cost(p) + [[Searching the State Space#Heuristics|h(n)]]** 
-  *p* is a path, *n* is the last node on *p*
-  *cost(p)* = cost of path p (This is the actual cost from starting node to node *n*)
-  *h(n)* = an estimate of cost from n to goal (an optimistic estimate)
-  *f(p)* = estimated total cost of path through p to goal 
The frontier is a priority queue ordered by *f(p)*
## Monotonicity
#### Definition:
- A heuristic is monotone or consistent if for every two nodes n, and n' which is reachable from n:
	- ```h(n) <= cost(n,n`) + h(n`)```
	- ![[Pasted image 20230812114737.png|200]]
	



