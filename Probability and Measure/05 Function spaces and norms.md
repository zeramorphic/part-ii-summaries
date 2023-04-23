- A norm on a real vector space is a subadditive function that preserves scalar multiplication, zero iff input is zero.
- If $1 \leq p < \infty$, $\|f\|_p = \sqrt[p]{\int_E |f(x)|^p \,\mathrm{d}\mu(x)}$.
- $\|f\|_\infty = \mathrm{ess\,sup}\,f = \inf \{\lambda \geq 0: |f| \leq \lambda \text{ a.e.}\}$ is the smallest almost-everywhere upper bound.
- $L^p$ is the space of measurable $f \colon E \to \mathbb R$ with finite $\|f\|_p$.

Four key inequalities on function spaces.
- Markov's inequality: $\mu(f \geq \lambda) \leq \frac{\mu(f)}{\lambda}$ by integrating $\lambda \mathbb 1_{\{f \geq \lambda\}} \leq f$.
- Jensen's inequality: $c(\mathbb E[X]) \leq \mathbb E[c(X)]$ for convex $c$, if $X$ is finite in expectation.
- Hölder's inequality: $\mu(|fg|) \leq \|f\|_p \cdot \|g\|_q$ if $\frac{1}{p} + \frac{1}{q} = 1$. Generalises Cauchy-Schwarz (set $p = q = 2$).
- Minkowski's inequality: $\|f + g\|_p \leq \|f\|_p + \|g\|_p$.

So:
- $L^p$ spaces are normed vector spaces (technically, only after taking quotient by "difference has zero integral" equivalence relation, giving $\mathcal L^p$).
- In fact, $\mathcal L^p$ is a Banach space (complete normed vector space).
- The Cauchy completion of $(V,\|\cdot\|)$ on $[a,b]$ is $L^1(\mu)$ if $V$ is "continuous functions", "simple functions", etc.

$\mathcal L^2$ is special because we have an inner product $\langle f, g \rangle = \int_E fg \,\mathrm{d}\mu$.
- A set is closed iff every sequence converges a.e. to something in that set (a.e. as we're in $\mathcal L^2$ not $L^2$).
- Can take orthogonal complement in $\mathcal L^2$. Orthogonal decomposition $f = v + u$ where $v \in V$ and $u \in V^\perp$, and this is such that $v \in V$ has $\|f - v\|_2$ minimal (unique minimiser in $\mathcal L^2$). This $v$ is called the projection of $f$ onto $V$.

More notions of convergence...
- **Bounded convergence theorem**. Let $X_n$ be random variables all bounded by $C < \infty$, converging in probability to $X$. Then $X_n \to X$ in $L^1(\mathbb P)$.
- (!) Let $\mathcal X$ be a collection of r.vs. They are uniformly integrable if they are bounded in $L^1(\mathbb P)$ and $$\sup\{\mathbb E[|X|\mathbb 1_A] \mid \mathbb P(A) \leq \delta, X \in \mathcal X\} \downarrow 0$$ as $\delta \downarrow 0$.
- $\mathcal X$ is uniformly integrable iff $\sup_{X \in \mathcal X} \mathbb E[|X|\mathbb 1_{\{|X| > K\}}] \to 0$.
(!) TFAE:
- $X_n, X \in L^1(\mathbb P)$ and $X_n \to X$ in $L^1(\mathbb P)$;
- $X_n$ are u.i. and $X_n \to X$ in probability.