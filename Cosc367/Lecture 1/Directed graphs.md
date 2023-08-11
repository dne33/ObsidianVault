#Graphs
- Many AI problems can be abstracted into the problem of finding a path in a directed graph
- A graph consists of a set of **nodes** and a set of **arcs** 
	- **Nodes** are usually used for states 
	- **Arcs** are used for actions [[State space & its Graphs#State Space Graphs|The Left, Right, Suck]]

## Paths
- In theory, a **path** is a sequence of nodes <n<sub>0</sub>, n<sub>1</sub>, ... n<sub>k</sub>> where there is an arc from n<sub>i</sub> to n<sub>i+1</sub>
	- In practice, a path is a sequence of **arcs**
-  The length of an path <n<sub>0</sub>, n<sub>1</sub>, ... n<sub>k</sub>>  is k.

-  An arc can have an associated cost (distance, time, energy, etc). The **cost** is the sum of the **cost**
of the **arcs** along the **path**.

- Given a set of **starting nodes** and a set of **goal nodes** (desired states), a solution is a path form a start node to a goal node.