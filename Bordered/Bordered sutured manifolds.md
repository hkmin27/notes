### Sutured manifolds and surfaces

---
**Definition 1.** A *sutured manifold* is a pair $(Y,\Gamma)$ where $Y$ is an oriented 3-manifold with boundary and $\Gamma$ is a collection of closed simple curves on $\partial Y$ called *sutures*. Every component of $\partial Y$ contains sutures and $\Gamma$ divides $\partial Y$ into two regions $R_+$ and $R_-$.

---

There is a 2-dimensional analogue of a sutured manifold.

---
**Definition 2.** A *sutured surface* is a pair $\mathcal{F}=(F,\Lambda)$ where $F$ is an oriented surface with boundary and $\Lambda$ is a collection of points on $\partial F$ called *sutures*. Every component of $\partial F$ contains sutures and $\Lambda$ divides $\partial F$ into two components $S_+$ and $S_-$.

**Definition 3.** Let $\mathcal{F} = (F,\Lambda)$ be a sutured surface. A *dividing set* $\Gamma$ for $\mathcal{F}$ is a finite collection of oriented properly embedded arcs and simple closed curves in $F$ for which $\partial\Gamma = -\Lambda$. Also, $\Gamma$ separates $F$ into two regions $R_+$ and $R_-$ with $\partial{R_\pm} = (\pm\Gamma)\cup S_\pm$.

---

Insert figure of sutured surfaces

### Arc diagrams and bordered sutured manifolds

---
**Definition 4.** An *arc diagram* of rank k is a triple $\mathcal{Z} = (Z, a, M)$ where $Z$ is a finite collection of oriented arcs, $a = \{a_1, ... , a_{2k}\} \subset Z$ is a set of $2k$ disjoint points and $M: a \to \{1,...,k\}$ is a 2-1 matching. Also the 1-manifold obtained by 0-surgery along each 0-sphere $M^{-1}(i)$ in $Z$ should have no closed component.

---

Given an arc diagram $\mathcal{Z}$, we can associate a graph $G(\mathcal{Z})$ by attaching 1-cells to points in $a$ according to the matching $M$.
We can also associate a sutured surface $\mathcal{F}(\mathcal{Z}) = (F(\mathcal{Z}),\Lambda(\mathcal{Z}))$ in the following way. Starting with the product $Z \times [0,1]$ and attach (2-dim) 1-handles along $M^{-1}(i) \times \{0\}$. The suture set is given by $\Lambda(\mathcal{Z}) := -(\partial Z \times \{\frac12\})$, and the positive and negative regions are the portions of $\partial F(\mathcal{Z})$ containing $Z \times \{1\}$ and $Z \times \{0\}$ respectively. See figure...
There is an obvious embedding $G(\mathcal{Z})$ in $\mathcal{F}(\mathcal{Z})$ sending $Z$ to $Z \times \{1/2\}$ and the 1-cells to the cores of the 1-handles. So when we say $Z$ in $\mathcal{F}(\mathcal{Z})$, we always mean $Z \times \{1/2\}$.
If there is a diffeomorphism from $\mathcal{F}(\mathcal{Z})$ to a sutured surface $\mathcal{F} = (F,\Lambda)$, we say $\mathcal{Z}$ parametrizes $\mathcal{F}$.

**Definition.** A *bordered sutured manifold* $(Y,\Gamma,\mathcal{Z})$ is a sutured manifold $(Y,\Gamma)$ together with an embedding  sutured surface $\mathcal{F}(Z)$ into $\partial Y$ that sends $Z$ into $\Gamma$ (in an orientation preserving way).


<!--stackedit_data:
eyJoaXN0b3J5IjpbLTc0NTE1OTkwNCwxNDI3ODA3NjY5LC02OT
YyOTExNjcsMTE3MzQ3NjQ0LC0xMDQxMjc5ODEwLDM0MDIwOTAz
MSw1NDkxNTMyODYsLTg2MjI5NTMzNiwtNTg4NTMwNjQ2LDE4OD
UzNzc0MV19
-->