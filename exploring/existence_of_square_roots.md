# The Existence of Square Roots

**Theorem** For every $p \in \mathbb{R}^{+}$, there exists a unique $\alpha \in \mathbb{R}^{+}$ such that $\alpha^2 = p$.

**Proof:** Define $$T = \{ t \in \mathbb{R} : t^2 < p \}.$$

$T$ is non-empty (since $0 \in T$) and bounded above. Let $\alpha = \sup{T}$. We show $\alpha^2 = p$ by ruling out the possibilities $\alpha^2 < p$ and $\alpha^2 > p$.

For $\alpha^2 < p$, we will show that there exists an element in $T$ which is larger than $\alpha$ and for $\alpha^2 > p$, we will show that there exists an upper bound for $T$ smaller than $\alpha$.

**Case 1:** Suppose $\alpha^2 < p$.

Let $\delta = \frac{p - \alpha^2}{2 \alpha + 1} > 0$. By the Archimedean Property there exists an $n \in \mathbb{N}$ such that $\frac{1}{n} < \delta$. Then

$$\begin{align*}
\left( \alpha + \frac{1}{n} \right)^2 &= \alpha^2 + \frac{2 \alpha}{n} + \frac{1}{n^2} \\
&< \alpha^2 + \frac{2 \alpha + 1}{n} \\
&< \alpha^2 + (2 \alpha + 1) \delta = p.
\end{align*}$$
Thus $\alpha + \frac{1}{n} \in T$, contradicting that $\alpha$ is an upper bound for $T$.

**Case 2:** Suppose $\alpha^2 > p$.

Let $\epsilon = \frac{\alpha^2 - p}{2 \alpha} > 0$. Choose $n \in \mathbb{N}$ such that $\frac{1}{n} < \epsilon$. Then

$$\begin{align*}
\left( \alpha - \frac{1}{n} \right)^2 &= \alpha^2 - \frac{2 \alpha}{n} + \frac{1}{n^2} \\
&> \alpha^2 - \frac{2 \alpha}{n} \\
&> \alpha^2 - 2 \alpha \epsilon = p.
\end{align*}$$

Hence, for any $t \in T$, we have $t^2 < p < (\alpha - \frac{1}{n})^2 \implies t < \alpha - \frac{1}{n}$. So $\alpha - \frac{1}{n}$ is an upper bound for $T$ smaller than $\alpha$, contradicting that $\alpha$ is the least upper bound.

Therefore, $\alpha^2 = p$. Uniqueness follows from the positivity of $\alpha$ and the fact that $\alpha^2 = \beta^2 = p$ implies $(\alpha - \beta)(\alpha + \beta) = 0$ and $\alpha + \beta > 0$.