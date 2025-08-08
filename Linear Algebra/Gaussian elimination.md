
A method of matrix manipulation via 3 allowed operations, with the end goal of observing an upper-right triangle.
	The shape of the end matrix ensures that you have enough information to find variable values
###### Row Operations
- Multiply a row by a scalar
	- $4R_1 → R_1$
- Add a multiple of a row to any other row
	- $2R_2 \pm R3 → R3$
- Swap two rows

If you get an error, $0 = 3$, the system has no solutions

###### Free variables
Consider the system
$$
\begin{pmatrix}
1 & 0 & 1 \\
2 & 1 & 0 \\
3 & 1 & 1
\end{pmatrix}
\cdot \begin{pmatrix}
x \\
y \\
z
\end{pmatrix}
= \begin{pmatrix}
1 \\
2 \\
3
\end{pmatrix}
$$
Gaussian elimination reduces this matrix to
$$
\begin{pmatrix}
1 & 0 & 1 & 1 \\
0 & 1 & -2 & 0 \\
0 & 0 & 0 & 0
\end{pmatrix}
$$
A free variable is one that does not correspond to a column with a pivot when reduced
	A pivot is the first nonzero entry in each row; $1, 1$ along the leading diagonal are identified as pivots, and those columns are pivot columns
	The 3rd column is not a pivot column, and so $z$ is declared a free variable

The linear equations that follow:
- $x + z = 1$
	- $x = 1-z$
- $y - 2z = 0$
	- $y = 2z$
When a free variable is identified, you should solve the other variables as terms of $z$.
The solution set is then 
$$
\{(1-z, 2z, z): z \in \mathbb{R}\}
$$
