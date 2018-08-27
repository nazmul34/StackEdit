# SPOJ - LCS2
## About problem:
At most 10 string with 10^5 size is given. All are in lower case. Find the **longest common substring(LCS)** among them.


##  Problem Idea:

 1. At first we add the first string to suffix automata. 
 2. For the other string, we only find its **LCS**  with first string. We saved the minimum **LCS** to every node. And finally maximum among the minimum is the ans. 

<!--stackedit_data:
eyJoaXN0b3J5IjpbMTY3NzcxNDU0LC00MDUxOTQwNV19
-->