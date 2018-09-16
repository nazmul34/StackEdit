# LightOj 1379 - Toll Management

## About problem:  
A graph is given with 1000 node and 50000 edge. Find those path from **s** to **t** which cost is less then **p** .Print the size of maximum edge cost from all those path.
  

## Problem Idea:  

 1. I call a Dijkstra from **s** and a Dijkstra from **t** . 
 2. Then i finally check each edge:   
 

    1.  if((lev[0][j]+y+lev[1][x])<=p)
    
2.  {
    
3.  mx=max(mx,y);
    
4.  }

<!--stackedit_data:
eyJoaXN0b3J5IjpbMTU5NDQyNjY3NF19
-->