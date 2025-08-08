
- `Random variables` are denoted with uppercase letters; $X, Y, Z$
- `Outcomes` or realisations of RVs are denoted by a corresponding lowercase letter; $x, y, z$

###### Distribution Functions

- A `cumulative distribution function`, cdf, is … #todo 
	It’s defined as 
$$
F(x) = Pr(X \leq x), \quad -\inf < x < \inf
$$

- Discrete RVs have a `probability mass function`:
$$
p(x) = Pr(X=x), \quad x belongsto \Omega
$$
where $\Omega$ is a discrete set

- Continuous RVs have a `probability density function`:
$$
f(x) = F'(x) = \frac{d}{dx}[F(x)]
$$
	, where
$$
F(x) = \int_{-\inf}^{x}f(t)dt
$$
	- $F(x)$ tends to 1 as $x → \inf$
	- $F(x)$ tends to 0 as $x → -\inf$

- $Pr(X>x) = 1 - F(x)$ is a `tail probability` of $X$


###### Worked Examples
