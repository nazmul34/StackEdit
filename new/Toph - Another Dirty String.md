# Toph - Another Dirty String

## About problem:  
Given three strings  **A**,  **B**  and  **C**.

Find the length of the longest common substring of  **A**  and  **B**, which doesn’t have  **C**  as a substring.
  
  For each test there will be three lines describing string  **A**,  **B**, and  **C**.

1 ≤ T ≤ 100

1 ≤ |A|, |B|, |C| ≤ 10^5  

## Problem Idea:  

 1. First for each index **i ( 0<=i<A.size() )** I found the maximum position I can take to the right A[i...j], so that that does not contain C as substring. We can do it but running a KMP.
 2. Then I join string A and B and find the suffix sort array and lcp.
 3. Now consider x as a common substring between between last inex 
<!--stackedit_data:
eyJoaXN0b3J5IjpbMTkzNzUyNDMxNiwtMTExMDgxODEwLDE2Mz
Y0NjIxMTJdfQ==
-->