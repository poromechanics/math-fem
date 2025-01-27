# Convergence

## Strong convergence

## Weak convergence

A sequence $\{x_{n}\}$ in E is said to be weakly converging iff:

$$
\forall x^{*} \in E^{*}, \lim_{n \rightarrow \infty}\langle x^*, x_{n} \rangle_{E^*, E} < \infty
$$

A sequence $\{x_{n}\}$ in E is said to converge weakly to x iff

$$
\forall x^{*} \in E^{*}, \langle x^*, x_{n} \rangle_{E^*, E} \rightarrow \langle x^{*}, x \rangle_{E^*, E}
$$

This weak convergence is denote by

$$
x_{n} \rightharpoonup x \text{ weakly in E}
$$

The uniqueness of $x$ can be proven by Hahn-Banach theorem.

:::{.callout-note appearance="simple"}
Strong convergence implies weak convergence.
:::

:::{.callout-tip appearance="simple"}
If E is finite dimensional Banach space, the strong convergence and the weak convergences are equivalent.
:::

If $\{x_{n}\}$ be a sequence weakly convergent to x in E. Then

1. $\{x_{n}\}$ is bounded sequence in E, that is, there exists a constant C independent of n such that
$$
\forall n \in \mathbb{N}, \Vert x_{n} \Vert_{E} \le C
$$

2. The norm of x is lower semi-continuous with respect to the weak convergence, that is,

$$
\Vert x \Vert_{E} \le \liminf_{n\rightarrow\infty} \Vert x_{n} \Vert_{E}
$$

## Uniformly convex space

We say that the Banach space E is uniformly convex if any $\varepsilon>0$, there exists $\delta > 0$ such that

$$
\left(x,y\in E,\Vert x\Vert_{E}\le1,\Vert y\Vert_{E}\le1,\Vert x-y\Vert_{E}>\varepsilon\right)\implies\left(\Vert\frac{x+y}{2}\Vert_{E}<1-\delta\right)
$$

:::{.callout-note appearance="simple"}
Any uniformly convex Banach space is reflexive, the converse being not true. Any Hilbert space is uniformly convex and thus reflexive.
:::

## Weak* convergence

In order to study the weak convergence of a sequence in Banach space E, we should be aware of its dual space $E^*$. However, it may happen that the dual space is*too big* a space. In that case proving the weak convergence can be difficult. Moreover, in such cases, there are too few weakly convergent sequences.

Definition: Let E be a Banach space and $E^*$ be the dual space. A sequence $\{ x_{n} \}$ in E is said to converge weakly* to x iff

$$
\left\langle x_{n}^{*},x\right\rangle _{E^{*},E}\rightarrow\left\langle x^{*},x\right\rangle _{E^{*},E}\forall x\in E
$$

:::{.callout-tip appearance="simple"}
Let $F$ be a Banach space and $E=F^*$. Then any weak convergent sequence in E is also weakly* convergent.
:::
