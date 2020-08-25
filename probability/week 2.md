**Proposition.** $\mu^*$: outer measure on $\Omega$. Then,
$$\Sigma := \{ A \subset \Omega: A  \mu^*-measurable \}$$
is $\sigma$-field and 
$\mu^*$ is a measure on $\Sigma$

$\Sigma$



Then	
$$\mu^*(\bigcup_{i=1}^\infty A_i) \leq \sum_{i=1}^\infty \mu^*(A_i)$$
Next, for any pair of disjoint sets $B_1,B_2$ in $\Sigma$, we have $\mu^*(B_1\cup B_2) = \mu^*((B_1\cup B_2)\cap B_1) + \mu^*((B_1 \cup B_2) \cap B_1^c)$ 
so, $\mu^*$ is finitely additive on $\Sigma$. Then $\mu^*(\bigcup_{i=1}^n A_i) = \sum_{i=1}^n \mu^*(A_i)$

Let $(A_i)_{i=1}^\ifnty$ - sequence of elements from $\Sigma$. Define $A_i' := A_i \setminus \cup_{j<i} A_j$.
$A_i' \in \Sigma$, disjoint and $\cup_{i=1}^\infty A_i = \cup_{i=1}^\infty A_i'$ Pick $B \subset \Omega$
We need to check that 
$$\mu^*(B) = \mu^*(B \cap \cup_{i=1}^\infty A_i) + \mu^*(B\cap (\cup_{i=1}^\infty A_i)^c)$$
$$\mu^*(B) \leq \mu^*(B \cap \cup_{i=1}^\infty A_i) + \mu^*(B\cap (\cup_{i=1}^\infty A_i)^c)$$

For every $n$ we have 
$$\mu^*(\cup_{i\leq n} A_i' \cap B), A_n'-measurable$$
$$= \mu^*(\cup_{i\leq n} A_i' \cap B \cap A_n') + \mu^*(\cup_{i\leq n}A_i' \cap B \cap (A'_n)^c) = \mu^*(B\cap A_n') + \mu^*(B\cap \cup_{i\leq n-1} A_i')$$
$$= \cdots = \sum_{i=1}^n \mu^*(B\cap A_i')$$

#

$$\mu^*(\bigcup_{i=1}^\infty A_i \cap B) \leq \lim_{n\to \infty} \sum_{i=1}^n \mu^*(B\cap A_i') (subadditivity of \mu^*)$$

$$\mu^*(\cup_{i=1}^\infty A_i \cap B) \leq \lim_{n\to\infty} \mu^*(\cup_{i=1}^\infty A_i' \cap B)$$

at the same time, by monotonicity, 
$$\{ \mu^*(B\cap (\cup_{i=1}^\infty A_i)^c ) \leq \mu^*(B\cap (\cup_{i=1}^n A_i')^c) \}$$
$$\Rightarrow \mu^*(B) \leq \lim_{n\to\infty} [\mu^*(\cup_{i=1}^n A_i' \cap B) + \mu^*(B\cap (\cup_{i=1}^n A_i')^c = \lim_{n\to\infty} \mu^*(B)$$

We need to check that 

$$\mu^*(B) = \mu^*(B\cap \cup_{i=1}^\infty A_i) + \mu^*(B\cap (\cup_{i=1}^\infty A_i)$$
<!--stackedit_data:
eyJoaXN0b3J5IjpbNDc1ODYxOTUyLDE5MzA1MDk4MzhdfQ==
-->