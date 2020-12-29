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
Check every facts

$v$ is expanding: $\mathcal{L}_v\omega = \omega$
$i_vd\omega + di_v\omega = \sum d(-q_idp_i-2p_idq_i)+\sum d(x_idy_i-y_idx_i)=\omega$
$v$ is gradient for $f$

---

**Conformal symplectic normal bundles**
Let $S$ be an isotropic submanifold of a contact manifold $(M,\alpha)$.  Then we define a *conformal symplectic normal bundle* as follows.
$$CSN(S) = TS^{\perp d\alpha}/TS$$

**framing in 3-dimension**
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTEyMjgzMDgzMDksMzA2OTA4NTk3LC04OT
kxODY3NywxODc3NzI0NDcyLDUyMTk3NjMxOSwyMDM2NTU5Nywx
MTI5NDEzNDI3LC0yMTQ0MDM4MDY0LC0xNDIwNTIxMjE2XX0=
-->