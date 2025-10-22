Cartesians are made up of sets and tuples 

Set vs Tuple
	Duplicates cannot exist : Duplicates are fine
	The order is not important : (x,y) is not the same as (y,x)
	Squiggly bracket : round bracket


Let A be {1.2.3}
Let B be {7,8,9}

A * B gives {(x,y) | X E A AND y E B} 
{(1,7), (1,8) (1,9), (2,7), (2,8), (2,9), (3,7), (3,8), (3,9)} <- the order is important as its x, y

you can also square a set such as A * A or A$^2$
if you have {(x,y)} you will end up with 
1,1 1,2 1,3 2,1 2,2 2,3
but if you have (x,x)
then its 1,1 2,2 3,3


# Relations
Reflexivity 
	(∀x ∈ A) x R x
	All members of set a relates to itself 
	Example of the set 
	{x,y,z} the relation is {(x,x), (y,y), (z,z)} if you remove any of these its no longer reflexive

Symmetry
	(∀x ∈ A)(∀y ∈ A) (x R y ⇐⇒ y R x)
	x is related to y if y is related to x: two way relation
	Example of the set 
	{x,y,z} the relation is {(x,y), (y,x), (x,z), (z,x)}

Transitivity
	(∀x ∈ A)(∀y ∈ A)(∀z ∈ A) ((x R y ∧ y R z) ⇒ x R z)
	If A relates to Y, and Y relates Z, then X relates to Z kind of like skipping
	Example of the set
	{x,y,z} the relation {(x,y), (y,z), (x,z)}