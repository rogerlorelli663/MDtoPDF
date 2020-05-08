
# Exam #2

## Problem #1
* a) Write pseudocode for a dynamic algorithm which takes as input an undirected graph and outputs a set containing all cliques in $G$. Your algorithm should find $C_n$ by finding $C_i$ for each $i < n$ sequentially. 
```
IN: undirected graph G = (V,E)
C = {C[0]} where C[0] = {0}  
v = vertex of V

while(V is not empty)
   v = V[0]
   remove v from V
   add v as new clique to new clique set C_i
   for each previous clique set C[j] in C
	   c = clique in C[j]
	   if(v does not have an edge with c[0])
	       break
       else
	       for k in range of initial number of clique in C[j]
		       if(v shares an edge with all vertices in c[k])
				   add union of v & c[k] as new clique to C[i] 
   add C_i to C

OUT: C, an set of clique sets containing all possible cliques within G      
             
```
 b) Does your algorithm always terminate? Prove it.
*  Yes, this algorithm always terminates by the LNP. V has a finite number of elements and during each loop 1 element is being removed. As such there will be an iteration that will find there are 0 elements left in the loop and will terminate.

c) Is your algorithm fully correct? Justify your answer in 3 sentences or less (this is not a proof).
 * This algorithm is fully correct since it always terminates, by LNP, it's pre-conditions must have been met to even run, and when it does terminate the post conditions are met. Post-conditions are guaranteed to be met since all vertices have been traversed and compared against all previous cliques, as such it has boot strapped itself to include all possible cliques.  

## Problem #2
Find the time complexity of ALG .


# Exam #2

## Problem #1
* a) Write pseudocode for a dynamic algorithm which takes as input an undirected graph and outputs a set containing all cliques in $G$. Your algorithm should find $C_n$ by finding $C_i$ for each $i < n$ sequentially. 
```
IN: undirected graph G = (V,E)
C = {C[0]} where C[0] = {0}  
v = vertex of V

while(V is not empty)
   v = V[0]
   remove v from V
   add v as new clique to new clique set C_i
   for each previous clique set C[j] in C
	   c = clique in C[j]
	   if(v does not have an edge with c[0])
	       break
       else
	       for k in range of initial number of clique in C[j]
		       if(v shares an edge with all vertices in c[k])
				   add union of v & c[k] as new clique to C[i] 
   add C_i to C

OUT: C, an set of clique sets containing all possible cliques within G      
             
```
 b) Does your algorithm always terminate? Prove it.
*  Yes, this algorithm always terminates by the LNP. V has a finite number of elements and during each loop 1 element is being removed. As such there will be an iteration that will find there are 0 elements left in the loop and will terminate.

c) Is your algorithm fully correct? Justify your answer in 3 sentences or less (this is not a proof).
 * This algorithm is fully correct since it always terminates, by LNP, it's pre-conditions must have been met to even run, and when it does terminate the post conditions are met. Post-conditions are guaranteed to be met since all vertices have been traversed and compared against all previous cliques, as such it has boot strapped itself to include all possible cliques.  

## Problem #2
Find the time complexity of ALG .

