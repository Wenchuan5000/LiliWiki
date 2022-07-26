# [[Complete Metric Spaces]]

## Definitions

A [[Metric Spaces|metric space]] $(X, \rho)$ is said to be **complete** if and only if every Cauchy sequence in $X$ converges in $X$.

#### Cauchy Sequence

A sequence $u$ in $(X, \rho)$, i.e., $u: I \subseteq \mathbb N \to (X, \rho)$, is said to be **Cauchy** if and only if for any $\varepsilon \in \mathbb R_{> 0}$, there is an $i \in I$, such that for nay $m,n \in I_{> i}$,

$$
\rho(u_m, u_n) < \varepsilon.
$$

### Examples

#### The Set of Rational Numbers Is Not Complete

Let $\rho$ be an [[Metric Spaces#Euclidean Metrics|Euclidean metric]] on $\mathbb Q$. Then $(\mathbb Q, \rho)$ is not complete. This can be proved by a counter example. Let $u: \mathbb N \to \mathbb Q$ be defined as

$$
u(n) = \sum_{i = 1}^n \frac{1}{i! \cdot 2^i}.
$$

