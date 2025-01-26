# Metric spaces

Metric spaces are topological spaces. They have additional structure defined on them which is induced due to the metric. The notion of metric allows us to define distances between two points of topological spaces.

The metric $g$ on X is a map from $X \times X$ to real number $\mathbb{R}$:

$$
g: (x,y) \in X \times X \mapsto g(x,y) \in \mathbb{R}
$$

which satisfies the following axioms:

- Symmetric: $g(x,y)=g(y,x)$
- Positive definite: $g(x,y) > 0, \iff x \ne y$
- $g(x,x) = 0$
- Triangle inequality: $g(x,z) \le g(x,y) + g(y, z)$

We can use metric to define the open balls.

$$
B_{r}(x) = \{ y \vert g(x,y) < r, \forall y \in X\}
$$

A point $x_{0} \in X$ is called the accumulation point of a subset $M$ iff, for every $\varepsilon > 0$, there exists at least one point $y \ne x_{0}$ of M such that $g(x_{0}, y) < \varepsilon$.

## Open set

A subset $M$ of X is open iff, for every $m \in M$, there exists a ball $B_{r}(m)$ which is completely contained in M.

## Close set

A subset $M$ of X is close if it not open.

In otherwords if the subset M contains all its accumulation points then subset M is close.

## Continuous mapping

Let $X$ and $Y$ be topological spaces. Let $f:X \mapsto Y$ be a mapping defined on these spaces.

Then, $f$ is called continuous at a point $x_{0} \in X$ if for every neighborhood U of $f(x_{0})$ there exists a neighborhood V of $x_{0}$ such that image of V, that is, $f(V) \subseteqq U$.

The mapping f is said to be continuous if it is continuous at every point of its domain $D(f) = X$.

The mapping $f$ is continuous iff the inverse image under $f$ of every open set of Y is an open set of X.

## Compactness

A system of sets $G_{\alpha},\alpha \in A$, is called a covering of the set X if X is contained as a subset of the union $\bigcup_{\alpha \in A}G_{\alpha}$.

A subset M of a topological space X is called compact if every system of open sets of X which covers M contains a finite subsystem also covering M.

Compact subsets of a topological space are necessarily closed.

A closed subset $M_1$ of a compact set M of a topological space X is compact.
