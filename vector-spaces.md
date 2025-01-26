# Vector Spaces

Vector spaces are also known as linear space.

An element of a vector space is called a vector.

A vector space is associated with a field, which can be Real ($R$) or complex ($C$).

:::info
A vector space is close under addition `(+)` and multiplication `(*)` operation. It means that:

- In a vector space, if we add two elements, then we get another element of that vector space.
- If we multiply a vector with a scalar (an element of field), then the resultant vector remains in the vector space.
:::

:::note
Every vector-space contains a zero vector. This is because, if we subtract a vector from itself we get zero vector. We also get zero vector by multiplying a vector with zero. Further, if we add  zero vector to any vector, the resultant vector is same as the original vector.
:::

## Mathematical definition

Let $V$ be a vector space defined over the field ($R$ or $C$), then $V$ satisfies the following axioms:

- if $x, y \in V$ and $\alpha, \beta \in R$, then $\alpha x + \beta y \in V$.
- if $x \in V$ and $\alpha \in V$, then $\alpha * x \in V$.

In this way:

$$
+: (x,y) \in V \times V \rightarrow x+y \in V
$$

$$
*: (\alpha,x) \in R \times V \rightarrow \alpha* x \in V
$$

## Finite-dimensional vector space

:::info Definition: Finite Dimensional Vector Space
A vector space $V$ is finite-dimensional if every linearly independent set is a finite set. In other words, for all sets $E \subseteq V$ such that:
$$
\sum_{i=1}^{N}a_{i}v_{i}=0\implies a_{1}=a_{2}=\cdots=a_{N}=0,\forall v_{1},\cdots,v_{N}\in E
$$

$E$ has a finite cardinality.

:::

Some examples of finite-dimensional vector spaces:

- $R^{2}$
- $R^{n}$
- $C^{n}$

## Infinite-dimensional vector space

Vector space $V$ is infinite Dimensional if it is not finite Dimensional.

$C([0,1])$, the set of continuous function defined over $[0,1]$, is an infinite dimensional vector space. We can prove it by taking a subset $E$ which is defined as

$$
E := \left\{ x^{n}:n\in N\cup\{0\}\right\},
$$

which is indeed an infinite dimensional set.
