###### Relations
Broadly speaking, a relation describes an association between elements of one or more sets.
	[[Functions]] are a subset of relations

A binary relation relates two parameters. 


###### Inequalities
- When plotting a relation that involves an inequality, a good starting point is to plot the equality. Then regions that are in/out can be compared for the solution

###### Zeroes
The set of zeroes for a function $f(x,y)$ form a binary relation. They are the level sets (contour lines) such that $f(x, y) = c, \quad c=0$ 

###### Partial Derivatives
- $f_x$ → partial derivative of $f$ wrt $x$
- $f_y$ → partial derivative of $f$ wrt y
- $\triangledown f = \begin{bmatrix}f_x \\f_y\end{bmatrix}$ is the gradient vector
	- It always points in the direction of steepest increase from $(x, y)$ 

###### First order approximation
$$
f(x + \triangle x, y+\triangle y)
$$
 $$\approx f(x,y) + f_x(x, y) \cdot \triangle x + f_y(x, y) \cdot \triangle y$$

###### Stationary points
A stationary point of $f(x,y)$ is a point where boht partial derivatives are 0.
There are 3 types of stationary point:
- Local minimum
- Local maximum
- Saddle point

To find stationary points, you need to solve:
$$
\triangledown f = \begin{bmatrix}
0 \\
0
\end{bmatrix}
$$
	- Note: exponential factors can be ignored with consideration, as $e^x \neq 0$. They act as a constant and are factorised outside

###### Second partial derivatives
A [[Hessian matrix]] can be constructed with second order partial derivatives of $f(x, y)$. It’s used to diagnose stationary points

![[Pasted image 20250804184113.png]]
