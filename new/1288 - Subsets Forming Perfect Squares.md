# 1288 - Subsets Forming Perfect Squares
##  Problem Idea:

 1. Less then 300 , there are only 62 prime number. So, we could use 64 bit number to represent this 62 prime number. Each bit of a number represents a prime number.
 2. First of all, we prime factorize each of n number and if a number have a odd number of 2 in it's factorization then we add 1 bit at 0th position. If odd number of 3 exist then we add 1 bit at 1th position. We should do this same thing to other prime number and get new representation of each number.
 3. We could use this new number in [Gauss-Jordan elimination](https://cp-algorithms.com/linear_algebra/linear-system-gauss.html) could get the number of pivot element.The ans would be, *( 2 ^ (free element) - 1 ) % mod*.  Here 2 is used, because from **f**( number of free element) we could get 2^f combination of numbers. Here not choosing of any number is considered as a way. So we remove 1 from 2 ^ f.  
   *free element = n - number of pivot element*


<!--stackedit_data:
eyJoaXN0b3J5IjpbLTE3MDQzNTAwMjgsLTEyNTk1MDgwMDIsLT
EwMjgwOTA0NDhdfQ==
-->