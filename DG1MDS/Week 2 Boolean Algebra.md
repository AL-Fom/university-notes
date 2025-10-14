
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
