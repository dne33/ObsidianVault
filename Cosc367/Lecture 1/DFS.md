#Algorithms 
In Depth First Search the [[General Purpose Search Algorithm|Generic Graph Search]] must be used with a stack [[Frontier|Frontier]]

If the stack is a Python list of the form ```[..., p, q]``` where each element is a [[Directed graphs#Paths|path]], then:

1. *q* is selected (popped)
2. if the algorithm continues, then [[Directed graphs#Paths|paths]] that extend *q* are pushed (appended) to the stack.
3. *p* is only selected (popped) when all paths from *q* have been explored
As a result at each stage the algorithm expands the deepest path.

### Depth First Illustration
![[Pasted image 20230723104955.png|400]]
Assume right arc comes before the left arc

#Problem 
### Behaviour
![[Pasted image 20230723105140.png|400]]
Which shaded goal will a DFS find first?
#### Click to reveal answer

![[Pasted image 20230723105916.png|400]]
A arcs are appended to the stack first then B.
Since DFS B is popped first and explored.>)






## DFS: behaviour and complexity


> [!question]- Does DFS guarantee to find a solution with the fewest arcs (if there is a solution)?
> No, If there is a Cycle e.g A->B, A->C B->D D->A If A->C is the right arc it will constantly be on the bottom of the stack and if C is the solution it will never be found.

> [!question]- Is it complete? (i.e. does it guarantee to find a solution if there is one?)
> No, If there is a Cycle e.g A->B, A->C B->D D->A If A->C is the right arc it will constantly be on the bottom of the stack and if C is the solution it will never be found.

> [!question]- Does it halt on every graph?
> No, If there is a Cycle e.g A->B, A->C B->D D->A If A->C is the right arc it will constantly be on the bottom of the stack and if C is the solution it will never be found.

> [!question]- Does the goal state affect the search behaviour?
> Yes, It keeps going until it either reaches the goal or gets stuck. If the goal is nearby, DFS might find it quickly, but if it's far away, the search can take longer. Also, DFS doesn't always find the shortest path to the goal.


**Assume a finite search tree of depth d and branching factor b:** 
> [!question]- What is the time complexity?
> O(b^d)

> [!question]- What is the space complexity?
> O(b\*d)


[[Frontier#Example Tracing frontier in DFS|Tracing Frontier Problem]]


