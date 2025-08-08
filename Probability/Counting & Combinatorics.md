##### Counting 
The `multiplication rule` provides a basic way to count the number of outcomes in an experiment
	An experiment consisting of 2 sub-experiments, A & B. 
	A has $a$ possible outcomes, and B has $b$ possible outcomes. The whole experiment then has $ab$ possible outcomes
		![[Pasted image 20250226122128.png]]


##### Multiplication rule
Consider a compound experiment consisting of two sub-experiments, $A$ & $B$. Each sub-experiment has its own set of discrete possible outcomes, $a$ & $b$. 
	The multiplication rule states that the compound experiment has $a\cdot b$ possible outcomes
This rule generally holds for sampling with replacement. If the set of outcomes decreases as outcomes occur, then the number of all possible outcomes is instead obtained by multiplying the number of reducing outcomes

Why?
	Consider the set of possible outcomes - 
		$[a_1, b_1], [a_1, b_2], ..., [a_n, b_m]$
	This can be visualised with a tree diagram, where $n$ possible outcomes of $A$ are mapped out, then branch out to the $m$ possible outcomes of $B$
		![[Pasted image 20250715142408.png]]
	In this example where $n = 3, m = 4$, the compound experiment has 12 possible outcomes
###### Examples -
- Suppose 10 people are running a race. Ties are not possible & all 10 will finish, therefore each runner will have a placement. How many possibilities are there for $1^{st}, 2^{nd}, 3^{rd}$ place?
	Mapping this out - event $A$ has 3 outcomes; $a_1, a_2, a_3$ representing podium placements. Event $B$ has outcomes that decrease as event $A$ occurs - 10 racers are eligible for $1^{st}$ place, but then only 9 can get $2^{nd}$ and 8 can obtain $3^{rd}$
	$\therefore$ the number of possible outcomes is $10 \cdot 9 \cdot 8 = 720$ 


##### Sampling with replacement
Consider making $k$ choices from $n$ objects, with replacement
- $n^k$ possible outcomes

##### Sampling w/o replacement
Making $k$ choices from $n$ objects without replacement
- $n \cdot (n-1) … (n-k+1)$ 
	- E.g. choosing 3 executive positions from a club of $n$ people
		${n\choose 3}$ → $\frac{n(n-1)(n-2)}{3!}$

##### Permutations
- A permutation is an arrangement of chosen objects in some order. E.g. `3,5,1` is a permutation of `1, 3, 5`
- Equivalent to sampling without replacement → you choose positions that objects take, and they appear only once

###### Birthday problem
- $k$ people in a room
- Each person’s birthday is equally likely to be any date & i.i.d

This is a sampling with replacement problem, since 2 people may have the same birthday. 
$\therefore$ naive probability is that there are $365^k$ ways to assign a birthday
- But this doesn’t work, since 2 different, or more people could share the same birthday
- Instead, consider the complement;
Number of ways to assign birthdays to $k$ people such that no two people share a birthday
![[Pasted image 20250225122430.png]]

