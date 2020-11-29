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
<!--stackedit_data:
eyJoaXN0b3J5IjpbMTEyNDU5MzQ2MSw5MDI0MzMxNTgsMTEwMj
I1NDg4NF19
-->