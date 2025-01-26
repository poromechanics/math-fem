---
sidebar_position: 2
---

# 𑗕 Banach spaces

:::info Definition: Banach space
A normed space is a Banach space if it is complete with respect to the metric induced by the norm.
:::

We know that space of rational numbers is not complete. This is because we can find a sequence of rational number which converges to the irrational number.  In this case, we know that the space of real numbers $R$ fills the holes.

We want to have similar property for Banach spaces.

- $R^{n}$ and $C^{n}$ are complete with respect to any of the $\Vert \cdot \Vert_{p}$ norms.

:::note Theorem
For any metric space $X$, the space of bounded, continuous functions of $X$ is complete, and thus $C_{\infty}(X)$ is a Banach space.
:::

## Linear forms on Banach spaces

Let $E$ and $F$ be Banach spaces with norm $\Vert \cdot \Vert_{E}$ and $\Vert \cdot \Vert_{F}$.

:::info Bounded linear form
Let $\Lambda : E \longmapsto F$ be a linear map. Then, $\Lambda$ is bounded iff

$$
\sup_{x \in E \backslash {0}} \frac{\Vert \Lambda(x) \Vert_{F}}{\Vert x \Vert_{E}} < \infty
$$

:::

Let us denote by $\mathcal{L}(E,F)$ the set of linear and bounded maps from E to F.

## Properties of bounded linear maps

The space  $\mathcal{L}(E,F)$ is a Norm space with following norm:

$$
\Vert \Lambda \Vert_{\mathcal{L}(E,F)} = \sup_{x \in E \backslash {0}} \frac{\Vert \Lambda(x) \Vert_{F}}{\Vert x \Vert_{E}}
$$

Because $\mathcal{L}(E,F)$ is linear space, we have:

$$
\Vert \Lambda \Vert_{\mathcal{L}(E,F)} = \sup_{x \in E, \Vert x \Vert_{E}=1} \Vert \Lambda(x) \Vert_{F}
$$

:::info
The space $\mathcal{L}(E,F)$ is also a Banach space with respect to the above-mentioned norm.
:::

Also we have,

$$
\Vert \Lambda(x) \Vert_{F} \le \Vert \Lambda \Vert_{\mathcal{L}(E,F)} \Vert x \Vert_{E}, \forall x \in E
$$

:::info Theorem
Let $\Lambda$ a linear map from E to F. Then, the following three assertions are equivalent:

1. $\Lambda$ is bounded
2. $\Lambda$ is continuous
3. $\Lambda$ is continuous at a point $v_{0} \in E$.
:::

## Linear functional

In the above-mentioned linear maps let's consider the case when $F$ is $\mathbb{R}$. In that case the linear-map maps element of $E$ to a real-value. This linear map has special name and it is called the **linear-functional** (or, simply the functional). Therefore, a linear functional $l$ is mapping:

$$
l: x \in E \longmapsto l(x) \in \mathbb{R}
$$

with

$$
l(\alpha u + \beta v) = \alpha l(u) + \beta l(v), \alpha,\beta \in \mathbb{R}, \forall u,v \in E
$$

The linear functional is bounded iff:

$$
\sup_{x \in E \backslash {0}} \frac{\vert l(x) \vert}{\Vert x \Vert_{E}} < \infty
$$

The space of bounded linear functional on $E$ will be denoted by

$$
\mathcal{L}(E, \mathbb{R})
$$

which is also known as the dual space of $E$ and denoted by $E^{*}$.

:::note
If $l(x)$ is bounded $\iff$ $l(x)$ is continuous.
:::

## Dual space

:::note Dual space
Let $E$ be the Banach space. The set of the linear and continuous (or, bounded) functional from $E$ into $\mathbb{R}$ is called the dual space of E and is denoted by $E^{*}$. If $x^{*} \in E^{*}$, the image $x^{*}(x)$ of $x \in E$ is denoted by $<x^{*}, x>_{E^{*}, E}$. The bracket $<\cdot, \cdot>_{E^{*}, E}$ is called the duality pairing between $E^{*}$ and $E$.
:::

Dual space of $E$ is a Banach space with following norm:

$$
\Vert x^{*} \Vert_{E^{*}} =  \sup_{x \in E \backslash {0}} \frac{\vert <x^{*}, x>_{E^{*}, E} \vert}{\Vert x \Vert_{E}}
$$

or

$$
\Vert x^{*} \Vert_{E^{*}} =  \sup_{x \in E, \Vert x \Vert_{E}=1} \vert \langle x^{*}, x \rangle_{E^{*}, E} \vert
$$

Also, we have

$$
\vert <x^{*}, x>_{E^{*}, E} \vert \le \Vert x^{*} \Vert_{E^{*}} {\Vert x \Vert_{E}}
$$

:::info
We have seen that the dual space of a Banach space is a Banach Space. Therefore, we can easily show that the dual space of the dual space of the dual space of the Banach space is also a Banach space. That is, if $E$ is a Banach space, then $E^{*}$ and $E^{**}$ are both Banach spaces.
:::

Let $x\in E$ be fixed and introduce the map

$$
f_{x} : x^{*} \in E^{*} \longmapsto \langle x^{*},x \rangle_{E^{*}, E} \in \mathbb{R}.
$$

Then $f_{x} \in E^{**}$ and the map

$$
\mathcal{F} : x \in E \longmapsto f_{x} \in E^{**}
$$

is an isometry, that is,

$$
\Vert x \Vert_{E} = \Vert \mathcal{F}(x) \Vert_{E^{**}} = \Vert f_{x} \Vert_{E^{**}}
$$

:::note
In this way, one can identify $x$ with $f_{x}$, and then $E$ with its image under the mapping $\mathcal{F}(E) \subset E^{**}$. Moreover, the space $E$ is called reflexive iff $\mathcal{F}(E) = E^{**}$.
:::
