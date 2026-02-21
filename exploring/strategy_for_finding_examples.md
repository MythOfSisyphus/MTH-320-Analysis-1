# General Strategy for Finding Examples

When you need to construct a sequence (or double sequence) with specific properties, it helps to start with simple building blocks:

- Basic convergent sequences: $1/n, 1/n^2$, etc.
- Oscillatory sequences: $(-1)^n, \sin{n}, \cos{n}$.
- Combinations: products, sums, or piecewise definitions.

For double sequences, you often want to control behavior along rows and columns separately. Think about:

- If you want the double limit to exist, you need the values to become small when both indices are large. So a factor like $1 / \min(m, n)$ or $1 / (m + n)$ works.
- To make the row limits (for fixed $m$) fail, you need the dependence on $n$ to not decay to zero. That means the factor involving $n$ should be something that oscillates without decaying, like $(-1)^n$ or $\sin{n}$. But then to keep the double limit, small, you multiply by something that decays with $m$ (like $1 / m$) so that when both are large, the product is small. However, that would make the column limits (for fixed $n$) decay for $m$, so they would exist. To make both row and column limits fail, you need the factor to depend on both variables in such a way that for fixed $m$, the $n$-dependence does not decay, and for fixed $n$, the $m$-dependence does not decay. That suggests using a denominator that is symmetric but does not decay when one variable is fixed, like $\min(m, n)$ or $\max(m, n)$ ? Actually, $\min(m, n)$ works because for fixed $m$, when $n$ is large, $\min(m, n) = m$ constant, so the factor $1/m$ is constant; for fixed $n$, when $m$ is large, $\min(m, n ) = n$ constant. So $1 / \min(m, n)$ gives constant amplitude in the other variable. Then multiply by an oscillatory factor like $(-1)^{m + n}$ or $\sin{m} \sin{n}$ to get the non-convergence.

**Another approach**: use a piecewise definition. For example, let $a_{mn} = 1$ if $m$ and $n$ are both even, and $0$ otherwise? That wouldn't give a double limit. But you can adjust.

The key is to experiment with simple forms and check the properties. If one attempt fails, tweak it.

---
## Example Double-Sequence

$$a_{mn} = \frac{\sin{m} \sin{n}}{\min(m, n)}.$$

