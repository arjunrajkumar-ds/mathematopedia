##### Naive definition
- Obtained by first finding the total number of outcomes via [[Counting & Combinatorics]]
- Then find expression for choosing the desired outcome of the experiment & divide
	- Requires symmetry + equally likely outcomes
	- Can be adjusted for overcounting iff symmetric

##### Non-naive definition
- Makes use of axioms to outline how we want probability-math to behave

`General definition of probability`
	A probability space consists of sample space $S$ & a `probability function` $P$
		$P$ takes an event $A \subseteq S$ & returns $P(A)$
			$\subseteq$ → A is a subset of B + A could $=$ B
		$P(A)$ → real number $[0, 1]$
	$P$ must satisfy the 2 axioms:
1. $P(\varnothing) = 0, \quad P(S) = 1$
2. If $A_1, A_2, …$ are disjoint (mutually exclusive) events;
	$$P(\bigcup^{\inf}_{j=1}A_j) = \Sigma^{\inf}_{j=1}P(A_j)$$
		LHS → Probability of all disjoint events
		RHS → Sum probability of individual events

##### Properties derived from axioms
1. $P(A^C) = 1 - P(A)$
2. If $A \subseteq B$, then $P(A) \leq P(B)$
3. $P(A \cup B) = P(A) + P(B) - P(A \cap B)$ 
		`inclusion-exclusion`![[Pasted image 20250226201215.png]]








![[Pasted image 20250223140122.png]]

