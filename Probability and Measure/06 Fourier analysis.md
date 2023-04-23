For a function,
$$\hat f(u) = \int_{\mathbb R^d} f(x) e^{i\langle u, x\rangle} \,\mathrm{d}x$$
For a measure,
$$ \hat\mu(u) = \int_{\mathbb R^d} e^{i \langle u, x\rangle} \,\mathrm{d}\mu(x) $$
- FT of a measure is cts by dominated convergence.
- Characteristic function of an r.vector is $$ \varphi_X(u) = \mathbb E[e^{i\langle u, X\rangle}] = \hat\mu_X(u) $$

Convolutions.
- Convolution of a function by a prob. measure is $$ (f \ast \nu)(x) = \int_{\mathbb R^d} f(x-y) \,\mathrm{d}\nu(y) $$ if $y \mapsto f(x-y)$ is $L^1$, and 0 otherwise.
- Convolution of two prob. measures is the prob. measure defined by $$ (\mu \ast \nu)(A) = \mathbb P(X + Y \in A) = \int_{\mathbb R^d \times \mathbb R^d} \mathbb 1_A(x+y) \,\mathrm{d}(\mu \otimes \nu)(x,y) $$
- $\widehat{f \ast \nu}(u) = \hat f(u) \hat \nu(u)$.
- $\widehat{\mu \ast \nu}(u) = \hat\mu(u)\hat\nu(u)$.

Gaussians.
- Define $g_t(x) = \frac{1}{\sqrt{2\pi t}} \exp(-\frac{x^2}{2t})$.
- $\hat g_1(u) = \sqrt{2\pi} g_1(u)$.

> [!theorem]
> **Fourier inversion theorem**. Let $f \in L^1(\mathbb R^d), \hat f \in L^1(\mathbb R^d)$. Almost everywhere, $$f(x) = \frac{1}{(2\pi)^d} \int_{\mathbb R^d} e^{-i\langle u,x\rangle} \hat f(u) \,\mathrm{d}u$$

FT is injective as $\hat f = \hat g$ implies $\widehat{f - g} = 0$ so $f - g = 0$ a.e. Proof: works for Gaussian convolutions, which are dense.

> [!theorem]
> **Plancherel identity**. Let $f \in L^1(\mathbb R^d) \cap L^2(\mathbb R^d)$. Then $\|f\|_2 = (2\pi)^{-\frac{d}{2}} \|\hat f\|_2$.

Have a linear isometry $L^2 \to L^2$ given by extending FT by continuity: the Fourier-Plancherel transform.

- The characteristic function uniquely determines the law of a random variable: $\hat\mu_X$ determines $\mu_X$.
- If $\varphi_X \in L^1$, then $\mu_X$ has a pdf, given a.e. by $$\frac{1}{(2\pi)^d} \int_{\mathbb R^d} e^{-i\langle u, x\rangle} \varphi_X(u) \,\mathrm{d}u$$