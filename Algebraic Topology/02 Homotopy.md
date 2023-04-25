For $f_0, f_1 \colon X \to Y$, write $f_0 \sim f_1$ ($f_0$ is homotopic to $f_1$) if there exists continuous $H \colon X \times I \to Y$ with $H(x,0) = f_0(x)$ and $H(x,1) = f_1(x)$.
- **Gluing lemma**. Let $X = C_1 \cup C_2$, $C_i$ closed. Then $f$ is continuous iff $f|_{C_1}, f|_{C_2}$ continuous.
- Homotopy is an equivalence relation.
- $f_0 \sim f_1, g_0 \sim g_1$ implies $g_0 \circ f_0 \sim g_1 \circ f_1$.

A space is contractible if $\mathrm{id} \sim c_p$, so the identity is homotopic to a constant map.
- All maps into contractible spaces are homotopic (as they are homotopic to a constant map).
- Contractible implies path-connected.

Spaces are homotopy equivalent if $f \colon X \to Y, g \colon Y \to X$ have compositions homotopic to the identity maps.
- Homotopy equivalence is an equivalence relation.
- A space is contractible iff it is homotopy equivalent to the one-point space.