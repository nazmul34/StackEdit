# SPOJ - NSUBSTR
## About problem:
You are given a string S which consists of 250000 lowercase latin letters at most. We define F(x) as the maximal number of times that some string with length x appears in S. For example for string 'ababa' F(3) will be 2 because there is a string 'aba' that occurs twice. Your task is to output F(i) for every i so that **1<=i<=|S|**.

##  Problem Idea:
I used suffix automata to solve this problem. Then we used a queue like topological sorting, this helps to find all the maximum occ
<!--stackedit_data:
eyJoaXN0b3J5IjpbMTc4Mzc1MTMwNCwtMTc4NTcxNDg4OV19
-->