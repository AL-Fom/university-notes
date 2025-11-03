## Matrix
a matrix is rectangular array of numbers referenced in rows and columns 
if you had a matrix (m) 

| 3   | 5   | 3   |
| --- | --- | --- |
| 2   | 7   | 6   |
| 6   | 4   | 2   |
| 8   | 9   | 0   |
to find 0 you would go to m$_4$$_,$$_3$ 

## Transposition 
of a vector rows become columns, columns become rows 
so that 
M

| 3   | 2   | 1   |
| --- | --- | --- |
| 4   | 5   | 6   |
becomes 
M$^T$

| 3   | 4   |
| --- | --- |
| 2   | 5   |
| 1   | 6   |
However this is NOT rotation 
as rotating the matrix above 90 degrees clockwise would make

| 4   | 3   |
| --- | --- |
| 5   | 2   |
| 6   | 1   |

## Vector
a vector is matrix with a single column 

| 3   |
| --- |
| 6   |
| 2   |
| 0   |
if you have vector V
to find 6 you just go to V$_2$

## Addition
only possible if the width and height is the same

you just add the elements of matrix A from position n,m with elements of B with the corresponding position

## Multiplication 
if a matrix one matrices' width is equal to the other height multiplication is possible so that
(row x column) x (row x column) 
the firsts column is equal to rows in 2nd
the resulting size of the matrix will be row of first x column of 2nd
you then multiply each row by each column