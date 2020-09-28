**Problem 1.1.** We first claim that if $A \subset B$, then $\mu(A \setminus B) = \mu(A) - \mu(B)$.  It is clear from the equality 
$$\mu(A) = \mu((A \setminus B) \cup B) = \mu(A \setminus B) + \mu(B).$$
Now we have
$$\begin{aligned}
\mu(\bigcup_{i=1} A_i)&=\sum_{i=1} \mu(A_{i+1} \setminus A_i)\\
&=\sum_{i=1} (\mu(A_{i+1}) - \mu(A_i))\\
&=\lim_{i\to\infty}\mu(A_i). \quad \square
\end{aligned}$$

**Problem 1.2.**  We will verify the 3 conditions.
- $\phi, \Omega \in S$: trivial.
- $A, B \in S \Rightarrow A \cap B \in S$: $$\bigcup_{i=1}^n A_i \cap \bigcup_{j=1}^m B_j = \bigcup_{i,j=1}^{n,m}(A_i\cap B_j).$$
- $A \in S \Rightarrow A^c \in S$: trivial. 
Also any field containing $S$ clearly has the property that any finite union of elements in $S$ should be in the field. $\square$


**Problem 1.3.** Let $n \geq 1$, Show that the following set is a semi-field.
$$S := \{ \prod_{i=1}^n (a_i,b_i]: -\infty \leq a_1,...,a_n,b_1,...,b_n \leq \infty \}. $$

**Solution.**  We will verify the 3 conditions.
- $\phi, \Omega \in S$: trivial.
- $A, B \in S \Rightarrow A \cap B \in S$: trivial.
- $A \in S \Rightarrow A^c$ is a finite union of sets in $S$: $(a_i,b_i]^c = (-\infty,a_i] \cup (b_i,\infty]$. $\square$

**Problem 2.1.**  Let $\mu_1$ be the counting measure on $\mathbb{R}$ and $\mu_2(A)=\infty$ except for $A = \phi$.
Since 
$$\bigcap_{n=1}^\infty (a - 1/n, a] = \{a\}$$
is in the Borel $\sigma$-field, the two measures do not coincide.  $\square$

**Problem 2.2.** Let $\mathcal{C}=\{\{1,2\}, \{2,3\}\}.$ Clearly $\sigma(\mathcal{C}) = 2^{\{1,2,3,4\}}$. Notice that $\mathcal{C}$ is not a $\pi$-system. Now define $\mu_1, \mu_2$ as follows.
$$\mu_1(\{i\}) = 1/4,\\\mu_2(\{1\}) = \mu_2(\{3\}) = 1/2,\, \mu_2(\{2\}) = \mu_2(\{4\}) = 0$$

**Problem 2.3.** $\mathcal{L} = \{ \phi, [-1,0], [0,1], (-\infty, -1) \cup (0, \infty), (-\infty, 0) \cup (1, \infty), \mathbb{R} \}$ is a $\lambda$-system. However, it's not a $\sigma$-field. (since $[-1,0]$ and $[0,1]$ intersect)
<!--stackedit_data:
eyJoaXN0b3J5IjpbMjcxNzkxMzE5LC0xMzI1OTYzMjc1LDE4OD
Y2Mjk4NDksMTc2NDU2MDQ0Miw2MzM2MDc1MzhdfQ==
-->