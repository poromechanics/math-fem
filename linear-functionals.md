# Linear functional

A linear function $l(u)$ on $\mathcal{V}$ is a real valued linear function such that

$$
l(\alpha u + \beta v) = \alpha l(u) + \beta l(v), \alpha,\beta \in R, \forall u,v \in \mathcal{V}
$$

If $l(u)$ is continuous then, there exits a $c$ such that:

$$
l(u) \le c \Vert u \Vert \forall u \in \mathcal{V}
$$

The set of all continuous linear functional defined on $V$ forms itself a norm space which is called the dual space of $V$ and it is denoted by $V^{*}$. The norm on the dual space is given by

$$
\Vert l \Vert _{V*} := sup \left (\frac{l(u)}{\Vert u \Vert} \right ) = sup \left ( l \left (\frac{u}{\Vert u\Vert} \right ) \right )
$$
