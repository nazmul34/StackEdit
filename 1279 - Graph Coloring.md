# 1279 - Graph Coloring
##  Problem Idea:
**color(v) = color(u1) + color(u2) + ... + color(um) (modulo K)**  
There are n equation for  each  **0**  ≤  **v**  ≤  **n** .
We can find the value of each v by using [Gauss-Jordan elimination for linear equations](https://cp-algorithms.com/linear_algebra/linear-system-gauss.html).  
Number of color is K. In the RREF(Reduced Row-Echelon Form) matrix, if there is no free element then ans would be 1. Otherwise ans would be, *( K ^ (free elment) ) % mod*.  
   
   *free element = n - number of pivot element*  
   
   in the RREF matrix. Pivot element have only one solution.But free element can have infinity number of solution. Here number of color is K, so each free element can have K kind of solution and overall   *K^( free elment )*  solution.     



<!--stackedit_data:
eyJoaXN0b3J5IjpbLTEwOTAzMzQzODQsLTE5MTY5OTc0MzksLT
QxODY0NjM0MCw4NDIxODg1MTJdfQ==
-->