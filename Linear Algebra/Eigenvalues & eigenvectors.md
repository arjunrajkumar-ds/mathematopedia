The defining equation for both eigenvalues and eigenvectors is :
$$
Ax = \lambda x
$$

#### Eigenvalues
Eigenvalues $\lambda_i$ are found by solving the characteristic equation
$$
(A-\lambda I)x = 0
$$
- While $x=0$ is a constant solution, $x$ is nonzero by definition, so this is solved to find any $\lambda_i$ such that this equation holds
- If $(A-\lambda I)$ has an inverse, this equation reduces to nothing, so we need that quantity to not be invertible. This occurs iff $$det(A-\lambda I) = 0$$ and this is the equation to solve. It will result in a polynomial 

#### Eigenvectors
Eigenvectors correspond to an eigenvalue, & can also be used to verify correctness
	Multiplying a matrix by an eigenvector always results in a scalar multiple of that eigenvector
To find eigenvectors, use the characteristic equation, but now plug in values of $\lambda_i$.

E.g.
$$
\begin{pmatrix}
-2 & 2 \\
2 & -2
\end{pmatrix}
\cdot \begin{pmatrix}
x_1 \\
x_2
\end{pmatrix}
=0
$$
[[Gaussian elimination]] is used to find solutions to this equation:
$$
\begin{pmatrix}
-2 & 2 \\
0 & 0
\end{pmatrix} \cdot
\begin{pmatrix}
x_1 \\
x_2
\end{pmatrix} =0
$$
- Since $-2$ is the first nonzero entry in a row, $x_1$ is a pivot column → $x_2$ is a free variable
- $-2x_1 + 2x_2 = 0$ → $x_1 = x_2$
$\therefore$ the eigenvector solution set is $\begin{pmatrix}t \\t\end{pmatrix}: t \in \mathbb{R}$ 
	Check correctness by choosing any value & multiplying & confirm that you get a scalar multiple of the chosen eigenvector

###### Properties
- Eigenvectors are nonzero by definition