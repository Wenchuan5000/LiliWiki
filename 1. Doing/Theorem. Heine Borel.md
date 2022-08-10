# Theorem. Heine Borel

## Theorem

Let $(X, \rho)$ be a [[Definition. Metric Spaces|metric space]].

$(X, \rho)$ is [[Definition. Compact Spaces|compact]] if and only if it is both [[Definition - Complete Metric Spaces|complete]] and [[Definition. Totally Bounded Metric Spaces|totally bounded]].

## Proof

Assume $(X, \rho)$ is [[Definition. Compact Spaces|compact]].

**Compactness Implies Total Boundedness**

Let $\delta \in \mathbb R_{> 0}$ be arbitrary. Then, $\{B(x, \delta): x \in X\}$ is an [[Definition. Basis of Sets|basis]] of $X$, where $B(x, \delta)$ denotes the [[Definition. Balls|open ball]] with $x$ as the center and $\delta$ as the radius.

As $(X, \rho)$ is [[Definition. Compact Spaces|compact]], there is a finite $F \subseteq X$, such that $\{B(x, \delta): x \in F\}$ is a [[Definition. Basis of Sets|subbasis]] of $X$. In this case, $F$ is a finite [[Definition. Nets of Metric Spaces|net]] of $X$.

Thus, $X$ is [[Definition. Totally Bounded Metric Spaces|totally bounded]].

**Compactness Implies Completeness**

Let $(M, \rho')$ be a [[Definition - Complete Metric Spaces|complete]] [[Definition. Metric Spaces|metric space]], such that $(X, \rho)$ is a [[Definition. Subspaces|subspace]] of $(M, \rho')$.

By [[Theorem. Compact Subspaces of Hausdorff Spaces Are Closed]], $X$ is [[Definition. Closed Sets|closed]] in $(M, \rho')$.

By [[Theorem. Any Subspace of Any Complete Metric Space Is Complete iff It Is Closed]], $(X, \rho)$ is [[Definition - Complete Metric Spaces|complete]].

$\Box$

Assume $(X, \rho)$ is [[Definition - Complete Metric Spaces|complete]] and [[Definition. Totally Bounded Metric Spaces|totally bounded]].

Let $(M, \rho')$ be a [[Definition - Complete Metric Spaces|complete]] [[Definition. Metric Spaces|metric space]], such that $(X, \rho)$ is a [[Definition. Subspaces|subspace]] of $(M, \rho')$.

By [[Theorem. Any Subspace of Any Complete Metric Space Is Complete iff It Is Closed]], $(X, \rho)$ is [[Definition. Closed Sets|closed]].






