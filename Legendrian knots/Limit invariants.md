### Limit invariant
Consider a knot $K$ in a closed 3-manifold $Y$. Let $Y(K)$ be the knot complement $\overline{Y \setminus N(K)}$, and $\Gamma_i$ a pair of sutures on $\partial Y(K)$ of slope $-i$. Notice that there are two minimally twisting tight contact structures $\xi_+$ and $\xi_-$ on $B_i := \overline{(Y(K),\Gamma_{i+1}) \setminus (Y(K),\Gamma_i))}$.

Thus we have a gluing map induced by $\xi_-$.
$$\phi_-: SFH(-Y(K), -\Gamma_i) \to SFH(-Y(K), -\Gamma_{i+1}).$$

Taking the direct limit of the above sequence of groups, we obtain *the sutured limit homology of $K$*.
$$\underrightarrow{SFH}(-Y,K) := \underrightarrow{\lim}SFH(-Y(K),-\Gamma_i).$$

We also have another gluing map induced by $\xi_+$.
$$\psi_+:SFH(-Y(K), -\Gamma_i) \to SFH(-Y(K), -\Gamma_{i+1}).$$

We will **show** that the maps induce a well-defined map
$$\Psi: \underrightarrow{SFH}(-Y,K) \to \underrightarrow{SFH}(-Y,K).$$

The group $\underrightarrow{SFH}(-Y,K)$ can be given the structure of $\mathbb{F}[U]$-module, where $U$ acts by $\Psi$. **(why?)**

**Theorem.** Let $K \subset Y$ be a null-homologous knot. Then there exists an isomorphism of bigraded $\mathbb{F}[U]$-modules
$$I_-: \underrightarrow{SFH}(-Y,K) \to HFK^-(-Y,K).$$
**(why do we need null-homologous cond?)**

### Legendrian invariant

$$EH(K_i) \in SFH(-Y(K),-\Gamma_i)$$

$$\phi_-(EH(K_i)) = EH(K_{i+1})$$

$$\underrightarrow{EH}(K) \in \underrightarrow{SFH}(-Y,K)$$

**Theorem.** Let $K \subset (Y, \xi)$ be a null-homologous Legendrian knot. Then the isomorphism 
$$I_-: \underrightarrow{SFH}(-Y,K) \to HFK^-(-Y,K)$$

identifies $\underrightarrow{EH}(K)$ and $\mathcal{L}(K)$

### Inverse limit invariant
Now, let $\Gamma_i$ be a pair of sutures on $\partial Y(K)$ of slope $i$. In this case, we can define an inverse limit invariant
$$\underleftarrow{SFH}(-Y,K)$$

**Theorem.** Let $K \subset Y$ be a null-homologous knot. Then there exists an isomorphism of bigraded $\mathbb{F}[U]$-modules
$$I_+: \underleftarrow{SFH}(-Y,K) \to HFK^+(-Y,K).$$

We can also define the Legendrian invariant of $\underleftarrow{EH}(K) \in \underleftarrow{SFH}(-Y,K)$.
<!--stackedit_data:
eyJoaXN0b3J5IjpbNTY5MDA2NzkzLC0yMDgyMTE4MTgxLDQ2NT
Q2MjMzNywxODI5MTAzNDAsLTEzMDc4NzExNTMsLTE1MTQ4Njcy
ODcsOTQ0NjA5OTM3LC0zMjkxNjU1NTZdfQ==
-->