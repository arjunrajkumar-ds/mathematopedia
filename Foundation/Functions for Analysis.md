
Choosing functions for data appropriately:
- Consider convexity
- Consider real-world situation; exponential for things like population growth
### Power-Law
A power-law function is of the form:
$$
f:(0, \infty) → (0, \infty), \quad f(x) = b \cdot x^{-a}
$$
- If data fitting an exponential distribution is log-transformed, it will create a linear plot

### Log-Log
Given a data set $(x_1, y_1), …, (x_n, y_n)$:
	log-log transforms the data to
$$
(ln(x_i), ln(y_i))
$$
- The choice of base is arbitrary
- If a log-log plot looks linear, the original data follows a power-law distribution

### Log-Lin
Given a data set $(x_1, y_1), …, (x_n, y_n)$:
	log-log transforms the data to
$$
(x_i, ln(y_i))
$$
- If a log-lin plot looks linear, the original data follows an exponential distribution

### Lin-Log
Given a data set $(x_1, y_1), …, (x_n, y_n)$:
	log-log transforms the data to
$$
(ln(x_i), y_i)
$$
- If a lin-log plot looks linear, the original data follows a logarithmic distribution

