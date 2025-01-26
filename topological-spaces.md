# Topological-Spaces

Let us consider a set $X$. Now lets construct another set $\tau$, which is a collection of subsets of X. That is, every element of $\tau$ is a subset of $X$.

Now lets give following properties to $\tau$:

- $\tau$ contains a void set
- $\tau$ contains the set X
- $\tau$ is close under the union operation, that is the union of two elements of $\tau$ is in $\tau$
- $\tau$ is closed under the intersection operation, that is finite number of intersection of elements of $\tau$ is in $\tau$

If $\tau$ has the above properties then we say that $\tau$ defines a topology in $X$.

- The elements of $\tau$ are called the open sets of the topological space  $(X, \tau)$.
- We shall often omit $\tau$ and refer to $X$ as a topological space. So when we say, $X$ is a topological space, it means there exist $\tau$ "topology in X".

For every pair $(x_1, x_2)$ of distinct points $x_1, x_2, \in X$, there exist disjoint open sets $G_{1}$ $G_2$ such that $x_1 \in G_1$ and $x_2 \in G_2$.

:::note
We know that a set has no structure. What topology does (bare minimum) for us is gives the set an extra structure.
:::

## Example

A circle is a topological space which is denoted by $S^{1}$.

## Neighborhood

A neighborhood of point $x \in X$ is a set containing an open-set which contains x.

A neighborhood of the subset M of X is a set which neighborhood of every point of M.

A point x of X is an accumulation point or limit point of a subset M of X if every neighborhood of x contains at least one point $m \in M$ different from x.

## Continuity

Consider two topological spaces $(X, \tau_{X})$ and $(Y, \tau_{Y})$, and map $f:X \mapsto Y$.

$f$ is continuous if $\forall y \in \tau_{Y}$: preimage of $y$ under map f belongs to $\tau_{X}$.
