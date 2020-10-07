**Problem 1.1.** We first need the following lemma.

**Lemma.** If $A_{i+1} \subseteq A_i$, then 
$$\mathbb{P}(\bigcap_{i=1}^\infty A_i) = \lim_{i\to\infty}\mathbb{P}(A_i)$$
**Proof.** From **Problem 1.1.** in measure theoretic foundation, we have
$$\begin{aligned} \mathbb{P}(\bigcup_{i=1}^\infty A^c_i) &= \lim_{i\to\infty}\mathbb{P}(A^c_i)\\
1-\mathbb{P}(\bigcap_{i=1}^\infty A_i) &= 1-\lim_{i\to\infty}\mathbb{P}(A_i) \quad \square \end{aligned}$$

If $a_1 \leq a'_i$, we have $\{X_i \leq a_i \} \subseteq \{X_i \leq a'_i\}$. Thus the first item follows from the definition of measure. (It's not left continuous since $\bigcup A_i = (-\infty, a)$)
If $a^m \downarrow a$, then we have $A_{m+1}:=\{X_i \leq a^{m+1}_i \} \subseteq \{X_i \leq a^m_i\}$ and $\lim_{i\to\infty} A_i = \{X_i \leq a_i\}$. Now the second item follows from **Lemma**.
If $a_i \to \infty$ for all $i$, then we can find a monotone increasing subsequence for all i. Relabel it as $a_i$. Now apply **Problem 1.1** in measure theoretic foundation and we obtain the third item. $-\infty$ is similar.

**Problem 4.1.** It's almost same as the case of $\mathbb{R}$.

**Problem 4.2.** By u-sub $(x \to y := x + \mu)\, (y \to u := u/\sqrt{2}\sigma)$, we have

$$\begin{aligned}\int_{-\infty}^\infty x\rho_X(x)\,dx &= \int_{-\infty}^\infty \frac{x}{\sqrt{2\pi}\sigma}\exp\left(-\frac12\frac{(x-\mu)^2}{\sigma^2}\right) \,dx\\
&= \int_0^\infty \frac{2\mu}{\sqrt{\pi}}\exp(-u^2)\,du\\
&= \sqrt{\int_0^\infty \frac{2\mu}{\sqrt{\pi}}\exp(-u^2)\,du \cdot \int_0^\infty \frac{2\mu}{\sqrt{\pi}}\exp(-v^2)\,dv}\\
&= \frac{2\mu}{\sqrt{\pi}} \sqrt{\int_0^{\pi/2}\int_0^\infty \exp(-r^2)r \,dr \,d\theta}\\
&=\mu. \end{aligned}$$

Similarly,

$$\begin{aligned}\int_{-\infty}^\infty x^2\rho_X(x)\,dx &= \sigma^2+\mu^2. \end{aligned}$$



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

$$\begin{aligned} &\mathbb{E}(X-t)^2 \leq 2\text{Var}X = 2\text{Var}(X-t)\\ 
\Leftrightarrow \,&\mathbb{E}(X-t)^2 \leq 2(\mathbb{E}(X-t)^2 - (\mathbb{E}(X-t))^2)\\
\Leftrightarrow \,&(\mathbb{E}(X-t))^2 \leq \mathbb{E}(X-t)^2 - (\mathbb{E}(X-t))^2 = \text{Var}X.\\
\Leftrightarrow \,&|\mathbb{E}(X-t)| \leq \sqrt{\text{Var}X}.
\end{aligned}$$

However, by Jensen's inequality (or the definition of variation),

$$|E(X-t)| \leq E|X-t| 
\leq E|X-EX| \leq \sqrt{E(X-EX)^2} =\sqrt{\text{Var}X}. \quad\square$$

Or we can just use
$$\mathbb{E}(X-t)^2 \leq \mathbb{E}(X-\mathbb{E}X + \mathbb{E}X -t)^2 = \text{Var}X + (\mathbb{E}X - t)^2 \leq 2\text{Var}X$$

**Problem 4.5.** Suppose the probability space is $P = ([0,1],\mathcal{R})$ and 

$$\begin{aligned} X &= \begin{cases}1/t \quad &1/(2n-1) \leq t \leq 1/2n,\\ 0 \quad &1/2n < t < 1/(2n+1).\end{cases}\\
Y &= \begin{cases}1/t \quad &1/(2n) < t < 1/(2n+1),\\ 0 \quad &1/(2n-1) \leq t \leq 1/2n.\end{cases}
\end{aligned}$$

Thus $XY = 0$ so $\mathbb{E}XY = 0$. However, $\mathbb{E}X = \int_0^1X(t)\,dt = \infty$. Similarly, $\mathbb{E}Y = \infty$.

$Z := \min{(X,Y)}$. Then $Z^2 \leq XY$. By Jensen's inequality, we have

$$(\mathbb{E}Z)^2 \leq \mathbb{E}Z^2 \leq \mathbb{E}XY < \infty.$$
Thus $\mathbb{E}Z < \infty \quad \square$. 

**Problem 5.1.** Suppose $X$ is subexponential.
$$\begin{aligned}
\mathbb{E}|X|^p &= \int_0^\infty \mathbb{P}\{|X|\geq t^{1/p}\}\,dt\\
&\leq \int_C^\infty \exp(-ct^{1/p})\,dt + D\\
&\leq \int_0^\infty pc^{-p}u^{p-1} \exp (-u)\,du, \quad (u=ct^{1/p})\\ 
&=pc^{-p}\Gamma(p)
\end{aligned}$$

Since $\Gamma(p)^{1/p} \leq p$, the inequality follows. Conversely, if the inequality holds, then

$$\mathbb{E}(e^{\lambda |X|})=1+\sum_{k=1}^\infty \frac{\lambda^k\mathbb{E}(|X|^k)}{k!}<\infty$$

for $|\lambda| < C$. Now we need a lemma.
 
**Lemma. (Chernoff bound)** $\mathbb{P}\{X \geq t\} \leq e^{-\lambda t}\,\mathbb{E}(e^{\lambda X})$.

**Proof.** $\mathbb{E}(e^{\lambda X}) = \int e^{\lambda X}d\mathbb{P} \geq \int e^{\lambda X} \cdot 1_{X \geq t}d\mathbb{P} \geq \int e^{\lambda t} \cdot 1_{X \geq t}d\mathbb{P} \geq e^{\lambda t}\,\mathbb{P}\{X \geq t\}.\quad\square$

By lemma, $\mathbb{P}\{|X| \geq t\} \leq de^{-\lambda t} \leq e^{-ct}$ for $t \geq C. \quad\square$
<!--stackedit_data:
eyJoaXN0b3J5IjpbMzkwODMyMzk5LDE3NzgwNTk1NTQsMTk4Mj
cyODk5NiwxOTQ0OTc0ODI4LC0xMzcwMDY5NjU4LDE0NzQ3ODMy
NjBdfQ==
-->