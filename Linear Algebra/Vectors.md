A vector can be represented as a directed line segment
- The length of the line is the `magnitude`
- The orientation of the line is the `direction`

Linear algebra smoothly translates properties of 2-dimensional maths into <i>n</i> -dimensional space.

A pair of two seperate numbers, $v_1, v_2$ produce a two-dimensional vector $v$:
$$
v = \begin{bmatrix}
v_1 \\
v_2
\end{bmatrix}
$$
Vectors can be represented as:
- 2 numbers
- A coordinate point in a plane
- Arrow from the origin to coordinate
	But they actually describe a displacement; $x$ units displaced in the $x$ direction, $y$ units …

##### Linear combinations & linear independence
Linear combinations are one of the key operations with vectors. 
 - Line → Plane → Space
	- A single vector $u$ has a range of possible linear combinations $cu$, and all combinations of $cu$ form a line in coordinate space
	- All combinations of the linear combination of two vectors $cu + dv$ fill a plane
	- All combinations of the linear combinations of three vectors $cu + dv + ew$ fill three-dimensional space
- A vector $w$ is a linear combination of vectors $v_1, …, v_n$ if it can be expressed as:
		$w = a_1 \cdot v_1 + ... + a_n \cdot v_n$
- If a set of vectors $v_n$ can be expressed as a sum of some multiple of the others, they are `linearly dependent`
	- `Linear independence` occurs when the above is not true


Vectors that add to 0 lie on the same plane

##### Magnitude & Dot Products
For two vectors $v$ & $w$, the dot product is:
$$v \cdot w = v_1w_1 + ... + v_n \cdot w_n$$
The magnitude/length/norm of a vector is its dot product with itself
$$
||v|| = \sqrt{v_1^2 + ... + v_n^2}
$$
##### Orthogonality
If the dot product is $0$, it means that the vectors $v$ & $w$ are perpendicular or `orthogonal`. That is, the angle between them is $90\degree$.
- The $0$ vector is orthogonal & linearly dependent to every other vector
If a set of vectors $v_1, …, v_n$ are pairwise orthogonal, they are `linearly independent`

##### Properties
- Vector addition → $v + w$
- Linear combinations → $cv + dw$
###### Vector Addition 
$$
v = \begin{bmatrix}
v_1 \\
v_2
\end{bmatrix}, \quad w = \begin{bmatrix}
w_1 \\
w_2
\end{bmatrix} \rightarrow v+w = \begin{bmatrix}
v_1 + w_1 \\
v_2 + w_2
\end{bmatrix}
$$
Subtraction follows the same idea

###### Scalar Multiplication
$$
2v = \begin{bmatrix}
2v_1 \\
2v_2
\end{bmatrix}, \quad -v = \begin{bmatrix}
-v_1 \\
-v_2
\end{bmatrix}
$$