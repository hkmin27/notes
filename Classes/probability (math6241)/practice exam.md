**Problem 1.** Choose a random variable $X$ of which probability density function is 
$$\rho = \begin{cases} \int_1^\infty(x\log(1+x))^{-2}\,dx/(x\log(1+x))^2 \quad &x>1,\\
0 \quad &x<1.\end{cases}$$
Now $\mathbb{E}(X) = \int_1^\infty t\,\rho(t)\,dt <\infty$. However, $\mathbb{E}(X\log(1+X)) = \int_1^\infty t\log(1+t)\rho(t)\,dt=\infty.$ $\square$

**Problem 2.** The probability density function is
$$\rho = \begin{cases}1/3 \quad &x \in [2,4] \cup [8,9],\\
0  &\text{otherwise}.\end{cases}$$
Thus $\mathbb{E}(X) = \int t\,\rho\,dt = 29/6$, $\mathbb{E}(X^2) = \int t^2\,\rho\,dt = 91/3$.
Thus $Var(X)=\mathbb{E}(X^2)-\mathbb{E}(X)^2=153/3=51.$

**Problem 3.** By continuity, $\rho_X(t) \geq \epsilon$ for $|t| < \delta$. Thus
$$\int_{-\infty}^{\infty} \frac{\rho_X(t)}{t}\,dt \leq \int_{-\delta}^{\delta}\frac{\epsilon}{t$$

**Problem 6.** $F_X = \frac{\text{length of arc} }{2\pi}$ (why?)
$F_X(a,b) = $

<!--stackedit_data:
eyJoaXN0b3J5IjpbMjAzNTQwNDEzMiwxMTE0NzAzNDI4LC05OD
Y0NzIxMjAsMjAzNzMzODQ0NCwtMTQ0MTgxMTY5MiwxNTk5Njk4
MTU5LC04NDUxNDMyOTUsLTM2ODYwMzU0MCwtOTgyOTA0NjksOD
k5NjQwNDYyLDU0NTk3NjU0Myw1NzIyOTY3MzYsLTIyNDA0ODg4
OF19
-->