# Sobolev Spaces

How to define the smoothness of a mathematical function? There are many criteria for smoothness.

- Continuity $C^0$
- Differentiable $C^0$, which also implies continuity
- Continuity of the derivatives $C^p,p\ge1$

In the twentieth century, it was observed that the space $C^1, C^2, \cdots$ was not exactly the right space to study solutions of differential equations. The Sobolev spaces are the modern replacement for these spaces in which to look for solutions of partial differential equations.

In the one-dimensional case the Sobolev space $W^{k,p}(\mathbb {R} )$  for $1\leq p\leq \infty$ is defined as the subset of functions $f$ in $L^{p}(\mathbb {R} )$  such that $f$ and its weak derivatives up to order $k$ have a finite $L_p$ norm.

When $p=2$, we get the Sobolev space which are also Hilbert space, that is

$$
H^p(\Omega) = W^{2,p}(\Omega)
$$

## Weak derivatives

Let us understand the concept of multi-index. A multi-index $\alpha$ is an array of non-negative integers which serves as short-hand for derivatives as in

$$
\frac{\partial^3 u}{\partial x^2 \partial y} = \partial_{\alpha} u \quad \alpha=(2,1), \quad \vert \alpha \vert=3
$$

$$
\frac{\partial^4 u}{\partial x^2 \partial y^2} = \partial_{\alpha} u \quad \alpha=(2,2), \quad \vert \alpha \vert=4
$$

Let $\alpha$ a multi-index and $u \in L_{2}(\Omega)$. The function $u_{\alpha} := \partial_{\alpha} u \in L_{2}(\Omega)$ is called the weak derivative of $u$ if:

$$
\int_{\Omega} u \partial_{\alpha} \phi = (-1)^{\vert \alpha \vert} \int_{\Omega} \partial_{\alpha}u \phi \quad \forall \phi \in C_{0}^{\infty}(\Omega)
$$
