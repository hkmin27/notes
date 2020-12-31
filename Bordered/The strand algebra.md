### The strand algebra

---
**Definition** The strand algebra $\mathcal{A}(n,k)$ is a free $\mathbb{F}$-module with generators $\mu=(S,T,\phi)$ where $S,T \subset \{1,...,n\}$ and $|S|=|T|=k$ and $\phi:S \to T$ is a non-decreasing bijection. Let $\text{Inv}(\mu)$ be the set of inversions of $\phi$, i.e. pairs $i > j$ in $S$ such that $\phi(i) < \phi (j)$. We denote the cardinality of $\text{Inv}(\mu)$ by $\text{inv}(\mu)$ or $\text{inv}(\phi)$. 
The multiplication is given by
$$(S,T,\phi) \cdot (U,V,\psi) = \begin{cases} (S,V,\psi \circ \phi) \quad &\text{if } T=U \text{and } \text{inv}(\phi)+\text{inv}(\psi)=\text{inv}(\psi\circ\phi) \\0 &\text{otherwise}\end{cases} $$

---

In the bordered sutured setting, we need the *extended strand algebra* of $(n_1,...,n_l;k)$
$$\mathcal{A}(n_1,...,n_l;k) = \bigoplus_{k_1+\cdots+k_l=k} \mathcal{A}(n_1,k_1)\otimes\cdots\otimes\mathcal{A}(n_l,k_l)$$

We can view $\mathcal{A}(n_1,...,n_l;k)$ as a subalgebra of $\mathcal{A}(n_1+\cdots+n_l,k)$.

Let $(Z,a)$ be a finite collection of oriented arcs and a subset of $2k$ points. Denote by $Z_i$ the i-th arc and $a_i=Z_i \cap a$. The strand algebra associated to the pair $(Z,a)$ is

$$\mathcal{A}'(Z,a) = \bigoplus_{i=1}^{2k}\mathcal{A}(|a_1|,...,|a_l|;i)$$

<!--stackedit_data:
eyJoaXN0b3J5IjpbLTI2NDQ0OTM4OSwxMzg3NTQwNjI5LDM0NT
Q0ODk0Ml19
-->