#Problem 
## Trace LCFS with pruning on the following graph:
![[Pasted image 20230730134715.png|200]]
```
nodes = {S, A, B, G}, 
edge_list=[(S,A,3), (S,B,1), (B,A,1), (A,B,1), (A,G,5)], 
starting_nodes = [S], 
goal_nodes = {G}.
```
#### Answer:
```
			#Considered = {}
+S, 0        
-S, 0       #Considered = {S}
+SA, 3
+SB, 1
-SB, 1      #Considered = {S, B}
+SBA, 2     
-SBA, 2     #Considered = {S, B, A}
+SBAB, 3!   #Not Added (!)
+SBAG, 7    
-SA, 3!     #Not added (already explored)
-SBAG, 7    #Considered = {S,B,A,G}
```

