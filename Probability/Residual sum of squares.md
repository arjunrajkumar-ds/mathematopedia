A residual is the difference left over when subtracting an observation from a real value

The residual sum of squares (RSS) is a method to evaluate how well a function $f$ approximates some data points $((x_1, y_1), …, (x_n, y_n))$
	It compares the `real` value $y_i$ to the image value of $x_i$ when approximated with the function $f$. That is, it compares $y_i$ & $f(x_i)$
	The RSS is a scalar value - big numbers indicate large deviations, small numbers indicate low deviations
$$
RSS = \Sigma^n_{i=1}[y_i - f(x_i)]^2
$$

One application of the RSS is to tune parameters of the function used to approximate.
	E.g. Data: ${(0,0), (1,2), (2, 4), (3, 5)}$ is approximated with $f(x) = mx$
	$RSS = (0)^2 + (2-m)^2 + (4-2m)^2 + (5-3m)^2$
	$=14m^2 - 55m + 45$

The RSS is a quadratic function that can take on a range of values representing how high/low the deviations are. Remembering that we want this value to be as low as possible, you find extremum & find the function parameter for which RSS has a global minimum.
	$R’(m) = 28m-55$
	$R’’(m) = 28 > 0$
		This convex function $R$ has a global minimum at $m=\frac{28}{55}$

