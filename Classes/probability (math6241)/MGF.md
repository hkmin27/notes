---
**Problem 2.1.** 
$$\begin{aligned} 
M_X(t) &= \int_a^b \exp(ts)\frac{1}{b-a}\,ds\\
&=\frac{\exp(bt) - \exp(at)}{t(b-a)}
\end{aligned}$$

---
**Problem 2.2.** 
Claim. $M_X^{(j)}(0) = \mathbb{E}(X^j)$.

Now if $M_X(t) = \exp(f(t))$ where $f(t) = \sum_{i=3}^\infty a_i t^i$, then $M_X(t)' = M_X(t)'' = 0$. This implies that 
$$V(X) = \mathbb{E}(X^2) - \mathbb{E}(X)^2=0.$$
Therefore, $\mathbb{P}(X = 0)=1$.  

---

**Problem 3.1.**  Let $Y := X -\mu$. Then 
$$\begin{aligned}
\phi(t) &= \mathbb{E}(\exp(it^T(Y+\mu)))\\
&=
\end{aligned}$$

---

**Problem 3.2.**  independent $\Rightarrow$ uncorrelated: trivial.
For the other direction,  assume $\mu=0$. From Proposition 3.11, we have $\rho_X(t) = c\exp(-\frac12 t^T\Sigma^{-1} t)$. Since $\Sigma$ is diagonal, we have
$$\rho_X(t) = \rho_{X_1}(t_1) \cdots \rho_{X_n}(t_n)$$
Thus $X_1,\cdots,X_n$ are independent.

---
<!--stackedit_data:
eyJoaXN0b3J5IjpbODYyMDQzMjczLC0xMjA5ODY0NTc3LDQzNT
U3MDY0LC0xMjU2NjI2NjgzLDkwMjQzMzE1OCwxMTAyMjU0ODg0
XX0=
-->