### Weinstein handles

**Weinstein k-handles**
We will define a *Weinstein k-handle* as a subset of $\R^{2n} = T^*\R^k\times\R^{2(n-k)}$. Set the coordinates of the space as follows.
$$(q_1,...,q_k,p_1,...,p_k) \in T^*\R^k\\
(x_1,y_1,...,x_{n-k},y_{n-k}) \in \R^{2(n-k)}$$

Consider a symplectic structure $\omega=\sum dq_i\wedge dp_i + \sum dx_i\wedge dy_i$.
and expanding vector field $v = \sum(-q_i\partial_{q_i}+2p_i\partial_{p_i})+\frac12\sum (x_i\partial_{x_i}+y_i\partial y_i)$
corresponding Morse function $f = \sum (-\frac12q_i^2+p_i^2)+\frac14\sum(x_i^2+y_i^2)$
Now define $H := f^{-1}(-1,1) \cap$ inside of trajectories.
$(H,\omega,v,f)$ is called a *Weinstein k-handle*.

---
Check the facts

$v$ is expanding: $\mathcal{L}_v\omega = \omega$
$i_vd\omega + di_v\omega = \sum d(-q_idp_i-2p_idq_i)+\sum d(x_idy_i-y_idx_i)=\omega$
$v$ is gradient for $f$: trivial

---

**Conformal symplectic normal bundles**
Let $S$ be an isotropic submanifold of a contact manifold $(M,\alpha)$. $d\alpha$ is a symplectic structure on $\xi$. Then we define a *conformal symplectic normal bundle* as follows.
$$CSN(S) = TS^{\perp d\alpha}/TS$$

We can decompose $TM|_S$ as follows.
$$TM|_S = \xi \oplus TM / \xi = (CSN(S) \oplus TS \oplus \xi/TS^\perp) \oplus \R,$$

where $\R$ is spanned by the Reeb vector field.
Since $T(T^*S)|_S \cong TS \oplus \xi/TS^\perp$, $S$ determines $TM|_S$ except for $CSN(S)$.

**framing in 3-dimension**
We will figure out the natural framing of Legendrian surgery in 3-dimension. Let $k=n=2$.  Then the attaching sphere is $L := S^1_H = \{|q|=1,p=0\}$. Thus the contact form along $L$ is  
$$\alpha = i_v\omega = -q_1dp_1 - q_2dp_2-2p_1dq_1-2p_2dq_2,\\
\alpha \wedge d\alpha|_L = 2q_ 1dp_1 \wedge dp_2 \wedge dq_2 + 2q_2dp_2 \wedge dp_1\wedge dq_1.$$

Orient $L$ by the vector field $q_1 \partial_{q_2} - q_2\partial_{q_1}$. Then the normal orientation of $L$ is given by $(2q_1^2+2q_2^2)dp_1 \wedge dp_2$, so the framing of the surgery is given by an ordered basis $(\partial_{p_1}, \partial_{p_2})$. **(Q: why is it the surgery framing?)**
The contact framing of $L$ is given by the vector field $q_2\partial_{p_1} -q_1\partial_{p_2}$. This make one positive twist relative to the basis $(\partial_{p_1}, \partial_{p_2})$. Thus the framing of Legendrian surgery is contact framing - 1 (if it is null-homologous, $tb(L)-1$).


**Remark.** difference btw contact framing of unknot: this case has outward vf. Weinstein case has inward vf. 
<!--stackedit_data:
eyJoaXN0b3J5IjpbMTk0Nzg0OTczMCwtMTQzMDQzMjU1NywtMj
EwMjc4MjA2MywtMTUyMDMxNzQwLC02NjUxOTc4MTYsNzk4MzI2
MDc2LC0xMjcwMTk2MjQ3LDE5NTk2MDk1NzksODU4MDU1NzM1LC
0xNjQ0MjM0NzQyLDMwNjkwODU5NywtODk5MTg2NzcsMTg3Nzcy
NDQ3Miw1MjE5NzYzMTksMjAzNjU1OTcsMTEyOTQxMzQyNywtMj
E0NDAzODA2NCwtMTQyMDUyMTIxNl19
-->