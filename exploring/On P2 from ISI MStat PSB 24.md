**Problem:** Use the identity $n^2 + (2n + 1) = (n + 1)^2$ to prove that the set $S = \{ (x, y) \in \mathbb{Q}^2 : x^2 + y^2 = 1 \}$ has infinitely many elements.

**Proof:** Comparing the given identity, $n^2 + (2n + 1) = (n + 1)^2$, with $x^2 + y^2 = 1$, we see that,
$$x^2 = \frac{n^2}{(n + 1)^2}, \quad y^2 = \frac{2n + 1}{(n + 1)^2}.$$
For any $n \in \mathbb{N}, x = n/(n + 1) \in \mathbb{Q}$. But it is not true for $y = \sqrt{2n +1}/(n +1)$, for $y$ to be rational, we have to guarantee that $\sqrt{2n + 1} \in \mathbb{N}$. For that, assume that $2n + 1 = k^2$ for some $k \in \mathbb{N}$ then $n = (k^2 - 1) / 2$, substituting this gives,
$$x = \frac{k^2 - 1}{k^2 + 1} \in \mathbb{Q} \quad \text{and} \quad y = \frac{\sqrt{2n + 1}}{n+1} = \frac{2k}{k^2 +1} \in \mathbb{Q},$$
for any $k \in \mathbb{N}$. Moreover,
$$x^2 + y^2 = \left( \frac{k^2 - 1}{k^2 + 1} \right)^2 + \left( \frac{2k}{k^2 + 1} \right)^2 = 1.$$
Now define a function $f: \mathbb{N} \to \mathbb{Q}^2$ such that $f(k) = ((k^2 - 1)/(k^2 + 1), 2k/(k^2 + 1))$.
Further, suppose for $k_1, k_2 \in \mathbb{N}$ with $f(k_1) = f(k_2)$ then,
$$\left(\frac{k_1^2 - 1}{k_1^2 + 1}, \frac{2k_1}{k_1^2 + 1} \right) = \left(\frac{k_2^2 - 1}{k_2^2 + 1}, \frac{2k_2}{k_2^2 + 1} \right)$$
implies, $k_1^2 - 1 = k_2^2 - 1$ and $2k_1 = 2k_2$ both are true only when $k_1 = k_2$. Means, $f$ is one-one function. Therefore, $S$ has infinitely many elements.