Let $A \subseteq X$. Say $f_0, f_1 \colon X \to Y$ are homotopic relative to $A$ if they have a homotopy fixing $A$ at all points $t \in I$. Write $f_0 \sim_e f_1$ if $f_0 \sim f_1$ rel endpoints.
- Homotopy relative to a set is an equivalence relation.
- If $f_0 \sim f_1$ rel $A$ and $g_0 \sim g_1$ rel $f(A)$ (for either $f_0$ or $f_1$) then $g_0 \circ f_0 \sim g_1 \circ f_1$ rel $A$.
- If $f_0, f_1 \colon I \to I$ have the same endpoints, they are homotopic rel endpoints by convexity.
- If $f \colon I \to I$ and $\gamma \colon I \to X$ with $f(0) = 0, f(1) = 1$, we have $\gamma \circ f \sim_e \gamma$.
- If $f \colon I \to I$ and $\gamma \colon I \to X$ with $f(0) = 0, f(1) = 0$, we have $\gamma \circ f \sim_e c_{\gamma(0)}$.

Let $\Omega(X,p,q)$ be the set of continuous paths from $p$ to $q$ in $X$. Let $\Omega(X,p) = \Omega(X,p,p)$.
- If $\gamma \in \Omega(X,p,q)$ and $\gamma' \in \Omega(X,q,r)$, can define $\gamma\gamma' \in \Omega(X,p,r)$ by gluing.
- Let $\gamma_0, \gamma_1 \in \Omega(X,p,q)$ and $\gamma_0', \gamma_1' \in \Omega(q,r)$ such that $\gamma_0 \sim_e \gamma_1$ and $\gamma_0' \sim_e \gamma_1'$. Then $\gamma_0\gamma_0' \sim_e \gamma_1\gamma_1'$.
- Let $\gamma \in \Omega(X,p,q)$. Define the reverse $\gamma^{-1} \in \Omega(X,q,p)$.
- $c_p \gamma \sim_e \gamma \sim_e \gamma c_q$.
- $\gamma \gamma^{-1} \sim_e c_p$ and $\gamma^{-1}\gamma \sim_e c_q$.
- $\gamma(\gamma'\gamma'') \sim_e (\gamma\gamma')\gamma''$, assuming $\gamma(1) = \gamma'(0)$ and $\gamma'(1) = \gamma''(0)$.

The fundamental group of $X$ based at $x_0 \in X$ is $\pi_1(X,x_0) = \Omega(X,x_0)/\sim_e$. Write $[\gamma]$ for the equivalence class in $\pi_1$.
- $[\gamma][\gamma'] = [\gamma\gamma']$, $[c_{x_0}] = 1$, $[\gamma]^{-1} = [\gamma^{-1}]$ make $\pi_1$ a group.
- Let $f \colon X \to Y$, $f(x_0) = y_0$. Then $\Omega(X,x_0) \to \Omega(Y,y_0)$ is given by left-composition with $f$. This descends to the induced homomorphism $f_\star \colon \pi_1(X,x_0) \to \pi_1(Y,y_0)$ given by $[\gamma] \mapsto [f \circ \gamma]$.
- The induced map is functorial.
- If $f_0, f_1 \colon (X,x_0) \to (Y,y_0)$ are homotopic rel $x_0$, then $(f_0)_\star = (f_1)_\star$.
- $\pi_1$ is a topological invariant.
- Let $\iota \colon A \to X$ be the inclusion and $p \colon X \to A$. $p$ is a retraction if $p \circ \iota = \mathrm{id}_A$, and a strong deformation retraction if additionally $\iota \circ p \sim \mathrm{id}_X$ rel $A$.
- $\iota_\star$ is injective and $p_\star$ is surjective, as $p_\star \circ \iota_\star = 1$. For an sdr, $\iota_\star$ and $p_\star$ are isomorphisms.
- If $p \colon X \to A$ is an sdr, $X \sim A$.

$f \colon X \to Y$ is null-homotopic if $f \sim c_p$ for some $p \in Y$.
- Functions from contractible spaces are null-homotopic.
- $f \colon S^1 \to Y$ extends to $D^2$ iff $f$ is null-homotopic.
- Let $\gamma \in \Omega(X,x_0)$. Define $\overline \gamma \colon S^1 \to X$ by $\overline \gamma(e^{2\pi i t}) = \gamma(t)$.
- $\gamma_0 \sim_e \gamma_1$ implies $\overline \gamma_0 \sim \overline \gamma_1$.
- $\overline{\gamma\gamma'} = \overline{\gamma'\gamma}$ by composition with the antipodal map, which is homotopic to the identity.
Let $\gamma_0, \gamma_1 \in \Omega(X,p,q)$. TFAE:
- $\gamma_0 \sim_e \gamma_1$;
- $\overline{\gamma_0 \gamma_1^{-1}}$ is null-homotopic;
- $[\gamma_0\gamma^{-1}] = 1$ in $\pi_1(X,p)$.
TFAE:
- $\gamma_0 \sim_e \gamma_1$ for all $\gamma_0, \gamma_1 \in \Omega(X,p,q)$ and all $p,q \in X$;
- any map $S^1 \to X$ is null-homotopic;
- $\pi_1(X,x_0) = 1$ for all $x_0 \in X$.

Changing basepoint.
- Let $X_0$ be the path-connected component of $X$ containing $x_0 \in X$. If $Z$ is path-connected and $f \colon Z \to X$ is a map with $x_0$ in its image, $\mathrm{Im}\, f \subseteq X_0$.
- Let $\iota$ be the inclusion from the path-component $X_0$ to $X$. Then if $Z$ is path-connected, $f \colon Z \to X$ factors through $\iota$.
- $\iota_\star$ is an isomorphism.
- For $u \in \Omega(X,x_0,x_1)$, define $u_\sharp \colon \Omega(X,x_0) \to \Omega(X,x_1)$ by $\gamma \mapsto u^{-1} \gamma u$. This descends to a map between fundamental groups.
- $u_\sharp$ is a group isomorphism with inverse $(u^{-1})_\sharp$.
- If a space is path-connected and its fundamental group is trivial at all points, we say the space is simply connected.
- A space is simply connected if it is path-connected and its fundamental group is trivial at any point.
- Let $f_0, f_1 \colon X \to Y$ be homotopic. Let $u$ be the path traced out by $x_0 \in X$ under the homotopy. Then $f_{1\star} = u_\sharp \circ f_{0\star}$.
- Let $X \sim Y$ via $f \colon X \to Y$ and $g \colon Y \to X$. Then $g_\star \colon \pi_1(Y,f(x_0)) \to \pi_1(X,g(f(x_0)))$ is an isomorphism of fundamental groups, as it is injective and surjective by checking left and right compositions with appropriate $f_\star$.
- Contractible spaces are simply connected.