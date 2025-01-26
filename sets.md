# Sets

Sets are primitive object in mathematics. It denotes the collection of elements, and it has no structure on it. We denote by X the set which is collection of elements $a, b, c, \cdots$ by

$$
X = \{ a, b, c, \cdots\}
$$

If an element $a$ is in X, we denote it by $a \in X$. If $b$ is not in X, then we denote it by $b \notin X$.

## Cartesian product

Let $X$ and $Y$ be two sets. Then Cartesian product of X and Y is a set of ordered pairs of elements from X and Y:

$$
X \times Y = {(x_i, y_i), x_i \in X, y_i \in Y, \text{ for }, i=1,2,\cdots}
$$

## Maps

$f$ is a map from X to Y, which is denoted by $f: X \longmapsto Y$ such that

$$
x_{i} \in X: \exists y_{i} \in Y: y_{i} = f(x_{i})
$$

So we say:

$$
f: x_{i} \in X \longmapsto f(x_{i}) \in Y
$$

- $f(x_{i})$ is called the image of $x_{i}$ in Y with respect to the mapping $f$.
- $X$ is called the domain of $f$.
- $Y$ is called the co-domain of $f$.
- The set $\{y_{i}: y_{i}=f(x_{i}), \forall x_{i} \in X\}$ is called the range of $f$.

## Injective maps

A map $f:X \mapsto Y$ is called injective if each element of $X$ maps to a unique element of $Y$. Injective maps are called one-to-one map. In other words, range of X under the map $f$ is contained in Y.

## Surjective maps

A map $f$ is called surjective if every element of $X$ maps to at least one element in $Y$. In other words, there should be no $y_{i} \in Y$, such that, $y_{i} \ne f(x_{i})$. In other words, range of X under the map $f$ is same as Y.

## Bijective maps

A map $f$ is Bijective if it is both surjective and injective. In this case, we say $X$ and $Y$ are isomorphic under $f$, and $f$ is called isomorphism.
