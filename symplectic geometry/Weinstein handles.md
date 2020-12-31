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
We will figure out the natural framing of Legendrian surgery in 3-dimension. Let $k=n=2$.  Then 
$$\alpha = i_v\omega = $$
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTE1MjAzMTc0MCwtNjY1MTk3ODE2LDc5OD
MyNjA3NiwtMTI3MDE5NjI0NywxOTU5NjA5NTc5LDg1ODA1NTcz
NSwtMTY0NDIzNDc0MiwzMDY5MDg1OTcsLTg5OTE4Njc3LDE4Nz
c3MjQ0NzIsNTIxOTc2MzE5LDIwMzY1NTk3LDExMjk0MTM0Mjcs
LTIxNDQwMzgwNjQsLTE0MjA1MjEyMTZdfQ==
-->