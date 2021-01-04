### $A_\infty$-modules
*$A_\infty$-algebra* over $\mathbb{F}$ is a pair $\mathcal{A}=(A,\{\mu_i\})$ where $A$ is a graded $\mathbb{F}$-module and the $\mu_i$ are a sequence of multiplication maps

$$\mu_i:A^{\otimes i} \to A[2-i]$$

for $i 	= 1, 2, ...$ satisfying 

$$\sum_{i+j=n+1} \sum_{l=1}^{n-j+1} \mu_i(a_1 \otimes \cdots \otimes a_{l-1} \otimes \mu_j(a_l \otimes \cdots \otimes a_{l+j-1})\otimes a_{l+j} \otimes  \cdots \otimes a_n) = 0$$

for any $n$. There is also a unital element $1 \in A$ for which $\mu_2(a,1)=\mu_2(1,a)=a$ for all $a \in A$ and $\mu_i$ vanishes on i-tuples containing $1$ for $i \neq 2$. Here, $A[n]$ is a module $A$ with grading shifted *down* by $n$. Thus $\mu_1$ is a differential and $\mu_2$ is a multiplication.

___
**Definition.** Let $\mathcal{A}$ be a unital $A_\infty$-algebra over $\mathbb{F}$ and $\mathcal{I}$ the subalgebra of idempotents with orthogonal basis $\{I_i\}$ satisfying $\sum I_i = 1 \in \mathcal{A}$.  A (right unital) $A_\infty$-module over $\mathcal{A}$ is a graded module $M$ over  the base ring $\mathcal{I}$

$$M_{\mathcal{A}} := \bigoplus_i M \cdot I_i$$

together with a family of homogeneous maps

$$m_i: M \otimes A^{\otimes i-1} \to M[2-i]$$
___

### Type D-structure

<!--stackedit_data:
eyJoaXN0b3J5IjpbMjQ4NDg2Mzg3LDU3Mjg5NjE1MywyMzM3MT
kzNCw0NzEzMTcwNzIsNDg5MTM3NDY0LDYzNDgwMjIxMywtMjAy
ODk3NTU1LDczMDk5ODExNl19
-->