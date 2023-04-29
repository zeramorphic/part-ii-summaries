(Skipping proofs in this section.)

- A curve is (for us) a smooth irreducible projective variety of dimension 1.
- Proper closed subvarieties of curves are finite sets.
- (!) $\mathfrak m_P$ is principal at smooth points of irreducible curves (by Nakayama).
- $Q \mapsto X(Q) - X(P)$ is a local parameter iff $\frac{\partial f}{\partial Y}(P) \neq 0$ for smooth points of irreducible plane affine curves $\mathbb V(f)$.
- $\nu_P \colon \mathbb C(V)^\star \to \mathbb Z$ is the valuation or order of vanishing.
- $\mathcal O_{V,P}$ is the set of functions with nonnegative $\nu_P$, together with the zero function.
- $\mathfrak m_P$ is the set of functions with positive $\nu_P$, together with the zero function.
- For $f \in \mathbb C(V)^\star$ we can write $f = \pi_P^{\nu_P(f)} u$ where $u \in \mathcal O_{V,P}^\star$ so it does not vanish at $P$.
- At smooth points of irreducible curves, $f$ or $f^{-1}$ is regular for each $f \in \mathbb C(V)$.
- (!) Any rational map $V \dashrightarrow \mathbb P^m$ is a morphism.

Maps between curves.
- For $\varphi \colon V \to W$ non-constant between irreducible projective curves, the fibres $\varphi^{-1}(Q)$ are finite.
- $\varphi \colon V \to W$ induces an inclusion $\varphi^\star \colon \mathbb C(W) \hookrightarrow \mathbb C(V)$ which makes $\mathbb C(V)$ a finite extension of $\mathbb C(W)$.
- $\deg \varphi = [\mathbb C(V) : \varphi^\star \mathbb C(W)]$.
- $e_P = e(\varphi, P) = \nu_P(\varphi^\star \pi_Q)$.
-  $\varphi \colon V \to W$ non-constant between irreducible projective curves is surjective.
- If $VB, W$ smooth, then $\deg \varphi$ is the sum of the ramification degrees of $\varphi$ on any fibre.
- Only finitely many points ramify.
- **Fundamental theorem of elimination theory**. $\pi_2 \colon \mathbb P^n \times \mathbb A^m \to \mathbb A^m$ is a Zariski closed map.
- Morphisms from projective varieties to quasi-projective varieties are Zariski closed maps.
- If $f \in \mathbb C(V)^\star$ regular at all points, $f$ is constant (not surjective onto $\mathbb P^!$).
- $f \in \mathbb C(V)^\star$ has nonzero valuation at only finitely many points.
- The sum of the valuations of $f \in \mathbb C(V)^\star$ at all points is zero.

Divisors.
- The group of divisors on a curve is the free abelian group on its points.
- The degree of a divisor is the sum of the coefficients on its basis elements.
- $\mathrm{div}(f) = \sum_{P \in V} \nu_P(f) [P] \in \mathrm{Prin}(V)$.
- $L(D) = \{f \in \mathbb C(V) \mid f = 0 \text{ or } \mathrm{div}(f) + D \geq 0\}$.
- $\mathrm{Cl}(V) = \mathrm{Div}(V)/\mathrm{Prin}(V)$.
- $D \sim D' \iff D - D' \in \mathrm{Prin}(V)$.
- Principal divisors are degree zero. Converse holds in $V = \mathbb P^1$.
- The hyperplane section of $V$ by $L$ homogeneous linear is $\mathrm{div}(L) = \sum_{P \in V} n_P [P]$ where if $X_i(P) \neq 0$, $n_P = \nu_P(L/X_i)$.
- $\mathrm{div}(L) - \mathrm{div}(L') = \mathrm{div}(L/L') \in \mathrm{Prin}(V)$ so the degrees match.
- **Bézout's theorem (weak form)**. If $V \neq V'$ are curves of degrees $m, n$ in $\mathbb P^2$, they intersect in at most $mn$ points.

Function spaces from divisors.
- A divisor is effective if it is pointwise nonnegative.
- $L(D)$ is the set of functions for which $\mathrm{div}(f) + D$ is effective.
- $L(D)$ is a complex vector subspace of $\mathbb C(V)$.
- $\ell(D) = \dim_{\mathbb C} L(D)$.
- $\deg D < 0$ implies $L(D) = 0$.
- $\ell(D) \leq \ell(D - P) + 1$.
- Hence, $\deg D \geq 0$ gives $\ell(D) \leq \deg D + 1$.
- $L(D)$ is finite-dimensional.
- $D \sim E$ implies $L(D) \sim L(E)$ as $\mathbb C$-vector spaces.