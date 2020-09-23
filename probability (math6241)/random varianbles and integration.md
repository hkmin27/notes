**Problem 1.1.** Prove Proposition 1.7 in the lecture note.
**Solution.** We first need the following lemma.

**Lemma.** If $A_{i+1} \subseteq A_i$, then 
$$\mathbb{P}(\bigcap_{i=1}^\infty A_i) = \lim_{i\to\infty}{P}(A_i)$$
**Proof.** From **Problem 1.1.** in measure theoretic foundation, we have
$$\mathbb{P}(\bigcup_{i=1}^\infty A^c_i) = \lim_{i\to\infty}{P}(A^c_i)\\
1-\mathbb{P}(\bigcup_{i=1}^\infty A_i) = 1-\lim_{i\to\infty}{P}(A_i) \quad \square$$

If $a_1 \leq a'_i$, we have $\{X_i \leq a_i \} \subseteq \{X_i \leq a'_i\}$. Thus the first item follows from the definition of measure.
If $a^m \downarrow $
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTE3NDU5OTQ3NzgsLTI1NzY1NTE4Nl19
-->