#BaseConcepts  
![[Pasted image 20230722130536.png|400]]
## Remarks
Which value is selected from the frontier at each stage defines the search strategy. In our implementation we pass a frontier object to the search procedure. The frontier object is in charge of selecting the next path.

The Function *neighbor* defines the graph. In our implementation we we use the method **outgoing_arcs** for this purpose.

The function goal(n<sub>k</sub>) defines what is a solution. In our implementation we use the method **is_goal** for this purpose. 

If more than one answer is required, the search can continue. For this reason in our implementation we use **Yeild** instead of return.
