- A finite sum of constant multiples of indicator functions is called a simple function.
- The integral of a simple function is defined in the obvious way, by measuring the set under each indicator, then multiplying by the constant.
- The integral of a nonnegative $f \colon E \to \mathbb R$ is the supremum of the integrals of simple functions lying below $f$.
- A function is integrable if its absolute value has finite integral (treated as a nonnegative function).
- The integral of an integrable function is $\mu(f) = \mu(f^+) - \mu(f^-)$ (LHS is being defined, RHS uses definition of integrals of nonnegative functions). This is a real number.

> [!theorem]
> **Monotone convergence theorem**. Let $f_n, f \colon E \to \mathbb R$ be measurable and nonnegative, with $f_n \uparrow f$. Then $\mu(f_n) \to \mu(f)$.

> [!theorem]
> The integral is a linear operator. Let $f, g$ be nonnegative and measurable. $g \leq f \implies \mu(g) \leq \mu(f)$. $f = 0$ a.e. iff $\mu(f) = 0$.

> [!theorem]
> **Fatou's lemma**. For nonnegative measurable $f_n$, we can bound the integral of the liminf. $\mu(\liminf_n f_n) \leq \liminf_n \mu(f_n)$.

> [!theorem]
> **Dominated convergence theorem**. Let $f_n, f$ be measurable and $|f_n| \leq g$ a.e. where $g$ is a $\mu$-integrable dominating function. Let $f_n \to f$ a.e., then $f_n, f$ are integrable and $\mu(f_n) \to \mu(f)$.

We can apply Riemann integration techniques to Lebesgue integration (valid for all bounded measurable functions) using the monotone class theorem.

> [!theorem]
> **Differentiation under the integral sign**. Let $U$ be an open set of reals. Let $f \colon U \times E \to \mathbb R$ be a function parametrised by a real in $U$. Suppose that $f$ is measurable at every $t \in U$, and $f$ is differentiable w.r.t. $t$ for every $x$. Suppose that the derivative $\frac{\partial f}{\partial t}$ is bounded by an integrable dominating function $g$. Then,
> $$ \frac{\mathrm{d}}{\mathrm{d} t} \int_E f(t,x)\,\mathrm{d}\mu(x) = \int_E \frac{\partial f}{\partial t}(t,x)\,\mathrm{d}\mu(x) $$

