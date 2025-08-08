
##### Definition 
A function $f: X → Y$ is made up of:
- a set $X$ that represents the domain of $f$
- a set $Y$ that represents the codomain of $f$
- a function rule that maps exactly one $X$ to one $Y$

A function’s domain & codomain outline all possible values that the input & output sets can take, respectively.

A function’s <b>image</b> is similar to the codomain, but showing real boundaries. The image is a (strict) subset of the codomain
	E.g. $f: \mathbb{R} → \mathbb{R} \quad f(x) = x^2$
	$f$ is a real-valued function, having $\mathbb{R}$ as both domain & codomain
	However, when plotting the graph of $f$, we can observe that $f(x)$ is never negative
```functionplot
---
title: f(x)
xLabel: x
yLabel: y
bounds: [-10,10,-10,10]
disableZoom: false
grid: true
---
f(x) = x^2
```
So the image is $[0, \infty]$ 

###### MAT9004 Convention
- If the codomain is not specified, is is assumed by convention to be the image

##### Function Zeroes
A function’s roots (zeroes) are where the function’s plot crosses the $x$-axis
	All points $x \in X$ with $f(x)=0$

The zeroes of a <u>quadratic function</u> $f(x) = x^2 + ax + b$ are:
$$
x= -\frac{a}{2} \pm \sqrt{\frac{a^2}{4} - b}
$$
- The zeroes exist in $\mathbb{R}$ iff $a^2 \geq 4b$ 
	

##### Inverse Functions
A function $g: Y → X$ is the inverse of $f: X →Y$ iff:
- $g(f(x)) = x$
- $f(g(y)) = y$
for all $x \in X, y \in Y$

Inverses don’t always exist, but if it does, they are always unique

##### Bijectivity
A function $f:X → Y$ is:
- <b>Injective</b> if distinct inputs are mapped to distinct outputs
	- $f(x_1) \neq f(x_2)$
	- One-to-one mapping of values
	- No two $x_i$ equal the same $f(x)$ 
- <b>Surjective</b> if the image of the function $f$ is equal to its codomain
	- Surjectivity depends on how the codomain is defined
		E.g. $f: \mathbb{R} → \mathbb{R}, f(x) = x^2$
		The codomain is $\mathbb{R}$, while the image is $[0, \infty]$
		This function is not surjective, but if the codomain was redeclared to be the image, it would be
	- Formally; $f$ is surjective if for every element of the codomain, there exists at least one $a$ such that $f(a) = b$: each output is mapped onto by an input
	- To remember: ‘onto’ - the entire codomain is being effectively mapped onto

A function that displays both injectivity & surjectivity is <b>bijective</b> and bijective functions have inverses.

##### Convexity
- A function is <i>convex</i> if for any two points on the plot, a straight line connecting those points lies entirely above the plot
	- Straight lines are convex
	
	$f$ is convex iff $f’’(x) \geq 0$ over all $x$
		A local minimum of a convex function is the global minimum

- A function is <i>concave</i> if for any two points, a straight line lines entirely below the plot
	Convexity informs the type of function you should try use to model something

	$f$ is concave if $f’’(x) \leq 0$ over all $x$
		A local maximum of a concave function is the global maximum
##### Increasing / Decreasing functions
Functions can be increasing or decreasing over an interval. When examined at a single point, this property doesn’t apply
	A function $f$ <b>increases</b> on an interval if as $x$ grows, the value $f(x)$ increases.
		A positive [[derivatives]] over an interval indicates that the function is increasing over that interval
	A function **decreases** on an interval if as $x$ goes down, the value $f(x)$ decreases.
		A negative [[derivatives]] over an interval indicate that $f(x)$ is decreasing over that interval

##### Stationary points
A function $f$ has a stationary point at point $s$ where $f’(s) = 0$

##### Local extrema - maximum & minimum
To consider:
1. Singular points where $f’(x)$ doesn’t exist
2. Endpoints of the domain
3. Stationary points where $f’(x)=0$

###### Derivative test
The $f’$ sign test provides a way to confirm whether a function $f$ has a local maximum/minimum at point $s$
- If $f$ is differentiable at $s$, with $f’(s) = 0$:
	If $f’(x)$ makes a sign change (positive → negative) at $x = s$ as $x$ moves from left to right, then $s$ is a local maximum
	Conversely, if $f’(x)$ makes a sign change (negative → positive) at $x=s$, then $s$ is a local minimum
Check the sign of the derivative at $s$ to left & right of the stationary point. 

###### Second derivative test
The $f’’$ test gives another way to verify local extrema
	If $a$ is a stationary point of $f$ & $f’’(a)$ exists:
		- $f$ has a local minimum at $x=a$ if $f’’(a)>0$
			- $f’’(a)$ positive → minimum
		- $f$ has a local maximum at $x=a$ if $f’’(a)<0$.
			- $f’’(a)$ negative → maximum
	- If $f’’(a)=0$, then this test is inconclusive

##### Global extrema
![[Pasted image 20250720125519.png]]

	

### Linear functions
A linear function is of the form:
$$
f: \mathbb{R} → \mathbb{R}, \quad f(x) = m \cdot x + b
$$
- $m$ is the slope
- $b$ is the intercept at $f(0)$

### Polynomial functions
A polynomial function (of degree $n>0$) is of the form:
	$f: \mathbb{R} → \mathbb{R}$ 
$$
f(x) = a_n \cdot x^n + a_{n-1} \cdot x^{n-1} + ... + a_1x + a_0
$$
- $f(x) = 0$ is a polynomial of degree $-\infty$ 

	In theory, there always exists a polynomial of degree n that achieves perfect interpolation, passing through all data points. It can be solved with a system of $n+1$ linear equations, with a corresponding number of unknowns

### Exponential Functions
An exponential function is of the form:
$$
f: \mathbb{R} → \mathbb{R}, \quad f(x) = b\cdot a^x, a>0, b \neq 0
$$
	Properties:
		- No zeroes for standard conditions
		- Injective for $a \neq 1$
		- Surjective for all $\mathbb{R}, b\neq 0$
		- Convex for $b>0$
		- Concance for $b<0$

### Logarithmic Functions
A logarithmic function is of the form:
$$
f(x) = log_a(x), \quad a>0, a \neq 1
$$
- It is the inverse to $f(x) = a^x$
	Properties:
		- $a^{log_a(x)} = x$
		- $log_a(a^x) = x$

Since f(t) represents the price of the stock at a point in time t, the amount of money that can be made by buying/selling at various points throughout those 3 years can be obtained by using the value of the image of the function at t
	Buys are represented by the how much money is being invested at that time * the image of the function at the time you decide to buy
		B * f(t)
	Similarly, sells are represented by
		- S * f(t)
E.g. 
- Buy $30,000 at 6 months (t=.5)
- Buy $10,000 at 12 months (t=1)
- Sell $20,000 at 24 months (t = 2)
