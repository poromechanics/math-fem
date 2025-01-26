# 𑗕 Lax-Milgram-Theorem

Let V be a real Hilbert space. Let $a:V\times V \rightarrow R$ be a bilinear form that is

- Continuous: $\vert a(u,v) \vert \le C_{1} \Vert u \Vert_{V} \Vert v \Vert _{V}$
- Coercive: $a(u,u) \ge C_{2} \Vert u \Vert^2_{V}$

Let $l:V\rightarrow R$ be a continuous linear functional. Then, there exists a unique $u \in V$ such that

$$
\forall v \in V, a(u,v)=l(v)
$$

Moreover, the solution $u$ is bounded by data

$$
\Vert u \Vert_{V} \le \frac{1}{C_2} \Vert l \Vert_{V^*}
$$

**Coercive** property tells us that

if $a(u,u)=0$, then $\Vert u \Vert ^{2} \le 0$, therefore, $u=0$. Hence, we can define a norm using $a(u,u)$ as follows

$$
\Vert u \Vert_{E}^2 = a(u,u)
$$

This is sometimes called the strain energy norm.

The norm on dual space $V^*$ is defined by

$$
\Vert l \Vert_{V^*} = \sup_{v\in V}\frac{\vert l(v)\vert}{\Vert v\Vert_{V}}
$$

Because $a(u,v)=l(v)$, we have

$$
\frac{\vert l(v) \vert}{\Vert v\Vert}=\frac{\vert a(u,v) \vert }{\Vert v\Vert}\le\frac{\Vert u\Vert\Vert v\Vert}{\Vert v\Vert}=\Vert u\Vert
$$

Therefore,

$$
\Vert l \Vert_{V^*} = \sup_{v\in V}\frac{\vert l(v)\vert}{\Vert v\Vert_{V}} \le \Vert u \Vert
$$

It means $\Vert u \Vert$ is an upper bound.
