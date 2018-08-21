# 1279 - Graph Coloring
##  Problem Idea:
**color(v) = color(u1) + color(u2) + ... + color(um) (modulo K)**  
There are n equation for  each  **0**  ≤  **v**  ≤  **n** .
We can find the value of each v by using [Gauss-Jordan elimination for linear equations](https://cp-algorithms.com/linear_algebra/linear-system-gauss.html).  
Number of color is K. In the RREF(Reduced Row-Echelon Form) matrix, if there is no free element then ans would be 1. Otherwise 
 ans would be , *K^(free elment)* .  
   
   *Free element = n - number of pivot element*  
   
   in the RREF matrix.

<!--stackedit_data:
eyJoaXN0b3J5IjpbLTE5MTY5OTc0MzksLTQxODY0NjM0MCw4ND
IxODg1MTJdfQ==
-->