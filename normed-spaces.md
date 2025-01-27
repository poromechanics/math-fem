# Normed spaces

In metric spaces we have metric to measure the distance between two elements of a metric space. By using the metric we can study how close or far two elements are from each other.

We want to develop such concepts in vector space. Then, we can check closeness between two elements of a vector space.

## Norm

Definition: Norm

A mapping

$$
\Vert \cdot  \Vert : x \in V \longmapsto \Vert x \Vert \in R^{+}
$$

is called a norm on the vector space $V$ iff

(Definiteness)

$$
\Vert x \Vert = 0 \text{ iff } x=0
$$

(Homogeneity)

$$
\Vert \alpha x \Vert = \vert \alpha \vert \Vert x \Vert, \quad  \forall x \in V, \text{ and } \alpha \in R
$$

(Triangle inequality)

$$
\Vert x + y \Vert \le \Vert x \Vert + \Vert y \Vert, \forall x, y \in V.
$$

Example: The Euclidean norm on $R^{n}$ or $C^{n}$, given by

$$
\Vert x \Vert_{2} := \left( \sum_{i=1}^{n} \vert x_{i} \vert ^{2} \right)^{1/2}
$$

is indeed a norm.

Following is also a norm:

$$
\Vert x \Vert_{\infty} := \max_{1\le i \le n} \vert x_{i} \vert
$$

In general, for $1 \le p < \infty$, following is also a norm:

$$
\Vert x \Vert_{p} := \left( \sum_{i=1}^{n} \vert x_{i} \vert ^{p} \right)^{1/p}
$$

## Seminorm

A seminorm is a mapping

$$
\vert \cdot  \vert : x \in V \longmapsto \Vert x \Vert \in R^{+}
$$

which satisfies the Homogeneity and Triangle inequality but not necessarily Definiteness property.

## Definition

Normed space: A vector space $V$ which is equipped with the norm $\Vert \cdot \Vert_{V}$ is called the normed space.


## Metric and Norm

Recall that if $X$ is metric space, then the metric $d$ is a mapping:

$$
d: (x,y) \in X \times X \longmapsto R^{+},
$$

which has following three conditions:

- (Identification) $d(x,y) =0$ iff $x=y$
- (Symmetry) $d(x,y) = d(y,x)$ for all $x,y \in X$
- (Triangle inequality) $d(x,y)+d(y,z) \ge d(x,z)$ for all $x,y,z \in X$

It is clear that norm induces a metric:

:::{.callout-note}
Metric induce by Norm: Let $\Vert \cdot \Vert$ be a norm on a vector space V. Then,

$$
d(x,y) = \Vert y - x \Vert, \forall x,y \in V
$$

defines a metric on $V$.
:::

## Example of Normed space

Let $X$ be a metric space. The vector space $C_{\infty}(X)$ is defined as:

$$
C_{\infty}(X):= \left \{  f: X \rightarrow C: f \text{ is Continuous and bounded}  \right \}
$$

For any metric space $X$, we can define a norm on the vector space $C_{\infty}$ via

$$
\Vert v \Vert_{\infty} := \sup_{x \in X} \vert v(x) \vert
$$

Proof:

- Definiteness: if $v=0$, then $\Vert v \Vert_{\infty}=0$.
- Homogeneity:

$$
\begin{aligned}\Vert\alpha v\Vert_{\infty} & =\sup_{x\in X}\vert\alpha v(x)\vert\\
 & =\sup_{x\in X}\vert\alpha\vert\vert v(x)\vert\\
 & =\vert\alpha\vert\sup_{x\in X}\vert v(x)\vert\\
 & =\vert\alpha\vert\Vert v\Vert_{\infty}
\end{aligned}
$$

- Triangle inequality:

$$
\begin{aligned}\Vert v+w\Vert_{\infty} & =\sup_{x\in X}\vert v(x)+w(x)\vert\\
 & \le\sup_{x\in X}\left(\vert v(x)\vert+\vert w(x)\vert\right)\\
 & =\sup_{x\in X}\vert v(x)\vert+\sup_{x\in X}\vert w(x)\vert\\
 & =\Vert v(x)\Vert_{\infty}+\Vert w(x)\Vert_{\infty}
\end{aligned}
$$

### Convergence of sequence

Now that we have a norm on $C_{\infty}(X)$, we can talk about the convergence of sequences.

Consider a sequence $\{u_{n}\}_{n=1}^{\infty}$ in $C_{\infty}(X)$. We say that the sequence converges to $u$, that is, $u_{n} \rightarrow u$, in $C_{\infty}(X)$ if

$$
\Vert u_{n} - u \Vert_{\infty} = 0,
$$

in other words,

$$
\forall\varepsilon>0,\exists N\in\mathbb{N}:\forall n\ge N,\forall x\in X,\vert u_{n}(x)-u(x)\vert<\varepsilon,
$$

which is the definition of **uniform convergence** on X.

## Example 2

Let us consider another example of Normed spaces. Consider a space of infinite sequences,$\{ a_{i} \}_{i=1}^{\infty}$, which will be designated by $l^{p}$ space:

$$
l^{p} := \left \{ \{ a_{i} \}_{i=1}^{\infty}: \Vert a \Vert_{p} < \infty \right \},
$$

where,

$$
\Vert a\Vert_{p}=\begin{cases}
\left(\sum_{i=1}^{\infty}\vert a_{i}\vert^{p}\right)^{1/p} & 1\le p<\infty\\
\sup_{1\le i\le\infty}\vert a_{i}\vert & p=\infty
\end{cases}
$$
