# CodeChef - SEAGM

## About problem:  
You are playing a game with a robot. The game starts with two integers:  **A**  and  **M**. The robot makes exactly one move in the entire game, and it does so at the very beginning - it will remove exactly 1 digit from  **A**  and output it as the starting value (say  _X_). Note that the value  **A**  remains intact. It is not changed by the robot. After the robot makes its moves, it is your turn. You can make an unlimited number of moves. In each move, you must remove exactly 1 digit from A and append it to  _X_  (to the right side of X). Again note that none of your moves change the value of  **A**. You win if you can eventually make X a multiple of M (i.e. X mod M = 0). How many possible starting moves bot can make such that you are guaranteed to win assuming you play optimally?

Here is an example of a game: Suppose the numbers are  **A**  = 1003,  **M**  = 4. The robot can make four possible starting moves: 003 by removing 1st digit, 103 by removing 2nd or 3rd digit (both count as a separate possibilities even though the starting X will be same) or 100 by removing the 4th digit. Let us say the robot chooses 003 as the starting move. Then you can win by appending 100 (by removing the 4th digit) making X = 003100 which is divisible by 4.
-   For each test case, output a single line containing the number of possible first moves that the robot can make such that you can force a win.
  -   **1**  ≤  **T**  ≤  **100**
-   **10**  ≤  **A**  <  **10^(10 ^ 6)**  (i.e. The number of digits in  **A**  can be upto 106)
-   **1**  ≤  **M**  ≤  **1000**
-   The sum of number of digits of  **A**  over all test cases will not exceed  **5 * 10^6**

## Problem Idea:  

 1. 1st I find all the number removing each digit.
 2. Then we mod those number by M suppose store in ara[].
 3. Then I build a graph if it is possible to go from x to y (y=x+ara[i] )%M . Here x,y<M .
 4. In the reverse graph if it is possible  to move from 0 to a node then cou 

<!--stackedit_data:
eyJoaXN0b3J5IjpbMjAxODEwNzc0OSwtNTYxMzAxMzA3XX0=
-->