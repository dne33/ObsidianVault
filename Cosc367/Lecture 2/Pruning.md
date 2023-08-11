#BaseConcepts 
Principle: Do not expand paths to nodes that have been **considered for expansion.**

A node is considered for expansions when the frontier returns a path ending in that node to a generic search algorithm (thus the algorithm tries to expand the path).

## Implementation
- The frontier keeps track of expanded nodes (usually by putting them in a set)
-  When trying to add a new path to the frontier, the frontier adds the path only if it does not end with a node that is already expanded, otherwise the path is discarded ***Pruned***.
```
def get_next_path():
	selected_path = select_path()
	remove_path(selected_path)
	if not selected_path.isExpanded():
		return selected_path
	//Already expanded so prune this branch
	return null
```
[[Tracing Frontiers With Pruning]]
