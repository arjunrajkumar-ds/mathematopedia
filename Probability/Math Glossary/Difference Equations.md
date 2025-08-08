
A `difference equation` describes a sequence of numbers recursively in terms of previously appearing terms in the sequence.

A `Fibonacci sequence` is a classic example, where 
$$
a_i = a_{i-1} + a_{i-2}, \quad i \geq 2
$$
- The $i^{th}$ term in the sequence depends on the two prior occurrences in the sequence

There are infinitely many such sequences, but they are uniquely determined when after the `initial conditions` / `boundary conditions` are specified; $a_0$ & $a_1$.

Difference equations often come up when applying the [[Law of Total Probability]]. Here, I will show how to solve difference equations of the form
$$
p_i = p \cdot p_{i+1} + q \cdot p_{i-1}, \quad p \neq 0, q=1-p
$$
1. ‘Try’ a solution of the form $p_i = x^i$. Plugging this in:
$$
x^i = p \cdot x^{i+1} + q \cdot x^{i-1}
$$
	#todo: Check how the equation ‘reduces’
	This reduces to form the `characteristic equation`:
$$
px^2 - x + q = 0
$$
2. The solution to the difference equation depends on whether the characteristic equation has $1$ or $2$ distinct roots
	a. If there are $2$ distinct roots $r_1, r_2$:
		The solution is of the form 
$$
p_i = a \cdot r_1^i + b \cdot r_2^i
$$
	b. If there is $1$ distinct root $r$:
		The solution is of the form
$$
p_i = a \cdot r^i + b \cdot r^i
$$
3. Find the roots to the difference equation to obtain the general solution - when two points in the sequence are known, $a$ & $b$ can be specified and a specific solution can be obtained

To find roots, use the determinant; 
