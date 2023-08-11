#Problem 
### Example: Tracing frontier in [[DFS]]
Given the following 
```
graph nodes={a, b, c, d, e}, 
edge_list=[(a,b), (a,d), (a, c), (c, d)], 
starting_nodes = [b, a, e], 
goal_nodes = {d}
```
trace the frontier in depth-first search (DFS).
Hint: use [[General Purpose Search Algorithm]]
##### Answer:
Stack = ``[b, aX, eX, ab, ad, acX, acd]``
Frontier Trace:
\+ b
\+ a
\+ e
\- e *pop, no children*
\- a *pop, explore children*
\+ ab
\+ ad
\+ ac 
\- ac *pop, explore children*
\+ acd
\- acd *pop, Goal found*


### Example: Tracing frontier in [[BFS]]
Given the following 
```
graph nodes={a, b, c, d}, 
edge_list=[(a,b), (a,d), (a, c), (c, d)], 
starting_nodes = [a], 
goal_nodes = {d}
```
trace the frontier in depth-first search (DFS).
Hint: use [[General Purpose Search Algorithm]]
##### Answer:
Frontier Trace:
\+ a
\- a *pop, explore children*
\+ ab
\+ ad 
\+ ac
\- ab *pop*
\- ad *pop, goal found*Sa


### Example: Tracing frontier in [[LCFS]]
Given the following 
```
nodes={a, b, c, d, g}, 
edge_lists=[(a,b,4), (a,c,2), (a,d,1), (b,g,4), (c,g,2), (d,g,4)], starting_nodes = [a], 
goal_nodes = {g}
```
trace the frontier in depth-first search (LCFS).
Hint: use [[General Purpose Search Algorithm]]
##### Answer:
Frontier Trace:
\+ a, 0
\- a, 0
\+ ab, 4
\+ ac, 2
\+ ad, 1
\- ad, 1
\+ acg, 4
\- ab, 4
\+ abg, 8
\- acg, 4



### Example: Tracing frontier in [[A* Search Strategy]]
