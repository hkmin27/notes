**Problem 1.** Choose a random variable $X$ of which probability density function is 
$$\rho = \begin{cases} \int_1^\infty(x\log(1+x))^{-2}\,dx/(x\log(1+x))^2 \quad &x>1,\\
0 \quad &x<1.\end{cases}$$
Now $\mathbb{E}(X) = \int_1^\infty t\,\rho(t)\,dt <\infty$. However, $\mathbb{E}(X\log(1+X)) = \int_1^\infty t\log(1+t)\rho(t)\,dt=\infty.$ $\square$

**Problem 2.** The probability density function is
$$\rho = \begin{cases}1/3 \quad &x \in [2,4] \cup [8,9],\\
0  &\text{otherwise}.\end{cases}$$
Thus $\mathbb{E}(X) = \int t\,\rho\,dt = 29/6$, $\mathbb{E}(X^2) = \int t^2\,\rho\,dt = 91/3$.
Thus $Var(X)=\mathbb{E}(X^2)-\mathbb{E}(X)^2=153/3=51.$

**Problem 3.** By continuity, $\rho_X(t) \geq \epsilon > 0$ for $|t| < \delta$. Thus
$$\mathbb{E}(\frac{1}{|X|}) = \int_{-\infty}^{\infty} \frac{\rho_X(t)}{|t|}\,dt \geq \int_{-\delta}^{\delta} \frac{\epsilon}{|t|}\,dt = \infty.$$

**Problem 6.** $F_X = \frac{\text{length of arc} }{2\pi}$ (why?)
$F_X(a,b) = $

**Problem 7.** The probability density functions are
$$\begin{aligned}\rho_1 &= \begin{cases} 1/2 \quad &t \in [1,3] \\ 0 \quad \text{otherwise} \end{cases}\\
\rho_2 &= \begin{cases} 1/2 \quad &t \in [1,2] \cup [4,5] \\ 0 \quad \text{otherwise} \end{cases}\end{aligned}$$

Let $Z := X_1 + X_2$. Since $X_1$ and $X_2$ are independent, $\mathbb{P}\{Z=z\} = \sum_t\mathbb{P}\{X_1 = t \;\&\; X_2 = z-t\} = \sum_{t}\mathbb{P}\{X_1 = t \} \mathbb{P}\{ X_2 = z-t\}$. Thus, 
$$\begin{aligned}\rho_{Z}(z) &= \int_{-\infty}^{\infty} \rho_1(t) \rho_2(z-t) \, dt\\
&=\int_1^3 \frac{1}{2} \rho_2(z-t)\,dt \end{aligned}$$

Now $\rho_2$ is nonzero if $1 \leq z-t \leq 2$ or $4 \leq z-t \leq 5$.
If $2 < z < 6$, 

$$\rho_{Z}(z) =\int_1^{z-1} \frac{1}{2} \rho_2(z-t)\,dt $$

<!--stackedit_data:
eyJoaXN0b3J5IjpbOTk3ODAxODY3LC0xNTQ5ODc4NjA4LDIwNj
YyMzI2NTMsMjAzNDk0NzkxMSwtMTE5NDI0NDkzMCwtMTYwMDYw
MDcxLDUzNzI0Mjc0MSwtNzQwOTY5MjA5LDExMTQ3MDM0MjgsLT
k4NjQ3MjEyMCwyMDM3MzM4NDQ0LC0xNDQxODExNjkyLDE1OTk2
OTgxNTksLTg0NTE0MzI5NSwtMzY4NjAzNTQwLC05ODI5MDQ2OS
w4OTk2NDA0NjIsNTQ1OTc2NTQzLDU3MjI5NjczNiwtMjI0MDQ4
ODg4XX0=
-->