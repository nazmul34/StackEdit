# CodeChef - SEAGM

## About problem:  
n number is given. At first x=0. Two player play a game. In each tern a player choose a number and make x=gcd(x,number) and that number can be used by any of them. If x=1 or no number left that player loose. 
**1<=N<=100 
1<=a[i]<=100** 
  

## Problem Idea:  

 1. This problem can be solved by DP. But how can we check which number we have taken. n=100 so bitmask is not possible.
 2.  We can find those number by using x. If x==gcd(x,number) then we can find how many number with common gcd x is taken. Other number is not 

<!--stackedit_data:
eyJoaXN0b3J5IjpbLTEzNzU3MjAxMDldfQ==
-->