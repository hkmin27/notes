**Problem 1.1.** Show that any measure  is continuous from below, in the sense that for any collection of measurable sets $(A_i)_{i=1}^\infty$ such that $A_i \subset A_{i+1}$
We first claim that if $A \subset B$, then $\mu(A \setminus B) = \mu(A) - \mu(B)$.  It is clear from the equality 
$$\mu(A) = \mu((A \setminus B) \cup B) = \mu(A \setminus B) + \mu(B).$$
Now we have
$$\begin{aligned}
\mu(\bigcup_{i=1} A_i)&=\sum_{i=1} \mu(A_{i+1} \setminus A_i)\\
&=\sum_{i=1} (\mu(A_{i+1}) - \mu(A_i))\\
&=\lim_{i\to\infty}\mu(A_i). \quad \square
\end{aligned}$$

**Problem 1.2.**
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTE5MjQ0MjUwMTIsLTE4ODg0NDM0MzVdfQ
==
-->