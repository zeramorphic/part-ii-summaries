Simplices.
- $\Delta^n$ is the set of points in $\mathbb R^{n+1}$ with positive coordinates with sum 1, taken with the subspace topology.
- Simplices are compact and Hausdorff.
- $e_0, \dots, e_n$ are the vertices of $\Delta^n$.
- For $I \subseteq \{0, \dots, n\}$, the $I$th face, denoted $e_I$, is the set of points with $x_i = 0$ for $i \not\in I$.
- $e_{\{i\}} = e_i$.
- $e_I$ is closed in $\Delta^n$ and is homeomorphic to $\Delta^{|I| - 1}$.
- $e_I \subseteq e_J$ iff $I \subseteq J$.
- $e_I \cap e_J = e_{I \cap J}$.
- $|f| \colon \Delta^n \to \mathbb R^N$ is affine linear if it is the restriction of a linear map.
- Affine linear maps are uniquely defined by their action on the $e_i$.
- $|f| \colon \Delta^n \to \Delta^m$ is simplicial if it is affine linear and maps vertices to vertices.
- Simplicial $|f|$ induce $\hat f \colon \{0, \dots, n\} \to \{0, \dots, m\}$ given by $|f|(e_i) = e_{\hat f(i)}$.
- Simplicial $|f|$ are uniquely defined by $\hat f$.
- $|f|(e_I) = e_{\hat f(I)}$.
- $v_0, \dots, v_n \in \mathbb R^N$ are affine linearly independent if $\sum t_i v_i = 0, \sum t_i = 0$ implies $t_i = 0$ for all $i$.
- TFAE:
	- $v_0, \dots, v_n$ are affine linearly independent
	- $\sum t_i v_i = \sum t_i' v_i$ and $\sum t_i = \sum t_i'$ implies $t_i = t_i'$ for all $i$
	- $v_1 - v_0, \dots, v_n - v_0$ are linearly independent
	- the affine linear map $|f| \colon \Delta^n \to \mathbb R^N$ given by $|f|(e_i) = v_i$ is injective
- If $v_0, \dots, v_n$ are ALI, we write $[v_0, \dots, v_n] = \mathrm{Im}\, |f|$. This is called a Euclidean simplex. 
- $\Delta^n$ compact and $[v_0, \dots, v_n]$ Hausdorff, so $|f| \colon \Delta^n \to [v_0, \dots, v_n]$ is a homeomorphism if the $v_i$ are ALI by topological IFT.
- For $X \subseteq \mathbb R^N$ let $Z(X)$ be the set of extreme points, so whenever $x = \sum t_i x_i$ for $\sum t_i = 1$ and $x_i \in X$, we have $x_i = x$ for some $i$.
- $Z([v_0, \dots, v_n]) = \{v_0, \dots, v_n\}$.
- If $[v_0, \dots, v_n] = [v_0', \dots, v_n']$ as subsets of $\mathbb R^N$, then $\{v_0, \dots, v_n\} = \{v_0', \dots, v_n'\}$. So a Euclidean simpliex determines its vertices.
- The set of Euclidean simplices $\mathcal S(\mathbb R^N)$ is in bijection with the set of sets of $k \leq N+1$ ALI vertices.

Abstract simplicial complexes.
- An abstract simplicial complex in $\Delta^n$ is a downward closed set of faces of $\Delta^n$. No topology.
- if $K$ is an ASC, $|K| = \bigcup K$ is its polyhedron.
- Polyhedra of ASCs are compact and Hausdorff.
- The $r$-skeleton of $K$, denoted $K_r$, are those faces of dimension at most $r$.
- $K$ an ASC implies $K_r$ an ASC.
- The vertex set is $V(K) = |K_0|$.
- $\boldsymbol\Delta^n = F(\Delta^n)$ has polyhedron $\Delta^n \simeq D^n$.
- $\mathbb S^{n-1} = \boldsymbol\Delta_{n-1}^n$ has polyhedron $\partial \Delta^n \simeq S^{n-1}$.
- If K, L are ASCs, a simplicial map $f \colon K \to L$ is a map such that there exists a simplicial $|f| \colon \Delta^n \to \Delta^m$ with $f(e_I) = |f|(e_I)$. (Note that simplicial maps between ASCs map simplices (elements of $K$) to simplices (elements of $L$), not points to points)
- Equivalently, $f \colon K \to L$ is a simplicial map if there exists $\hat f \colon \{0, \dots, n\} \to \{0, \dots, m\}$ such that $f(e_I) = e_{\hat f(I)}$ and $e_I \in K$ implies $e_{\hat f(I)} \in L$.
- The identity map is simplicial. The composition of simplicial maps is simplicial.
- A simplicial map is a simplicial isomorphism if it is a bijection.
- TFAE:
	- $f \colon K \to L$ is a simplicial isomorphism
	- $|f| \colon |K| \to |L|$ is a bijection
	- $|f| \colon |K| \to |L|$ is a homeomorphism

Euclidean simplicial complexes.
- $K \subseteq \mathcal S(\mathbb R^n)$ is a Euclidean simplicial complex if $K$ is a finite set of Euclidean simplices, closed under taking faces, and the intersection of two simplices is a face of each simplex.
- Note that the intersection of two simplices in an ESC is required to be a simplex, not a simplicial complex.
- Let $|\varphi| \colon \Delta^n \to \mathbb R^n$ be affine linear and $K'$ an ASC in $\Delta^n$. Then if $|\varphi|$ is injective on $|K'|$, $\varphi(K') = \{|\varphi|(e_I) \mid e_I \in K'\}$ is an ESC.
- An ESC is a realisation of an ASC if it is of the form $\varphi(K')$ for $|\varphi|$ affine linear and injective on $|K'|$ as above.
- For a realisation $\varphi(K')$, $|\varphi| \colon |K'| \to |\varphi(K')|$ is a homeomorphism.
- Any ESC is a realisation of some ASC, unique up to simplicial isomorphism.
- A simplicial map of ESCs is a map $K_1 \to K_2$ given by lifting a simplicial map of ASCs across realisations.

Boundaries and cones.
- If $\sigma$ is an $n$-dimensional Euclidean simplex, let $F(\sigma)$ be the faces of $\sigma$, an ESC with $|F(\sigma)| = \sigma$.
- Define the boundary ESC $\not\partial\sigma = F(\sigma)_{n-1} = F(\sigma) \setminus \{\sigma\}$.
- The topological boundary is $\partial \sigma = |\not\partial\sigma| \simeq S^{n-1}$.
- $\sigma^\circ = \sigma \setminus \partial\sigma$.
- $p \in \mathbb R^N$ is independent of $X \subseteq \mathbb R^N$ if for all $x \in X$, the ray $px$ has $px \cap X = \{x\}$.
- If $p$ independent of $X$, the cone is given by $C_p(X) = \{tp + (1-t)x \mid t \in [0,1], x \in X\}$.
- $p$ is independent of $[v_0, \dots, v_n]$ iff $\{v_0, \dots, v_n, p\}$ is affine linearly independent, in which case the cone is $[v_0, \dots, v_n, p]$.
- If $p$ is independent of the polyhedron of an ESC $K$, define $C_p(K) = K \cup \{[v_0, \dots, v_j, p] \mid [v_0, \dots, v_j] \in K\}$.
- If $p$ independent of $|K|$ then $C_p(K)$ is an ESC and $|C_p(K)| = C_p(|K|)$.

Barycentric subdivision.
- The barycentre of a simplex $\sigma = [v_0, \dots, v_n]$ is $b_\sigma = \frac{1}{n+1}\sum_{i=0}^n v_i \in \mathbb R^N$.
- $b_\sigma$ is independent of $\partial\sigma$.
- $C_{b_\sigma}(\partial \sigma) = \sigma$.
- Define barycentric subdivision on simplices and ESCs by induction on dimension, such that $|\beta(\sigma)| = \sigma$ and $|B(K)| = |K|$. Prove IH 1 (n) implies IH 2 (n) implies IH 1 (n+1).
	- IH 1: For $n$-dimensional simplices $\sigma$, $\beta(\sigma)$ is an ESC of dimension $n$ with $|\beta(\sigma)| = \sigma$, and if $\tau$ is a face of $\sigma$ and $\sigma_1 \in \beta(\sigma)$, then $\sigma_1 \cap \tau \in \beta(\tau)$.
	- IH 2:For $n$-dimensional ESCs $K$, $B(K)$ is an $n$-dimensional ESC with $|B(K)| = |K|$.
- Let $\sigma \in \mathcal S(\mathbb R^N)$ and $x, v \in \sigma$. Then $\|v - x\| \leq \max_{v_i \in V(\sigma)} \|v_i - x\|$.
- The mesh $\mu(\sigma)$ of a simplex $\sigma$ is the maximum distance between two points, or equivalently the maximum distance between two vertices by the above.
- The mesh $\mu(K)$ of an ESC $K$ is the maximum mesh of its faces.
- $\max_{v \in \sigma} \|b_\sigma - v\| \leq \max_{v_i \in V(\sigma)} \|b_\sigma - v_i\| \leq \frac{n}{n+1} \mu(\sigma)$.
- $\mu(\beta(\sigma)) \leq \frac{n}{n+1}\mu(\sigma)$.
- $\mu(B(K)) \leq \frac{n}{n+1}\mu(K)$.

Simplicial approximation.
- If $x \in \Delta^n$, there is a unique face $e_I$ with $x \in e_I^\circ$.
- $x \in e_I^\circ$ implies $x \in e_J$ iff $I \subseteq J$.
- If $K$ is an ASC in $\Delta^n$ and $x \in e_I^\circ$ with $x \in |K|$, then $e_I \in K$.
- If $K$ is an ESC and $x \in |K|$, there is a unique $\sigma \in K$ with $x \in \sigma^\circ$ (lift to ASC).
- Let $v \in V(K)$, then the star is $\mathrm{St}_K(v) = \bigcup_{v \in \sigma \in K} \sigma^\circ$.
- If $x \in \sigma^\circ$, $x \in \mathrm{St}_K(v)$ iff $v \in V(\sigma)$.
- $\mathrm{St}_K(v) = |K| \setminus \bigcup_{\{\sigma \in K \mid v \not\in V(\sigma)\}}\sigma^\circ = |K| \setminus \bigcup_{\{\sigma \in K \mid v \not\in V(\sigma)\}}\sigma$.
- The set of stars forms an open (by above) cover of $|K|$.
- $\hat g \colon V(K) \to V(L)$ is a simplicial approximation of a continuous $f \colon |K| \to |L|$ if $f(\mathrm{St}_K(v)) \subseteq  \mathrm{St}_L(\hat g(v))$. Think: stars are mapped inside corresponding stars.
- (!) Let $\hat g \colon V(K) \to V(L)$, $\varphi\colon K' \to K$ be a realisation, $g' \colon |K'| \to \mathbb R^M$ the affine linear map defined on $v \in V(K')$ by $|g'|(v) = \hat g(\varphi(v))$. Then $|g| = |g'| \circ |\varphi|^{-1}$ defines a simplicial $g \colon K \to L$, and $|g| \sim f$.
- **Simplicial approximation theorem**. For a continuous $f \colon |K| \to |L|$ between ESCs, there is $r > 0$ and $g \colon B^r(K) \to L$ simplicial such that $|g| \sim f$.
- Simplicial functions map an $i$-skeleton to an $i$-skeleton.
- Let $\dim K < \dim L$ and $f \colon |K| \to |L|$ is continuous, $f$ is homotopic to a map that is not surjective.
- If $k < n$, any continuous map $S^k \to S^n$ is null-homotopic.