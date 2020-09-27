**Problem 1.1.** We first need the following lemma.

**Lemma.** If $A_{i+1} \subseteq A_i$, then 
$$\mathbb{P}(\bigcap_{i=1}^\infty A_i) = \lim_{i\to\infty}\mathbb{P}(A_i)$$
**Proof.** From **Problem 1.1.** in measure theoretic foundation, we have
$$\begin{aligned} \mathbb{P}(\bigcup_{i=1}^\infty A^c_i) &= \lim_{i\to\infty}\mathbb{P}(A^c_i)\\
1-\mathbb{P}(\bigcap_{i=1}^\infty A_i) &= 1-\lim_{i\to\infty}\mathbb{P}(A_i) \quad \square \end{aligned}$$

If $a_1 \leq a'_i$, we have $\{X_i \leq a_i \} \subseteq \{X_i \leq a'_i\}$. Thus the first item follows from the definition of measure. (It's not left continuous since $\bigcup A_i = (-\infty, a)$)
If $a^m \downarrow a$, then we have $A_{m+1}:=\{X_i \leq a^{m+1}_i \} \subseteq \{X_i \leq a^m_i\}$ and $\lim_{i\to\infty} A_i = \{X_i \leq a_i\}$. Now the second item follows from **Lemma**.
If $a_i \to \infty$ for all $i$, then we can find a monotone increasing subsequence for all i. Relabel it as $a_i$. Now apply **Problem 1.1** in measure theoretic foundation and we obtain the third item. $-\infty$ is similar.

 **Problem 4.1.** By definition, we only need to show
 $$\mathbb{E}f(X) = \int_{\mathbb{R}^n} f(t)\,d\mu_X(t)$$

**Problem 4.3.** Since |Y-w| is a non-negative random variable, we have 

$$\begin{aligned} \mathbb{E}(|Y-w|) &= \int_0^\infty \mathbb{P}\{Y - w \geq t\}\,dt + \int_0^\infty \mathbb{P}\{w - Y \geq t\}\,dt\\
&= \int_w^\infty \mathbb{P}\{Y \geq t\}\,dt + \int_{-\infty}^w \mathbb{P}\{Y \leq t\}\,dt. \end{aligned}$$

Thus we have

$$g'(t) = \mathbb{P}(Y \leq t) - \mathbb{P}(Y \geq t)$$

If $g(w)$ is the minimum then $g'(w)=0$ and $w$ is median. If $w$ is median of $Y$, we obtain $g'(w) = 0$ from the above formula. Also notice that $g'(t)$ is monotone increasing function. Thus $\{t \;|\; g'(t)=0\}$ is an interval and the $g(w)$ is the minimum of $g$. $\square$  

(why do we need $\mathbb{E}(X)<\infty$ ?)
  
**Problem 4.4.** We first show that $\mathbb{E}(X-a)^2$ is minimized when $a = \mathbb{E}X$

$$\mathbb{E}(X-a)^2 = \mathbb{E}X^2 -2a\mathbb{E}X + a^2 = (\mathbb{E}X-a)^2 + \mathbb{E}X^2 - (\mathbb{E}X)^2.$$

Thus $\text{Var}X = \mathbb{E}(X-EX)^2 \leq \mathbb{E}(X-t)^2$. Next,

$$\begin{aligned} &\mathbb{E}(X-t)^2 \leq 2\text{Var}X\\ 
\Leftrightarrow \,&\mathbb{E}(X-t)^2 \leq 2\text{Var}(X-t)\\
\Leftrightarrow \,&\mathbb{E}(X-t)^2 \leq 2(\mathbb{E}X(X-t)^2 - (\mathbb{E}X(X-t))^2)\\
\Leftrightarrow \,&(\mathbb{E}(X-t))^2 \leq (\mathbb{E}(X-t)^2 - (\mathbb{E}(X-t))^2) = \text{Var}X.\\
\end{aligned}$$

However, by Jensen's inequality (or the definition of variation),

$$|E(X-t)| \leq E|X-t| 
\leq E|X-EX| \leq \sqrt{E(X-EX)^2} =\sqrt{\text{Var}X}. \quad\square$$

 **Problem 5.3.** Suppose $X$ is subexponential.
 $$\begin{aligned}
 \mathbb{E}|X|^p &= \int_0^\infty \mathbb{P}\{|X|\geq t^{1/p}\}\,dt\\
 &= \int_C^\infty \exp(-ct^{1/p})\,dt + D\\
 &\leq \int_0^\infty pc^{-p}u^{p-1} \exp (-u)\,du, \quad (u=ct^{1/p})\\ 
 &=pc^{-p}\Gamma(p)
 \end{aligned}$$

 Since $\Gamma(p)^{1/p} \leq p$, the inequality follows. Conversely, if the inequality holds, then
 
 $$\mathbb{E}(e^{\lambda |X|})=1+\sum_{k=1}^\infty \frac{\lambda^k\mathbb{E}(|X|^k)}{k!}<\infty$$
 
 for $|\lambda| < C$. Now we need a lemma.
 
**Lemma. (Chernoff bound)** $\mathbb{P}\{X \geq t\} \leq e^{-\lambda t}\,\mathbb{E}(e^{\lambda X})$.

**Proof.** $\mathbb{E}(e^{\lambda X}) = \int e^{\lambda X}d\mathbb{P} \geq \int e^{\lambda X} \cdot 1_{X \geq t}d\mathbb{P} \geq \int e^{\lambda t} \cdot 1_{X \geq t}d\mathbb{P} \geq e^{\lambda t}\,\mathbb{P}\{X \geq t\}$. $\square$

By lemma, $\mathbb{P}\{|X| \geq t\} \leq de^{-\lambda t} \leq e^{-ct}$ for $t \geq C$. $\square$
<!--stackedit_data:
eyJoaXN0b3J5IjpbMTc3ODA1OTU1NCwxOTgyNzI4OTk2LDE5ND
Q5NzQ4MjgsLTEzNzAwNjk2NTgsMTQ3NDc4MzI2MF19
-->