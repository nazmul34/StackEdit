# LightOj 1379 - Toll Management

## About problem:  
A graph is given with 1000 node and 50000 edge. Find those path from **s** to **t** which cost is less then **p** .Print the size of maximum edge cost from all those path.
  

## Problem Idea:  

 1. I call a Dijkstra from **s** and a Dijkstra from **t** . 
 2. Then i finally check each edge:   
 

    if(lev[x]+cost_of_the_edge+lev[y]<=p)
    {
			mx=max(mx,

<!--stackedit_data:
eyJoaXN0b3J5IjpbMjAxNjU3OTI5N119
-->