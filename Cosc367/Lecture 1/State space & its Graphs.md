#BaseConcepts
# State Space
State - Data struct (obj) that represents a possible config of the world (agent or  environment)

State Space of a problem is the set of all possible states for that problem
e.g A vacuum cleaner agent in two adjacent rooms which can either be clean or dirty (As below)
![[Pasted image 20230722102925.png|300]]
- Location {left, right}
-  Left-room {dirty, clean}
-  Right-room {dirty, clean}
- State-space = Cartesian product of Location, Left room, and Right room. -> 8 total states.
# State Space Graphs
### How actions change the state of the world
Suppose the vacuum cleaner agent can take the following actions: L (go left), R (go right), S (suck).
![[Pasted image 20230722103608.png]]

