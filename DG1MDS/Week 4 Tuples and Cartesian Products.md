Cartesians are made up of sets and tuples 

Set vs Tuple
	Duplicates cannot exist : Duplicates are fine
	The order is not important : (x,y) is not the same as (y,x)
	Squiggly bracket : round bracket


Let A be {1.2.3}
Let B be {7,8,9}

A * B gives {(x,y) | X E A AND y E B} 
{(1,7), (1,8) (1,9), (2,7), (2,8), (2,9), (3,7), (3,8), (3,9)} <- the order is important as its x, y

you can also square a set such as A * A or A^2
if you have {(x,y)} you will end up with 
1,1 1,2 1,3 2,1 2,2 2,3
but if you have (x,x)
then its 1,1 2,2 3,3