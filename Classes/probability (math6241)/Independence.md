---
**Problem 1.1.** 
$$\mathbb{P} (A \cap B) + \mathbb{P} (A^c \cap B) = \mathbb{P}(B)\\
 \mathbb{P} (A^c \cap B) = \mathbb{P}(B) - \mathbb{P} (A \cap B)  = \mathbb{P}(A^c)\mathbb{P}(B)$$

---

**Problem 2.1.** Since $Y$ is finite almost surely, for any $\delta$, there exists $N>0$ such that $\int_{-N}^N d\mu_Y(x) = 1-\delta$. 
This implies 

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

$$F_{\alpha X}(t) = \int_{-\infty}^t\rho _{\alpha X}(t) = \int_{-\infty}^{t/\alpha}\rho _{X}(t) = F_X(t/\alpha)$$

$$\int_{-\infty}^{t/\alpha}\rho _{X}(t) = \int_{-\infty}^t\alpha^{-1}\rho_X(u/\alpha)du$$

---
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTE2NzY1Mjk4NzcsMTcxNjY4NDA2NywtOD
A2Mzc2OTI4LC0yMjE1OTY2NTAsLTExMjUxNDI4MjIsLTM1OTk2
MDQ5LDQ3MjAzMjAwNiwxMjczMzE4MjEzXX0=
-->