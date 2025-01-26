---
sidebar_position: 1
---

# 𑗕 Lp spaces

Let $\mathcal{O}$ and $\Omega$ denote respectively, an open set and a bounded open set in $\mathbb{R}^{N}$.

## Support

For any function $\phi : \mathcal{O} \mapsto \mathbb{R}$, the support of $\phi$, denoted by $\text{supp} \phi$, is defined by the following closed set of $\mathcal{O}$:

$$
\text{supp} \phi = \bar{\{ x \in \mathcal{O}, \phi \ne 0\}} \cap \mathcal{O}
$$

## Space of smooth functions

We will denote by $\mathcal{D}(\mathcal{O})$  or by $C_{0}^{\infty}(\mathcal{O})$ the set of indefinitely differentiable functions whose support is a compact set of $\mathbb{R}^{N}$.

Further, we denote by $C_{c}^{0}(\mathcal{O})$ the set of continuous functions whose support is compact set of $\mathbb{R}^{N}$ in $\mathcal{O}$.

## Definition

Let $p \in \mathbb{R}$ with $1 \le p < \infty$. Define

$$
L^{p}(\mathcal{O})=\left\{ f,f:\mathcal{O}\mapsto\mathbb{R},f\text{ measurable and s.t. }\int_{\mathcal{O}}\vert f(x)\vert dx<\infty\right\}
$$

$$
L^{\infty}\left(\mathcal{O}\right)=\left\{ f,f:\mathcal{O}\mapsto\mathbb{R},f\text{ measurable and s.t. }\exists C\in\mathbb{R},\vert f(x)\vert<C\right\}
$$

We also define:

$$
L_{loc}^{p}\left(\mathcal{O}\right)=\left\{ f,f\in L^{p}\left(\omega\right),\text{ for any open bounded set } {\omega}\text{ with }\bar{\omega}\subset\mathcal{O}\right\}
$$

## Properties

$L^{p}$ spaces, for $1 \le p \le \infty$, are Banach spaces for the norm:

$$
\left\Vert f\right\Vert _{L^{p}}=\begin{cases}
\left[\int_{\mathcal{O}}\vert f(x)\vert^{p}dx\right]^{1/p} & p<\infty\\
\inf\left\{ C,\vert f\vert\le C\text{ a.e. on }\mathcal{O}\right\}  & p=\infty
\end{cases}
$$

It is worthnoting that for $p=2$, the space $L^{2}$ is a Hilbert space for the inner product:

$$
\left(f,g\right)_{L^{2}}=\int_{\mathcal{O}}f(x)g(x)dx
$$

The space $L^{p}(\mathcal{O})$ is separable for $1\le p < \infty$, and is uniformly convex for $1<p<\infty$.

The space $L^{p}(\mathcal{O})$ is reflexive for $1 < p < \infty$.

The space $L^{\infty}(\mathcal{O})$ is neither reflexive nor separable.

$\mathcal{D}(\mathcal{O})$ is dense in $L^{p}$, for $p \in [1,+\infty)$.

The density result does not hold true for $p=\infty$.

## Holder inequality

Let $1 \le p \le \infty$, then its conjugate $q$ is given by

$$
\begin{cases}
\frac{1}{p}+\frac{1}{q}=1 & 1<p<\infty\\
q=\infty & p=1\\
q=1 & p=\infty
\end{cases}
$$

Then, for $f \in L^{p}$ and $g \in L^{q}$, Holder inequality state that

$$
\int_{\mathcal{O}}\vert f(x)g(x)\vert dx\le\Vert f\Vert_{L^{p}}\Vert g\Vert_{L^{q}}
$$

Note that for $p=2$, $q=2$, therefore, Holder inequality coincides with the Cauchy-Schwarz inequality.

Due to this inequality following result holds:

Let $1\le p \le q \le \infty$, then

$$
L^{q}(\Omega) \subset L^{p}(\Omega)
$$

with

$$
\Vert f \Vert_{L^{p}} \le c \Vert f \Vert_{L^{q}},
$$

where the constant c depends upon $\vert \Omega \vert$, p and q.

## Representation theorem

Let $1 \le p < \infty$ and $q$ be the conjugate of p. Let $f \in L^{p*}$. Then, there exists a unique $g \in L^{q}$, such that

$$
\left\langle f,\phi\right\rangle _{L^{p*},L^{p}}=\int_{\mathcal{O}}g(x)\phi(x)dx,\forall\phi\in L^{p}\left(\mathcal{O}\right)
$$

Moreover,

$$
\Vert g \Vert_{L^q} = \Vert f \Vert_{L^{p*}}
$$

In otherwords, for $1\le p < \infty$, we can identify the dual space of $L^{p}$ with $L^{q}$.

## Characteristic function

Let A be a measurable set in $\mathbb{R}^{N}$. The Characteristic function $\chi_{A}$ of A is given by:

$$
\chi_{A}=\begin{cases}
1 & \text{if }x\in A\\
0 & \text{if }x\in\mathbb{R}^{N}\backslash A
\end{cases}
$$

## Step function

A function $f: \mathbb{R}^{N} \mapsto \mathbb{R}$ is called a step function if

$$
f(x) = \sum_{k=1}^{m} \alpha_{k} \chi_{I_{k}}
$$

with $m \in \mathbb{N},\alpha_{k} \in \mathbb{R}$ and where $I_{k}$ is an interval in $\mathbb{R}^{N}$, for any $k \in \{ 1, \cdots, m\}$.

If $\Omega \subset \mathbb{R}^{N}$ is a bounded open set, we denote by $S(\Omega)$ the set of step functions of the above-mentioned form, such that $I_{k} \subset \Omega$, for any $k \in \{1, \cdots, m\}$. It can be shown that $S(\Omega) \subset L^{p}(\Omega)$  for any p such that $1 \le p \le \infty$. Moreover, for $1 \le p < \infty$, $S(\Omega)$ is dense in $L^{p}(\Omega)$.
