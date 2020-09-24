**Problem 1.1.** Prove Proposition 1.7 in the lecture note.
**Solution.** We first need the following lemma.

**Lemma.** If $A_{i+1} \subseteq A_i$, then 
$$\mathbb{P}(\bigcap_{i=1}^\infty A_i) = \lim_{i\to\infty}{P}(A_i)$$
**Proof.** From **Problem 1.1.** in measure theoretic foundation, we have
$$\mathbb{P}(\bigcup_{i=1}^\infty A^c_i) = \lim_{i\to\infty}{P}(A^c_i)\\
1-\mathbb{P}(\bigcap_{i=1}^\infty A_i) = 1-\lim_{i\to\infty}{P}(A_i) \quad \square$$

If $a_1 \leq a'_i$, we have $\{X_i \leq a_i \} \subseteq \{X_i \leq a'_i\}$. Thus the first item follows from the definition of measure. (It's not left continuous since $\bigcup A_i = (-\infty, a)$)
If $a^m \downarrow a$, then we have $A_{m+1}:=\{X_i \leq a^{m+1}_i \} \subseteq \{X_i \leq a^m_i\}$ and $\lim_{i\to\infty} A_i = \{X_i \leq a_i\}$. Now the second item follows from **Lemma**.
If $a_i \to \infty$ for all $i$, then we can find a monotone increasing subsequence for all i. Relabel it as $a_i$. Now apply **Problem 1.1** in measure theoretic foundation and we obtain the third item. $-\infty$ is similar.
 
 **Problem 5.3** Prove that a random variable X is subexponential if and only if

$$\sup{\frac{(\mathbb{E}|X|^p)^{1/p}}{p}} < \infty$$

Similarly, prove that a random variable X is subgaussian if and only if
$$\sup{\frac{(\mathbb{E}|X|^p)^{1/p}}{\sqrt{p}}} < \infty$$
 **Solution.** We have
 $$\mathbb{E}|X|^p = \int_0^\infty \mathbb{P}\{|X|^p\geq t\}\,dt$$
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTEzMTUyMzYzMzksLTE2NDYwNzcxNjQsLT
E2NTU4MzMzNTcsLTg4NzE1MjE2MiwtMTYyODM4MTA1OCwtMjU3
NjU1MTg2XX0=
-->