Field automorphisms.
- A bijective hom $K \to K$ is called an automorphism. $\mathrm{Aut}(K)$ is the automorphism group under composition.
- $\mathrm{Aut}(L/K)$ is the group of $K$-automorphisms of $L$.
- $\mathrm{Hom}_K(L,L) = \mathrm{Aut}(L/K)$ so $|\mathrm{Aut}(L/K)| \leq [L:K]$ by counting embeddings theorem.
- $S \subseteq \mathrm{Aut}(K)$ induces the field $K^S$, the fixed field of $S$.
- $\mathbb C^{\{z \mapsto \overline z\}} = \mathbb R$.
- $\mathbb Q$ and $\mathbb F_p$ have no nontrivial automorphisms.

An extension L/K is Galois if it is algebraic and $L^{\mathrm{Aut}(L/K)} = K$. In this case we write $\mathrm{Gal}(L/K) = \mathrm{Aut}(L/K)$.

> [!theorem]
> Let L/K finite. TFAE:
> - L/K is Galois;
> - L/K is normal and separable;
> - L is the splitting field of a separable polynomial in K;
> - $|\mathrm{Aut}(L/K)| = [L:K]$.

For finite Galois extensions,
- $m_{x,K} = \prod_{i=1}^r (T - x_i)$ for all $x \in L$, where $x_i$ are given by the orbit of $G = \mathrm{Gal}(L/K)$ on $x$.
- $L = K(x)$ for some $x \in L$ which is separable over $K$ and has degree $[L:K]$, because $L/K$ is separable.

Let L/K be a finite Galois extension. Let $K \subseteq F \subseteq L$, $H \leq G$. The Galois correspondence states:
- L/F is Galois and $\mathrm{Gal}(L/F) \leq \mathrm{Gal}(L/K)$.
- $F \mapsto \mathrm{Gal}(L/F)$ is a bijection between intermediate fields F and subgroups of $\mathrm{Gal}(L/K)$.
- The inverse bijection is $H \mapsto L^H$.
- The bijection reverses inclusions.
- $[L^H : K] = (G : H)$.
- $\sigma H \sigma^{-1}$ corresponds to $\sigma L^H$, so $L^{\sigma H \sigma^{-1}} = \sigma L^H$.
TFAE:
- $L^H / K$ is Galois;
- $L^H / K$ is separable;
- $\sigma(L^H) = L^H$ for all $\sigma \in G$;
- $H \trianglelefteq G$.
If so, $\mathrm{Gal}(L^H / K) = \mathrm{Gal}(L/K)/H$.

Galois groups of polynomials.
- If $f \in K[T]$ and $L$ is a splitting field, $\mathrm{Gal}(L/K)$ acts on the roots of $f$ in $L$. This induces $\mathrm{Gal}(f/K) \leq S_n$.
- $f$ irreducible iff $\mathrm{Gal}(f/K)$ is transitive, so for all $i.j \in \{1, \dots, n\}$ there is a permutation $\sigma \in \mathrm{Gal}(f/K)$ mapping $i$ to $j$. In other words, there is exactly one orbit of $\{1, \dots, n\}$.
- Orbit-stabiliser gives $n \mid |G|$ if $G$ transitive.
- (!) Suppose not in characteristic 2. Let $f \in K[T]$ be monic with splitting field $L$. Then $L^{G \cap A_n} = K(\Delta)$ where $\Delta^2$ is the discriminant.
- (!) Thus $\mathrm{Gal}(f/K) \subseteq A_n$ iff $\mathrm{Disc}(f)$ is a square in $K$.