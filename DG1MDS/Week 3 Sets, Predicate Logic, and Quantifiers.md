# Sets
Sets - Enumeration Notation 
	Notation is {x,y,z}
	Order is irrelevant {x,y,z,} == {y,z,x}
	Repetition is ignored so {x,x,y,z} = {x,y,z}

Cardinality
	The size of a set 
	The smallest set you can have is {} == ∅ (It's not the same as zero)
	The lines around the set "| |" is asking for the cardinality |{0,2,1}| <- 3
	|{}| = 0

Number Range Notation 
	{0,1,2,3,4,5} = {0,...,5}
	(1,2,3,...) = all positive 
	Special Number Ranges:
		{0,1,2,...} = ℕ (All Natural Numbers)
		(...,-2,-1,0,1,2,...) = ℤ (All Integers)

Set Membership Notation
	x ∈ S = object x is a member of set S
	y ∉ S = object is NOT a member of set S

Subsets 
	Set within another set
	S ⊆ T = set S is a subset of set T
	{1} ⊆ {1,2}
	{} ⊆ {1,2}
	{} ⊆ T
	{1} ⊄ {} (Not a subset as there cant be a 1 in an emtpy set)
	Any set is a subset of itself 

Set Builder Notation
	Enumeration:
		Let B be {1,2,3,4,5}
	Builder Notation 
		{X ∈ B | x >0 ∧ x < 6 }
		Example:
			{X + 1 | x ∈ {1,2,3} ∧ x is odd}
			Truth Table

| x ∈ {1,2,3} | x is odd | x + 1 |
| ----------- | -------- | ----- |
| 1           | T        | 2     |
| 2           | F        | N/A   |
| 3           | T        | 4     |
			So the set is {2,4}

Set Operators
	Union U
		Can be expressed as { x | x ∈ A ∨ x ∈ B } A OR B
	Intersection ∩
		Can be expressed as { x | x ∈ A ∧ x ∈ B } A AND B
	Difference \
		Can be expressed as { x | x ∈ A ∧ x ∉ B } A NOT B
		THIS but NOT THAT


# Predicate Logic
Predicate logic works with the following
	Works similarly to 
		Proposition: John plays the guitar
		Predicate: "Plays The"
		Objects: John, Guitar
		Math Notation: playsThe(John, Guitar)
	True False (Truth values)
	∧  ∨ ¬ (Logical operators)
	12 -5 0 3.141 ... (Term Values ℤ)
	x y z  (Term Variables)
	P Q R (Predicate Variables)
		Each Variable is restricted to a set
		For example playsThe{x,y} or P{x,y}
		x ∈ People
		y ∈ Instruments

A predicate can contain any of the above 
	such as P(V$_1$, V$_2$,..., V$_n$) this predicate has arity of n
	Ax example would be IsEdible(x) where "x" can be cake or glass (True or False)

The average predicate will look like:
	P(y) "y is prime" such that 
		4 is false 
		3 is true 
	this predicate has an arity of 1 
	a predicate of arity 2 would look like the following
	R(x,y) "x > y" where R(5,5) is false and R(6,5) is true

Another example of a predicate could be:
	R(x) is the predicate of P(5,y)
	P(5,y) is the predicate 5 > y
	if you substitute 5 for x you get 5>5 which is not true



# Quantifiers
Universal Quantifier (∀) - Every statement is true for every element of the domain (For all)
	∀x ∈ ℕ, x + 0 = x
	This translates to for every natural number, if you add zero to it, it will equal itself


Existential Quantifier (∃) - For at least one element in the domain (There is at least one)
	∃x ∈ ℕ, x$^2$ = 4
	This translate to for at least one natural number the square of it will be equal to 4

| ℕ   | x$^2$ | 2x  | x$^2$ = 2x |
| --- | ----- | --- | ---------- |
| 0   | 0     | 0   | True       |
| 1   | 1     | 2   | False      |
| 2   | 4     | 4   | True       |
| 3   | 9     | 6   | False      |
| ... |       |     |            |

(∃x ∈ TheBeatles)(PlaysThe(x, Guitar) ∧ PlaysThe(x, Drums))

| x ∈ TheBeatles | PlaysThe (x, Guitar) | PlaysThe (x, Drums) | PlaysThe(x, Drums) ∧ PlaysThe(x, Guitar) |
| -------------- | -------------------- | ------------------- | ---------------------------------------- |
| John           | T                    | F                   | False                                    |
| Paul           | T                    | T                   | True                                     |
| George         | T                    | F                   | False                                    |
| Ringo          | F                    | T                   | False                                    |