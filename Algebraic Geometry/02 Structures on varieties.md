Coordinate rings.
- $\mathbb C[V] = \mathcal O(V) = \mathbb C[\mathbf X]/I(V)$ is the coordinate ring: functions modulo being the same on $V$.
- $\sqrt I$ is the ideal of elements with some power in $I$.
- $\sqrt{\sqrt I} = \sqrt I$.
- $\mathbb V(\sqrt I) = \mathbb V(I)$.

> [!theorem]
> **Strong form of Hilbert's Nullstellensatz**. $I(\mathbb V(I)) = \sqrt I$.

Morphisms.
- A morphism $V \to W$ is a function given coordinatewise by elements of the coordinate ring.
- Equivalently, the restriction of a map given on coordinates by polynomials, with image lying in $W$.
- Morphisms can be composed.
- $\varphi \colon V \to W$ gives a pullback $\varphi^\star \colon \mathbb C[W] \to \mathbb C[V]$.
- S $\mathbb C$-algebra homomorphism is a ring homomorphism $\mathbb C[X] \to \mathbb C[Y]$ that restricts to $\mathrm{id}$ on $\mathbb C$.
- Pulling back morphisms produces a bijection $\mathrm{Mor}(V,W)$ to the space of $\mathbb C$-algebra homomorphisms $\mathbb C[W] \to \mathbb C[V]$: injective and surjective.
- Affine varieties are isomorphic if there are inverse morphisms between them.
- Affine varieties are isomorphic iff their coordinate rings are isomorphic as $\mathbb C$-algebras.

Rational functions.
- Assuming $V$ is irreducible, $I(V)$ prime, so $\mathbb C[V]$ is an integral domain.
- $\mathbb C(V) = FF(\mathbb C[V])$ is a field as $\mathbb C[V]$ is an integral domain.
- For a rational function $\varphi$, $P \in V$ is regular if $\varphi$ can be written as a ratio with nonzero denominator at $P$.
- A local ring is a ring that has a unique maximal ideal.
- A ring is a local ring iff $R \setminus R^\times$ is an ideal, in which case, the unique maximal ideal is $R \setminus R^\times$.
- The local ring of $V$ at $P$ is $\mathcal O_{V,P} = \{f \in \mathbb C(V) \mid f \text{ regular at } P\}$.
- The local ring is a local ring, with maximal ideal $\mathfrak m_{V,P} = \ker (f \mapsto f(P))$.