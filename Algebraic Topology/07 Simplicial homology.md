A finitely generated chain complex $(C_\bullet, d)$ is
- a collection of free finitely generated abelian groups $C_i$ for $i \in \mathbb Z$, and $C_i = 0$ for all but finitely many $i$;
- a collection of boundary homomorphisms $d_i \colon C_i \to C_{i-1}$;
- such that $d^2 = 0$.
Chain complexes can also be defined over a ring such as $\mathbb Q$, in which case $C_i$ is a $\mathbb Q$-module (a $\mathbb Q$-vector space) and the $d_i$ are module homomorphisms (linear maps).

- $\widetilde C_k(K)$ is the free abelian group on a basis given by the $e_I \in K$ with $|I| = k+1$.
- $C_k(K) = \widetilde C_k(K)$ if $k \geq 0$, but $C_{-1}(K) = 0$.
- For $k \geq 1$, $d_k \colon \widetilde C_k(K) \to \widetilde C_{k-1}(K)$ is given by $d(e_I) = \sum_{j=0}^{|I|} (-1)^j e_{I_{\hat \jmath}}$ where $I_{\hat \jmath}$ is $I$ with the $j$th-smallest entry removed.
- $x \in C_k$ is a cycle or closed if $dx = 0$.
- $x \in C_k$ is a boundary or exact if $x = dy$ for some $y \in C_{k+1}$.
- Boundaries are cycles.

Homology groups.
- $H_k(C) = \ker d_k / \mathrm{Im}\, d_{k+1}$. Think: cycles modulo boundaries.
- $C_\bullet(K) = \widetilde C_\bullet(K)/\langle e_\varnothing \rangle$.
- $\widetilde H_i(K) = H_i(\widetilde C_\bullet(K))$. $H_i(K) = H_i(C_\bullet(K))$.
- $H_\bullet(K)$ depends only on $|K|$.

Chain maps.
- A chain map $f \colon C_\bullet \to C_\bullet'$ is a collection of homomorphisms $f_i \colon C_i \to C_i'$ that commute with $d$.
- $f \colon C_\bullet \to C_\bullet'$ descends to $f_\star \colon H_\bullet(C) \to H_\bullet(C')$.
- $(f \circ g)_\star = f_\star \circ g_\star$.
- Extend $e_I$ to be defined for strings $I$ on $\{0, \dots, n\}$ instead of sets. Define $e_I = -e_{I'}$ where $I, I'$ are related by a transposition of indices; define $e_I = 0$ if $I$ has a repetition.
- Under this new definition, $d(e_I) = \sum_{j=0}^k (-1)^j e_{I_{\hat \jmath}}$, so the old definition can still be used.
- Let $f \colon K \to L$ be simplicial. Define $f_\sharp \colon C_k(K) \to C_k(L)$ by $f_\sharp(e_I) = e_{\hat f(I)}$ where if $I = (i_0, \dots, i_k)$ we define $\hat f(I) = (\hat f(i_0), \dots, \hat f(i_k))$.
- If $f$ is a simplicial map, $f_\sharp$ is a chain map (i.e. commutes with $d$).

Chain homotopies.
- Let $f_0, f_1 \colon C_\bullet \to C_\bullet'$ be chain maps. $f_0$ is chain homotopic to $f_1$ if there are homomorphisms $h_i \colon C_i \to C_{i+1}'$ satisfying $dh + hd = f_0 - f_1$. We say $h$ is the chain homotopy.
- $f_1 \sim f_0$ implies $f_{1\star} = f_{0\star} \colon H_\bullet(C) \to H_\bullet(C')$.
- A chain complex is contractible if $\mathrm{id} \sim 0$.
- If $C$ is contractible, $H_\bullet(C) = 0$.
- Define a cone on an ASC in the obvious way: $K$ together with $e_{0I}$ for $e_I \in K$.
- $\widetilde C_\bullet(C_{e_0}(K))$ (the reduced chain complex of a cone) is contractible.
- All reduced homology groups of a cone are trivial.
- The only nontrivial unreduced homology group of a cone is $H_0(C_{e_0}(K)) = \mathbb Z$.
- The homology groups for the sphere are $\mathbb Z$ for $i=0, n$ and 0 otherwise.

Exact sequences.
- Let $A_k$ be abelian groups, $f_k \colon A_k \to A_{k-1}$ be homomorphisms. Sequence is exact at $A_k$ if $\ker f_k = \mathrm{Im}\, f_{k+1}$.
- Let $f \colon A \to B$. The cokernel of $f$ is $\mathrm{coker}\,f = B/\mathrm{Im}\,f$. Think: the coimage $A/\ker f$ is canonically isomorphic to $\mathrm{Im}\,f$ by the isomorphism theorem; this is the dual notion.
- Cokernel detects surjections, kernel detects injections. Surjective iff cokernel trivial.
- Exact sequence of chain complexes gives rise to an exact sequence at each grade $k \in \mathbb Z$.
- **Snake lemma**. Let $0 \to A_\bullet \xrightarrow f B_\bullet \xrightarrow g C_\bullet \to 0$. Then there is an exact sequence $$H_k(A) \xrightarrow{f_\star} H_k(B) \xrightarrow{g_\star} H_k(C) \xrightarrow{\partial_k} H_{k-1}(A) \xrightarrow{f_\star} H_{k-1}(B) \xrightarrow{g_\star} H_{k-1}(C) \to \cdots$$
- $0 \to C_\bullet(K_1 \cap K_2) \xrightarrow i C_\bullet(K_1) \oplus C_\bullet(K_2) \xrightarrow j C_\bullet(K_1 \cup K_2) \to 0$ is exact, and $$i = \begin{pmatrix}i_{1\sharp} \\ i_{2\sharp}\end{pmatrix};\quad j = \begin{pmatrix}j_{1\sharp}&-j_{2\sharp}\end{pmatrix}$$
- **Mayer-Vietoris sequence**. Long exact sequence given by snake lemma and above.

Homology of triangulable spaces.
- Let $f_0, f_1 \colon K \to L$ be simplicial approximations to $F \colon |K| \to |L|$. Then $f_{0\sharp} \sim f_{1\sharp}$ and $f_{0\star} = f_{1\star}$.
- There is an isomorphism $\nu_K \colon H_\bullet(BK) \to H_\bullet(K)$, induced by any simplicial approximation to the identity map on $|K|$.
- For $F \colon |K| \to |L|$ continuous, we can define $F_\star \colon H_\bullet(K) \to H_\bullet(L)$ by simplicial approximation then pulling back over $\nu_K$. Does not depend on the choice of simplicial approximation.
- $(\mathrm{id}_K)_\star = \mathrm{id}_{H_\bullet(K)}$.
- $(F \circ G)_\star = F_\star \circ G_\star$.
- Homotopic continuous maps have equal induced maps on homology groups.
- Homotopy equivalent polyhedra have isomorphic homology groups.
- A space is triangulable if it is homeomorphic to the polyhedron of some ASC.
- $H_0(K) \simeq \mathbb Z^k$ where $k$ is the number of path-connected components of $|K|$.
- $\mathbb R^n \simeq \mathbb R^m$ implies $n = m$, since if we take away a single point, this shows $S^n \simeq S^{m-1}$ but they're not even homotopy equivalent as their homology groups differ.
- There is no retraction $r \colon D^n \to S^{n-1}$, by considering the $n-1$ homology group.
- **Brouwer fixed-point theorem**. A continuous function $D^n \to D^n$ has a fixed point.
- The torus has $$H_0(T^2) = \mathbb Z;\quad H_1(T^2) = \mathbb Z^2;\quad H_2(T^2) = \mathbb Z$$
- $0 \to A \to B \to \mathbb Z^r \to 0$ gives $B \simeq A \oplus \mathbb Z^r$ by the structure theorem.
- (!) Compact surfaces of genus $g$ have $$H_0 = \mathbb Z;\quad H_1 = \mathbb Z^{2g};\quad H_2 = \mathbb Z$$
- (!) The thing with $M_r$, $M_{r,1}$.

Lefschetz fixed point theorem. Let $C$ be a chain complex over $\mathbb Q$.
- The Lefschetz number of $f \colon C \to C$ is $L(f) = \sum_k (-1)^k \mathrm{tr}\, f_k$.
- The Lefschetz number of $f_\star \colon H_\bullet(C) \to H_\bullet(C)$ is $L(f_\star) = \sum_k (-1)^k \mathrm{tr}\, f_{k\star}$.
- $L(f) = L(f_\star)$.
- The Euler characteristic of a chain complex is the Lefschetz number of the identity map.
- **Lefschetz fixed-point theorem**. Let $F \colon |K| \to |K|$ be continuous. If $L(F_\star) \neq 0$, $F$ has a fixed point.