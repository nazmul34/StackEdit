# 1272 - Maximum Subset Sum
##  Problem Idea:
Actually the problem is:  From A1^ A2 ^ .......^An find a subset which produce maximum result.   
Each number is 64 bit. By using this bit we could consider each number as a row of 64 element of a matrix. Now we could use Gaussian elimination in this matrix. After this elimination each row of the new matrix represent a number. At first ans = 0. From row i=0 to n-1  
`if (value_of_row_i ^ ans > ans )    
     ans = value_of_row_i ^ ans;`  
  
This is how we could update the result. A details solution is [here](https://math.stackexchange.com/a/52478/585911)

<!--stackedit_data:
eyJoaXN0b3J5IjpbLTE4OTA0MDc2NTUsLTEyOTgxOTk3OF19
-->