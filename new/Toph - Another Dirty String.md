# Toph - Another Dirty String

## About problem:  
Given three strings  **A**,  **B**  and  **C**.

Find the length of the longest common substring of  **A**  and  **B**, which doesn’t have  **C**  as a substring.
  
  For each test there will be three lines describing string  **A**,  **B**, and  **C**.

1 ≤ T ≤ 100

1 ≤ |A|, |B|, |C| ≤ 105

## Problem Idea:  

 1. First I found the xor of node 0 to  all other node.
 2. Then I add this number to a tri tree.
 3. Then for each node I found the maximum xor value possible. Maximum for all the node is the ans.

<!--stackedit_data:
eyJoaXN0b3J5IjpbMTAxMjkyODA0Nl19
-->