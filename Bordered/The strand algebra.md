### The strand algebra

---
**Definition** The strand algebra $\mathcal{A}(n,k)$ is a free $\mathbb{F}$-module with generators $\mu=(S,T,\phi)$ where $S,T \subset \{1,...,n\}$ and $\phi:S \to T$ is a non-decreasing bijection. Let $\text{Inv}(\mu)$ be the set of inversions of $\phi$, i.e. pairs $i > j$ in $S$ such that $\phi(i) < \phi (j)$. We denote the cardinality of $\text{Inv}(\mu)$ by $\text{inv}(\mu)$ or $\text{inv}(\phi)$. 
The multiplication is given by
$$(S,T,\phi) \cdot (U,V,\psi) = \begin{cases} (S,V,\psi \circ \phi) \quad \text{if } T=U \text{and} \text{inv}(\phi)+\text{inv}(\psi)=\teinv(\psi\circ\phi)}\\0 else \end{cases} $$


---
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTEwNDk0ODg3NjAsMzQ1NDQ4OTQyXX0=
-->