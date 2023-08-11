#Lecture 
Part 2: Pruning, informed search, other strategies
## The Problem with cycles and multiple paths
There is an issue that affects all search strategies in the framework of a [[General Graphs|Generic Graph Search]]
	The algorithm can expand multiple paths to the same node.
Can cause:
- Cycles (infinite search tree)
- Wasted computation
Solution:
	We "[[Pruning|Prune]]" unnecessary branches of the search tree.

## Search heuristic
Idea: don't ignore info about the goal when selecting paths. Often there is extra knowledge that can be used to guide the search: ***Heuristics***.
### Heuristics
**h(n)** is an estimate of the cost of the shortest path from node n to a goal node
h needs to be efficient to compute
h can be extended to paths h(⟨n<sub>0</sub>,...,n<sub>k</sub>⟩) = h(n<sub>k</sub>).
- h is said to be **Admissible** if and only if ∀n h(n) ≥ 0 \[i.e. h is non-negative]; and
-  there is no path from n to a goal node with cost less than h(n).
	- In other words h never over-estimates the cost.


## [[A* Search Strategy]]



