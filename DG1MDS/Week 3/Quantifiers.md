Universal Quantifier (∀) - Every statement is true for every element of the domain (For all)
	∀x ∈ ℕ, x + 0 = x
	This translates to for every natural number, if you add zero to it, it will equal itself

(∃x ∈ TheBeatles)(PlaysThe(x, Guitar) ∧ PlaysThe(x, Drums))

| ℕ   | x$^2$ | 2x  | x$^2$ = 2x |
| --- | ----- | --- | ---------- |
| 0   | 0     | 0   | True       |
| 1   | 1     | 2   | False      |
| 2   | 4     | 4   | True       |
| 3   | 9     | 6   | False      |
| ... |       |     |            |
Existential Quantifier (∃) - For at least one element in the domain (There is at least one)
	∃x ∈ ℕ, x$^2$ = 4
	This translate to for at least one natural number the square of it will be equal to 4

(∃x ∈ TheBeatles)(PlaysThe(x, Guitar) ∧ PlaysThe(x, Drums))

| x ∈ TheBeatles | PlaysThe (x, Guitar) | PlaysThe (x, Drums) | PlaysThe(x, Drums) ∧ PlaysThe(x, Guitar) |
| -------------- | -------------------- | ------------------- | ---------------------------------------- |
| John           | T                    | F                   | False                                    |
| Paul           | T                    | T                   | True                                     |
| George         | T                    | F                   | False                                    |
| Ringo          | F                    | T                   | False                                    |