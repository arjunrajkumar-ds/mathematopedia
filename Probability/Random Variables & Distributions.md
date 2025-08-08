
The introduction of the concept of a random variable allows us to quantify uncertainty & summarise the results of an experiment. 

>[!tip] Definition

Given an experiment with sample space $S$, a `random variable` is a <u>function</u> from $S$ to the real numbers $\mathbb{R}$. 
That is, an rv $X$ assigns a numerical value $X(s)$ to each possible outcome $s$ of an experiment. 
The mapping of numerical probability values is deterministic - $X(s_i)$ will always output the same value, and the randomness comes from the randomness of the experiment, described by its distribution. 

>[!tip] E.g. Coin Tossing 

Consider tossing a fair coin twice, with sample space; 
- $S = \{HH, HT, TH, TT\}$

Since random variables capture a certain outcome of the experiment, some examples are:
- $X$ is the number of heads. Therefore, mapping outcomes as a function looks like:
$$
X(HH) = 2, \quad X(HT)=X(TH) = 1, \quad X(TT)=0
$$
- $Y$ is the number of tails. This can be represented as the inverse of the function above, or in terms of $X$;
$$
Y = 2 - X(s)
$$

##### Probability Mass Functions & Distributions
Discrete random variables are one of the two types; the other are continuous r.v.s. 

>[!tip] Definition




###### Gambler’s Ruin
- Two gamblers, $A$ & $B$, make a sequence of $1 bets. In each bet; 
	- $A$ has probability $p$ of winning
	- $B$ has probability $q = 1-p$ of winning
	- $A$ starts with $i$ dollars
	- $B$ starts with $N - i$ dollars
		- The total wealth between the two remains constant - $1 goes from one player to the other each bet
	This can be visualised as a [[Random Walk]] on the integers between $0$ & $N$ - where $p$ is the probability of moving right in a given step, & $q$ moves left. 
	The game ends when the random walk reaches either $0$ or $N$. What is the probability that $A$ wins the game?
		![[Pasted image 20250715194651.png]]
	


#todo - after chapter 2, consider how to express the Gambler’s ruin problem in these scenarios
	![[Pasted image 20250715194049.png]]

