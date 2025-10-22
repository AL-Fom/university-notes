
| p ∧ q ⟺  q ∧ p                 | p ∨ q ⟺ q ∨ p                  | Commutative             |
| ------------------------------ | ------------------------------ | ----------------------- |
| (p ∧ q) ∧ r ⟺ p ∧ (q ∧ r)      | (p ∨ q) ∨ r ⟺ p ∨ (q ∨ r)      | Associative             |
| p ∧ (q ∨ r) ⟺(p ∧ q) ∨ (p ∧ r) | p ∨ (q ∧ r) ⟺ (p ∨ q)  (p ∨ r) | Distributive            |
| p ∧ p ⟺ p                      | p ∨ p ⟺ p                      | Idempotent              |
| p ∧ True ⟺ p                   | p ∨ False ⟺ p                  | Identity                |
| p ∧ !p ⟺ False                 | p ∨ !p ⟺True                   | Negation                |
| p ∧ False ⟺ False              | p ∨ True ⟺ True                | Domination              |
| p ∨ (p ∧ q) ⟺ p                | p ∨ (p ∧ q) ⟺ p                | Absorption              |
| !(p ∧ q) ⟺ (!p)∨(!q)           | !(p ∨ q) ⟺ (!p)  (!q)          | De Morgans              |
|                                | !(!p) ⟺ p                      | Involution              |
|                                | (p ⇒ q) ⟺ (!p) ∨ q             | Conditional Equivalence |
|                                | (p ⇒ q) ⟺ ((!q) ⇒ !p)          | Contrapositive          |



# Propositional Logic
Propositional Statement is one that is either True or False 
	5>5 is a proposition that is false
	Can combine multiple propositions using logical operators (known as logical connectives) into a single proposition
		Proposition + Operator (AND, OR) + Proposition = Proposition
	Made up of Truth Values 
		True False
	Propositional Letters
		snowing -> s
		hailing -> h
		...
its important because it follows the programming structure use in many languages 
	if (a>b):


Logical Operators 

| A   | B   | A AND B |
| --- | --- | ------- |
| 0   | 0   | 0       |
| 0   | 1   | 0       |
| 1   | 0   | 0       |
| 1   | 1   | 1       |
	CONJUNCTION - AND (∧) && .

| A   | B   | A OR B |
| --- | --- | ------ |
| 0   | 0   | 0      |
| 0   | 1   | 1      |
| 1   | 0   | 1      |
| 1   | 1   | 1      |
	DISJUNCTION - OR (∨) || +

| A   | NOT A |
| --- | ----- |
| 0   | 1     |
| 1   | 0     |
	NEGATION - NOT (¬) !

| A   | B   | IMPLIES B |
| --- | --- | --------- |
| 0   | 0   | 1         |
| 0   | 1   | 1         |
| 1   | 0   | 0         |
| 1   | 1   | 1         |
	IMPLICATION - IMPLIES (⇒)
