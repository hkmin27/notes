**Problem 1.1.** Prove Proposition 1.7 in the lecture note.
**Solution.** We first need the following lemma.

**Lemma.** If $A_{i+1} \subseteq A_i$, then 
$$\mathbb{P}(\bigcap_{i=1}^\infty A_i) = \lim_{i\to\infty}{P}(A_i)$$
**Proof.** From **Problem 1.1.** in measure theoretic foundation, we have
$$\mathbb{P}(\bigcup_{i=1}^\infty A^c_i) = \lim_{i\to\infty}{P}(A^c_i)\\
1-\mathbb{P}(\bigcup_{i=1}^\infty A_i) = 1-\lim_{i\to\infty}{P}(A_i) \quad \square$$

If $a_1 \leq a'_1$, we have $\{X_i \leq a_i \} \subset \{X_i \}$
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTc5NDY5NjQ4NywtMjU3NjU1MTg2XX0=
-->