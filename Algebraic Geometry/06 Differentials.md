- $\Omega_{K/\mathbb C}$ is given by $\{\delta x \mid x \in K\} / (\delta(x+y) - \delta(x) - \delta(y), \delta(xy) - x\delta(y) - y\delta(x), \delta(a))$.
- The exterior derivative is the $\mathbb C$-linear map $\mathrm{d} \colon K \to \Omega_{K/\mathbb C}$.
- A $\mathbb C$-linear $D \colon K \to U$ is called a derivation if $D(xy) = xDy + yDx$.
- $\mathrm{d}$ is a derivation.
- **Universal property**. Derivations factor through $\Omega$ and $\mathrm{d}$.
- **Multivariate chain rule**. $\mathrm{d}y = \sum_{i=1}^n \frac{\partial f}{\partial X_i}(x_1, \dots, x_n) \,\mathrm{d}x_i$ where $y = f(x_1, \dots, x_n)$.
- $\Omega_{K/\mathbb C}$ is spanned by the $\mathrm{d}x_i$ as a $K$-vector space where the $x_i$ generate $K$ over $\mathbb C$.
- $K/\mathbb C(t)$ finite and $t$ transcendental implies $\Omega_K$ is one-dimensional as a $K$-vector space and spanned by $\mathrm{d}t$.

Rational differentials.
- $\Omega_V = \Omega_{\mathbb C(V)/\mathbb C}$ is the space of rational differentials.
- $\omega \in \Omega_V$ is regular at $P \in V$ if $\omega = \sum_i f_i \,\mathrm{d}g_i$ where $f_i, g_i \in \mathcal O_{V,P}$.
- $\Omega_{V,P}$ is the set of rational differentials that are regular at $P$, which is an $\mathcal O_{V,P}$-module.
- $\Omega_{V,P}$ is a free $\mathcal O_{V,P}$-module generated by $\mathrm{d}\pi_P$ so $\Omega_{V,P} = \{f\,\mathrm{d}\pi_P\mid f \in \mathcal O_{V,P}\}$.
- Define $\nu_P(f\,\mathrm{d}\pi_P) = \nu_P(f)$.
- $\nu_P(\omega) \neq 0$ for only finitely many points $P$ if $\omega \neq 0$.
- $\mathrm{div}(\omega) = \sum_{P \in V} \nu_P(\omega)[P]$.
- $\mathrm{div}(\omega) - \mathrm{div}(\omega') \in \mathrm{Prin}(V)$ for nonzero $\omega, \omega'$.
- The divisor of any nonzero differential is a representative of the canonical class $K_V \in \mathrm{Cl}(V)$.
- The genus of $V$ is $g(V) = \ell(K_V)$.
- $g(\mathbb P^1) = 0$.

Differentials on plane curves.
- (!) The genus of a smooth plane cubic is 1.
- $K_V = (d-3)H$ for smooth projective plane curves $\mathbb V(F)$ of degree $d$, $H$ is a hyperplane section.
- TODO: the bit about the $x^r y^s$ basis
- Smooth plane curves of degrees $d \neq d'$ are not isomorphic, as $\deg K_V$ depends only on $V$ up to isomorphism.

> [!theorem]
> **Riemann-Roch theorem**. Let $V$ be a smooth irreducible projective curve of genus $g$, and let $D$ be a divisor on $V$. Let $K_V$ be the canonical divisor class. Then,
> $$\ell(D) - \ell(K_V - D) = \deg(D) - g + 1$$

- $\deg K_V = 2g - 2 = -\chi(V)$.
- For plane curves of degree $d$, we have $g(V) = \binom{d-1}{2}$ as $\deg H = d$.
- If $\deg D > 2g-2$, $\ell(D) = \deg D - g + 1$.
- If $g(V) = 1$ and $\deg D > 0$, then $\ell(D) = \deg D$.
- Let $P_0 \in V$ of genus 1. Then for $P, Q \in V$, $[P] + [Q] - [P_0]$ is equivalent to a unique effective divisor $[R]$ of degree 1. This gives the elliptic curve group law $P +_E Q = R$. The map $E \to \mathrm{Cl}^0(E)$ given by $P \mapsto [P - P_0]$ is a group isomorphism.
- For $F = X_0 X_2^2 - \prod_{i=1}^3 (X_1 - \lambda_i X_0)$ and $P_0 = (0 : 0 :1)$, $P +_E Q +_E R = 0_E$ iff $P, Q, R$ colinear.
- (!) $\nu_P(\varphi^\star \mathrm{d}\pi_Q) = e_P - 1$, hence $\nu_P(\varphi^\star \omega) = e_P \nu_Q(\omega) + e_P - 1$.

> [!theorem]
> **Riemann-Hurwitz formula**. Let $\varphi \colon V \to W$ be a morphism of curves, and $n = \deg \varphi, n \neq 0$. Then
> $$2g(V) - 2 = n(2g(W) - 2) + \sum_{P \in V} (e_P - 1)$$
> Equivalently,
> $$\chi(V) = n\chi(W) - \sum_{P \in V} (e_P - 1)$$

- $g(V) < g(W)$ implies that any rational map $V \dashrightarrow W$ (hence morphism $V \to W)$ is constant.

Equations using Riemann-Roch.
- There is an injection from "linear homogeneous polynomials in $\mathbb C[\mathbf X]$" to $L(D)$ given by $G \mapsto G/X_0$.
- For any point $P \in V$, there are linear homogeneous polynomials $F$ nonzero and $G$ zero at $P$.
- If $P$ is smooth and $L$ is the tangent line in $\mathbb P^n$, there is a linear homogeneous polynomial that vanishes on $P$ but not all of $L$.
- $D$ satisfies $(\star)$ if for all $P, Q \in V$, $\ell(D - P - Q) = \ell(D) - 2$.
- The morphism associated to $D$ with $\ell(D) = n+1 \geq 2$ is $(f_0 : \dots : f_n)$ where the $f_i$ are a basis for $L(D)$.
- $\varphi_D$ is an embedding iff $D$ satisfies $(\star)$.
- If $\deg D > 2g$, $D$ satisfies $(\star)$ by RR, so $\varphi_D$ is an embedding.
- Every curve of a fixed genus can be embedded in $\mathbb P^m$ for $m = m(g)$.
- A curve is hyperelliptic if there is a degree 2 morphism to $\mathbb P^1$.
- Hyperelliptic iff there is a degree 2 divisor with $\ell(D) = 2$.
- A curve of genus at least 2 that is not hyperelliptic has $\varphi_{K_V} \colon V \to \mathbb P^{g-1}$ an embedding by RR.