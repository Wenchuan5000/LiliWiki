# Definition. Open Sets

## Definitions of Open Sets in Topological Spaces Topological Spaces

Let $(X, \mathcal T)$ be a [[Definition. Topological Space|topological space]].

Let $S \subseteq X$.

### Definition via Topologies

$S$ is **open** if and only if $S \in \mathcal T$.

### Definition via Closed Sets

$S$ is **open** if and only if $X \setminus S$ is [[Definition. Closed Sets|closed]].

### Definition via Neighbourhoods

$S$ is **open** if and only if for any point $s \in S$, there is a [[Definition. Neighbourhoods|neighbourhood]] $N$ of $s$, such that $N \subseteq S$.

### Definition via Interiors

$S$ is **open** if and only if the [[Definition. Interiors|interior]] of $S$ is exactly $S$ itself.

## Proof of Equivalence of Definitions of Open Sets in Topological Spaces

### [[#Definition via Topologies]] if and Only if [[#Definition via Closed Sets]]

Assume $S$ is open. $X \setminus S$ is [[Definition. Closed Sets|closed]].

$\Box$

Assume $X \setminus S$ is [[Definition. Closed Sets|closed]],

$$
S = X \setminus (X \setminus S)
$$

is open.

$\blacksquare$

### [[#Definition via Topologies]] if and Only if [[#Definition via Neighbourhoods]]

Assume $S$ is open. Then, for any $s \in S$, $S$ itself is an [[Definition. Neighbourhoods|open neighbourhood]] of $s$.

$\Box$

Assume that for any point $s \in S$, there is a [[Definition. Neighbourhoods|neighbourhood]] $N$ of $s$, such that $N \subseteq S$.

Thus, for any $s \in S$, there is an [[Definition. Neighbourhoods|open neighbourhood]] $U_s$ of $s$, such that $U \subseteq S$.

Thus, we have

$$
\bigcup_{s \in S} U_s = S.
$$

By [[Definition. Topological Space|Open Set Axiom 2]], as every $U_s$ is open, $S$ is open.

$\blacksquare$

### [[#Definition via Neighbourhoods]] if and Only if [[#Definition via Interiors]]

Assume that for any point $s \in S$, there is a [[Definition. Neighbourhoods|neighbourhood]] $N$ of $s$, such that $N \subseteq S$.

By the [[Definition. Interiors|definition of interiors]], every $s \in S$ is [[Definition. Interiors|interior]] to $S$. Thus, $S$ is the interior of $S$ itself.

$\blacksquare$

## Definitions of Open Sets in Topological Spaces Metric Spaces

Let $(X, \rho)$ be a [[Definition. Metric Spaces|metric space]].

Let $\mathcal T$ be the [[Definition. Topological Space|topology]] [[Definition. Induced Topology|induced]] by $\rho$.

Let $S \subseteq X$.

### Definition via Induced Topologies

$S$ is **open** if and only if $S \in \mathcal T$.


### Definition via Open Balls

$S$ is **open** if and only if for any $s \in S$, there exists a $\delta_s \in \mathbb R_{> 0}$, such that the [[Definition. Balls|open ball]] $B(s, \delta) \subseteq S$.

## Proof of Equivalence of Definitions of Open Sets in Metric Spaces

### [[#Definition via Induced Topologies]] if and Only if [[#Definition via Open Balls]]

Assume $S \in \mathcal T$.

By the [[Definition. Topological Space|alternative definition of topologies]],

$$
\mathcal T = \left\{ \bigcup \mathcal A : \mathcal A \subseteq \mathcal B \right\},
$$

where $\mathcal B$ be the set of all [[Definition. Balls|open balls]] in $(X, \rho)$.

As $S \in \mathcal T$, there is an $\mathcal A \subseteq \mathcal B$ such that $S = \bigcup \mathcal A$. Thus, for any $s \in S$, there is an $A \in \mathcal A$, such that $s \in A$. That is, there exists an $\delta_s \in \mathbb R_{> 0}$, such that

$$
s \in A = B(s, \delta_s).
$$

$\Box$

Assume for any $s \in S$, there exists a $\delta_s \in \mathbb R_{> 0}$, such that the [[Definition. Balls|open ball]] $B(s, \delta) \subseteq S$.

As [[Theorem. Open Balls Are Open|open balls are open in the induced topology]], every $B(s, \delta_s)$ is open in $(X, \mathcal T)$.

As

$$
\bigcup_{s \in S} B(s, \delta_s) = S,
$$

By [[Definition. Topological Space|Open Set Axiom 2]], $S$ is open.

$\blacksquare$
