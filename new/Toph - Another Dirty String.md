# Toph - Another Dirty String

## About problem:  
Given three strings  **A**,  **B**  and  **C**.

Find the length of the longest common substring of  **A**  and  **B**, which doesn’t have  **C**  as a substring.
  
  For each test there will be three lines describing string  **A**,  **B**, and  **C**.

1 ≤ T ≤ 100

1 ≤ |A|, |B|, |C| ≤ 10^5  

## Problem Idea:  

 1. First for each index **i ( 0<=i<A.size() )** I found the maximum position I can take to the right A[i...j], that does not contain C as substring. We can do it but running a KMP.
 2. Then I join string A and B and find the suffix sort array and lcp.
 3. Now I consider **x** as a common substring between between last  index of A and B in the suffix sort array. At first **x**=0.
 4. If I found a suffix of string A, then I update **x** with maximum possible length of suffix A is possible **(starting at SA[i])** without C as substring.
 5. If previous suffix is for B then we update max with min(x,lcp[i]). Or if we found a suffix of B we update max with min(x,lcp[i]).
<!--stackedit_data:
eyJoaXN0b3J5IjpbMTQwMDAwODY1MiwtMTExMDgxODEwLDE2Mz
Y0NjIxMTJdfQ==
-->