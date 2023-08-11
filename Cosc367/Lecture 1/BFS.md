#Algorithms 
To perform Breadth First Search, the [[General Purpose Search Algorithm|Generic Graph Search]] must be used with a queue [[Frontier]] (FIFO)
As a result, at each stage, the algorithm expands the shallowest path.

## Breadth-First Illustration 
![[Pasted image 20230723125310.png|400]]
Assume left arc comes before the right arc.

#Problem 
### Behaviour
![[Pasted image 20230723125559.png|400]]
Which shaded goal will a DFS find first?
#### Click to reveal answer
![[Pasted image 20230723125512.png|400]]










## BFS: behaviour and complexity

> [!question]- Does BFS guarantee to find a solution with the fewest arcs (if there is a solution)?
> Yes

> [!question]- Is it complete? (i.e. does it guarantee to find a solution if there is one?)
> Yes, even if the search tree has an infinite loop if there is a solution you will see it.

> [!question]- Does it halt on every graph?
> No, If there is an infinite loop which has no goal node then it will not halt

> [!question]- Does the goal state affect the search behaviour?
> No

**Assume a finite search tree of depth d and branching factor b:** 
> [!question]- What is the time complexity?
> O(b^d)

> [!question]- What is the space complexity?
> O(b^d),  as all paths are stored not just the current path.

[[Tracing Frontiers#Example Tracing frontier in BFS|Tracing Frontier in BFS]]

