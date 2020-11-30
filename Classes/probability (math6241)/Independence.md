---
**Problem 1.1.** 
$$\mathbb{P} (A \cap B) + \mathbb{P} (A^c \cap B) = \mathbb{P}(B)\\
 \mathbb{P} (A^c \cap B) = \mathbb{P}(B) - \mathbb{P} (A \cap B)  = \mathbb{P}(A^c)\mathbb{P}(B)$$

---

**Problem 2.1.** Since $Y$ is finite almost surely, for any $\delta$, there exists $N>0$ such that $\int_{-N}^N d\mu_Y(x) = 1-\delta$. 
This implies $\int_{-\epsilon N}^{\epsilon N} d\mu_{\epsilon Y}(x) = \epsilon(1-\delta)$

$$F_\epsilon(t) = \int_{-\infty}^{\infty}F_X(t-y)d\mu_{\epsilon Y}(y)\\ \leq$$

---

**Problem 2.2.**  Let $D := \det(A)$ Then
$$\mathbb{P}(A \text{ is of full rank}) = \mathbb{P}(D \neq 0)$$
Since $D$ is a polynomial, $\{D = 0\}$ is measure 0. Also since pdf is continuous $\mathbb{P}(D=0) = 0$.

---

**Problem 2.3.** 
$$\mathbb{E}((X-\mathbb{E}(X) + Y -\mathbb{E}(Y))\cdot(X-\mathbb{E}(X) + Y -\mathbb{E}(Y))) = Cov(X)+Cov(Y) + 2\mathbb{E}((X-\mathbb{E}(X))\cdot(Y-\mathbb{E}(Y)))$$

$$\mathbb{E}((X-\mathbb{E}(X))\cdot(Y-\mathbb{E}(Y))) = \mathbb{E}(X)\mathbb{E}(Y) - 2\mathbb{E}(X)\mathbb{E}(Y)+\mathbb{E}(X)\mathbb{E}(Y) = 0$$

---

**Problem 2.4.** 
$$F_{\alpha X}(t) = \mathbb{P}(\alpha X\leq t) = \mathbb{P}(X\leq t/\alpha) = F_X(t/\alpha)$$

$$F_{\alpha X}(t) = \int_{-\infty}^t\rho _{\alpha X}(x) = \int_{-\infty}^{t/\alpha}\rho _{X}(x) = F_X(t/\alpha)$$

$$\int_{-\infty}^{t/\alpha}\rho _{X}(x) = \int_{-\infty}^t\alpha^{-1}\rho_X(u/\alpha)du$$

---

**Problem 4.1.** 
$[\Rightarrow]$: This is true. Let $A \in \Sigma_Y$. Then there is a Borel set $B$ such that  $A = Y^{-1}(B) = X^{-1}f^{-1}(B) \in \Sigma_X$.
$[\Leftarrow]$: ???

**Problem 4.2.**
$[\Leftarrow]$:  Suppose $X_1, ... , X_n$ are mutually independent. Then 
$$\begin{aligned}
	\mathbb{P}(X_{k+1}\leq t \mid (X_1,...,X_k)\in R') &= \frac{\mathbb{P}(X_{k+1}\leq t  \cap (X_1,...,X_k)\in R')}{\mathbb{P}((X_1,...,X_k)\in R')} \\
	&=\frac{\mathbb{P}(X_{k+1} \leq t) \mathbb{P}( (X_1,...,X_k)\in R')}{\mathbb{P}((X_1,...,X_k)\in R')} \\
	&=\mathbb{P}(X_{k+1} \leq t)
\end{aligned}$$
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTExODA2NzE2NjIsMTAzMTA2Mzc5LDExMT
I3MjY2NDEsODkxMjczNzM3LC0zNjEwMzc3MzcsNDA3MzUzNjU1
LDE3MTY2ODQwNjcsLTgwNjM3NjkyOCwtMjIxNTk2NjUwLC0xMT
I1MTQyODIyLC0zNTk5NjA0OSw0NzIwMzIwMDYsMTI3MzMxODIx
M119
-->