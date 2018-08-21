# 1151 - Snakes and Ladders
##  Problem Idea:
(Ex=number of expected throw from point x)

 1. If there is a ladder bottom or sanke head at point "x" and it leads to "y". 
	Eqn:
    Ex=(0+Ey) (0 because no throwing of dice is needed)
        Ex-Ey=0

 2. If we are at the 100th point. Then,
	Ex=0 
 3. Else ,for the other point.From point "x" we could get 1..6 number from the dice.
	Ex=(1+Ex+1);
	Ex=(1+Ex+2);
	.
	.
	Ex=(1+Ex+6);
	
	sum this six eqn:
	6Ex=6+(Ex+1....+Ex+6)
     =>(Ex+1....+Ex+6)-6Ex=-6
	
  suppose, (x+5 and x+6 is > 100) then 6Ex would be 4Ex... because those two expected value is   not in a valid state.
  so eqn. will be.
	
  Eqn:
  (Ex+1....+Ex+6)-4Ex=-6

after that we could find the solution using gaussian elimination.

<!--stackedit_data:
eyJoaXN0b3J5IjpbMTY2MDIwNTU2Nl19
-->