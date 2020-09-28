**Problem 1.** Choose a random variable $X$ of which probability density function is 
$$\rho = \begin{cases} \int_1^\infty(x\log(1+x))^{-2}\,dx/(x\log(1+x))^2 \quad &x>1,\\
0 \quad &x<1.\end{cases}$$
Now $\mathbb{E}(X) = \int_1^\infty t\,\rho(t)\,dt <\infty$. However, $\mathbb{E}(X\log(1+X)) = \int_1^\infty t\log(1+t)\rho(t)\,dt=\infty. \quad \square$ 

**Problem 2.** The probability density function is
$$\rho = \begin{cases}1/3 \quad &x \in [2,4] \cup [8,9],\\
0  &\text{otherwise}.\end{cases}$$
Thus $\mathbb{E}(X) = \int t\,\rho\,dt = 29/6$, $\mathbb{E}(X^2) = \int t^2\,\rho\,dt = 91/3$.
Thus $Var(X)=\mathbb{E}(X^2)-\mathbb{E}(X)^2=153/3=51. \quad \square$ (제곱안함)

**Problem 3.** By continuity, $\rho_X(t) \geq \epsilon > 0$ for $|t| < \delta$. Thus
$$\mathbb{E}(\frac{1}{|X|}) = \int_{-\infty}^{\infty} \frac{\rho_X(t)}{|t|}\,dt \geq \int_{-\delta}^{\delta} \frac{\epsilon}{|t|}\,dt = \infty. \quad\square$$

**Problem 4.** Suppose $X$ is not $\infty$ a.e. Then there is $c > 0$ such that 
$$\mathbb{P}\{X < c\} > 0.$$

Suppose $A := \{X < c\}$. We claim that $A \subseteq \bigcap\{\xi_n < c\}$ for all but finitely many n. Suppose not. Then there is $x \in A$ such that for infinite subset of $\mathbb{N}$, $x \notin \{\xi_n < c\}$, which implies that $\limsup \xi_n(x)>c$. Therefore, $\mathbb{P}\{\bigcap\{\xi_n< c\}\} > 0$ for all but finitely many $n$. Since $\xi_i$ are i.i.d, $\mathbb{P}\{ \bigcap\{\xi_n< c\}\} = \prod \mathbb{P}\{\xi_n< c\} = \prod \mathbb{P}\{\xi_1< c\} > 0$. Thus $\mathbb{P}\{\xi_n< c\} = 1$ for all $n$. Thus $X < c$ almost everywhere. 
Now suppose 
$$c := \inf_d \mathbb{P}\{X < d\} > 0$$ 
By the argument above, we have $X < c+1/n$ almost everywhere. Thus $c-1/n < X < c + 1/n$ almost everywhere for all $n$. Therefore, $X = c$ almost everywhere.

**Problem 5.** 

**Problem 6.** $X$ is uniformly distributed on the unit circle. Thus we have 
$$F_X(a.b) = (\text{length of arc contatined in (x,y) $\leq$ (a,b)})/{2\pi}. \quad \square$$

**Problem 7.** The probability density functions are
$$\begin{aligned}\rho_1 &= \begin{cases} 1/2 \quad &t \in [1,3] \\ 0 \quad \text{otherwise} \end{cases}\\
\rho_2 &= \begin{cases} 1/2 \quad &t \in [1,2] \cup [4,5] \\ 0 \quad \text{otherwise} \end{cases}\end{aligned}$$

Let $Z := X_1 + X_2$. Since $X_1$ and $X_2$ are independent, $\mathbb{P}\{Z=z\} = \sum_t\mathbb{P}\{X_1 = t \;\&\; X_2 = z-t\} = \sum_{t}\mathbb{P}\{X_1 = t \} \mathbb{P}\{ X_2 = z-t\}$. Thus, 
$$\begin{aligned}\rho_{Z}(z) &= \int_{-\infty}^{\infty} \rho_1(t) \rho_2(z-t) \, dt\\
&=\int_1^3 \frac{1}{2} \rho_2(z-t)\,dt \end{aligned}$$

Now $\rho_2$ is nonzero if $1 \leq z-t \leq 2$ or $4 \leq z-t \leq 5$. Thus we have

$$\rho_{Z}(z) = \begin{cases}
	0 \quad &z \leq 2 \text{ or } z \geq 8\\
	\int_1^{z-1} \frac{1}{4}\,dt = \frac{z-2}{4}\quad &2 \leq z \leq 3\\
	\int_1^2 \frac{1}{4}\,dt = \frac{1}{4} \quad &3 \leq z \leq 4\\
	\int_{z-3}^2 \frac{1}{4}\,dt = \frac{5-z}{4}\quad &4 \leq z \leq 5\\
	\int_4^{z-1} \frac{1}{4}\,dt = \frac{z-5}{z} \quad &5 \leq z \leq 6\\
	\int_4^5 \frac{1}{4}\,dt = \frac{1}{4} \quad &6 \leq z \leq 7\\
	\int_{z-3}^5 \frac{1}{4}\,dt = \frac{8-z}{4} \quad &7 \leq z \leq 8 \quad \square\\	 
	\end{cases} $$


<!--stackedit_data:
eyJoaXN0b3J5IjpbMTM1MDMxOTY0OSwyNzA2ODM5MjMsLTcxMD
UyMTI5MywxMDQyODMzNzkyLC0xOTk4NjMzMDU0LC0xODgzNTYy
NzY0LDMxNjk2OTM2NiwtNjcxOTYzMTQ3LC0xOTA4ODE4OTYyLC
04Njg3MDMwNTgsLTE1NDk4Nzg2MDgsMjA2NjIzMjY1MywyMDM0
OTQ3OTExLC0xMTk0MjQ0OTMwLC0xNjAwNjAwNzEsNTM3MjQyNz
QxLC03NDA5NjkyMDksMTExNDcwMzQyOCwtOTg2NDcyMTIwLDIw
MzczMzg0NDRdfQ==
-->