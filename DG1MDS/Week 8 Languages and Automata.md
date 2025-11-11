
denoted using Σ = {valid characters} it is a finite set of symbols non empty meaning you cant have Σ = {}
	you denote possible products of an alphabet by denoting it as: (product) is a word over Σ
	to represent an empty word you use the epsilon ε

an example alphabet we can have is Σ = {a,b,c,d,e,f,g,h,i,j}
where our language is L = {bad, fade, hi} as this language was made using symbols from the alphabet we can say this is a language over out alphabet
L⊆Σ* (Σ* means all possible words that can be made using the alphabet, this list is infinite as you can have {a, aa, aaa, ...})

dot operator concatenates (or glues) the letters together to form a word
for example 2+3 = 5 
2 dot 3 = 23

automata as math objects (formally) using binary as example
alphabet Σ = {0,1}
name the states q$_0$, q$_1$, q$_2$
name the set of states Q = {q$_0$, q$_1$, q$_2$}
identify initial state q$_0$
identify final states q$_1$, q$_2$
name the set of final states F = {q$_1$, q$_2$}
name the relation (set):
![[Pasted image 20251110173203.png]]