
###### Identity matrix
The $n \times n$ matrix $I_n$ is defined with $i_{ii} = 1$ & $i_{ij}=0$ for $i \neq j$ 
- Known to be useful as the multiplicative identity for multiplication; the matrix product of $A$ with $I$ is $A$

###### Matrix inverse
- Only square matrices have inverses

The definition of matrix invertibility is that $A$ is invertible if there exists a $B$ such that $$ BA = I$$
The inverse of an invertible square matrix is:
$$
A = \begin{pmatrix}
a & b \\
c & d
\end{pmatrix}
, \quad A^{-1} = \frac{1}{det(A)}\cdot \begin{pmatrix}
d & -b \\
-c & a
\end{pmatrix}
$$

###### Matrix determinant
The determinant of a square matrix tells us if it is invertible. 
- If $det(A) \neq 0$, then $A$ has an inverse
- $det(AB) = det(A) \cdot det(B)$
- $det(I) = 1$

###### Diagonal matrices
- Diagonal matrices can be powered trivially
A square matrix $A$ is `diagonalisable` if there’s an invertible $P$ & diagonal $D$ such that 
$$
A = PDP^{-1}
$$
- $D$ is a diagonal matrix where the entries correspond to eigenvalues of $A$
- $P$ is an $n \times n$ matrix where the columns correspond to eigenvectors of $A$
###### Properties
- $(AB)C = A(BC)$
- $(k+j)A = kA + jA$
- $(kA)B = k(AB) = A(kB)$
- $A(B+D) = AB + AD, (B+D)C = BC+DC$

If $A$ is invertible with inverse $B$; $BA = I$, then $AB = BA = I$ & $B$ is unique

