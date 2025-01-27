# Inner product spaces

## Definition

Let $H$ be a real linear space. A mapping 

$$
(\cdot, \cdot) : (x,y) \in H \times H \longmapsto (x,y)_{H} \in \mathbb{R} 
$$

is called a (real) inner product iff, $\forall x,y,z \in H$ and $\alpha, \beta \in \mathbb{R}$:

- $(x,x)_{H} > 0 x \ne 0$
- $(x,x)_{H} = 0$  $\iff x=0$
- $(x,y)_{H}=(y,x)_{H}$
- $(\alpha x + \beta y, z)_{H}=\alpha (x,z)_{H}+\beta (y,z)_{H}$

 Note that an inner product induces a norm by

$$
\Vert x \Vert = (x,x)_{H}^{1/2}
$$

Therefore, all inner-product spaces are norm spaces.

:::{.callout-note title="Hilbert Space"}
If $H$ is a Banach space with respect to the norm induced by the inner product, then $H$ is called a Hilbert space. In other words, Every Hilbert space is a Banach Space. But not all Banach spaces are Hilbert spaces. This is because not all norm comes from the inner product.
:::
