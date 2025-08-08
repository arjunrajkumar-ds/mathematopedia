
Let $f: D → \mathbb{R}, [a, b] \subseteq D \subseteq \mathbb{R}$
	The definite integral of $f$, measured between $a$ & $b$ is the `signed area` bounded by $f$, the $x$-axis & the vertical lines at $x=a, x=b$ 

The indefinite integral:
$$
\int f(x) \quad dx = F(X)
$$
- Is technically a family of functions - an indefinite integral by itself doesn’t represent any particular ‘thing’

##### Fundamental theory of calculus (FTC)
If $F$ is any antiderivative of $f$:
$$
\int_a^b [f(x) \quad dx] = F(b) - F(a)
$$

##### Properties
- Linearity
	$$
\int_b^a(f(x) + g(x)) \quad dx = \int f(x) dx + \int g(x)dx
	$$


##### Rules
- Linearity
$$
\int^b_a[f(x) \pm g(x)]dx = \int_a^b f(x) dx \pm \int_a^b g(x)dx
$$
- Constant
$$
\int^b_a c\cdot f(x)dx = c \cdot \int^b_af(x)dx
$$
- Reciprocal
$$
\int^b_a\frac{1}{x}dx = ln|x| + c
$$
- Exponential
$$
\int^b_a e^x dx = e^x + c
$$
$$
\int^b_a a^x = \frac{a^x}{ln(a)}+c
$$
- Logarithm
$$
\int ln(x) dx = x\cdot ln(x) - x + c
$$
