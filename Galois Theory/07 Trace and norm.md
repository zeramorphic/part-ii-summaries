$\mathrm{Tr}(x) = \mathrm{tr}\, U_x, N(x) = \det U_x, f_x = \det (TI - U_x)$ where $U_x \colon L \to L$ is the $L$-linear (hence $K$-linear) map given by $y \mapsto xy$.
Let $x, y \in L, a \in K, n = [L:K]$.
- $\mathrm{Tr}(x+y) = \mathrm{Tr}(x) + \mathrm{Tr}(y)$
- $N(xy) = N(x)N(y)$
- $N(x) = 0$ if and only if $x = 0$
- $\mathrm{Tr}(1) = n$
- $N(1) = 1$
- $\mathrm{Tr}(ax) = a\mathrm{Tr}(x)$
- $N(ax) = a^n N(x)$
- $\mathrm{Tr}_{L/K} \circ \mathrm{Tr}_{M/L} = \mathrm{Tr}_{M/K}$
- $N_{L/K} \circ N_{M/L} = N_{M/K}$ (not proven in lectures)
- If $L = K(x)$, $f_x = m_{x,K}$, so if $m_{x,K} = T^n + c_{n-1} T^{n-1} + \dots + c_0$ we have $\mathrm{Tr}(x) = -c_{n-1}, N(x) = (-1)^n c_0$. Proof uses basis $1, x, \dots, x^{n-1}$.
- If $K$ has characteristic $p > 0$ and $L = K(x)$ where $x \not\in K$ but $x^p \in K$, for all $y \in L$ we have $\mathrm{Tr}(y) = 0$ and $N(y) = y^p$. Proof: minimal polynomial of any element is $T - y$ or $T^p - y^p$.
- $\mathrm{Tr}(x) = \sum \sigma(x), N(x) = \prod \sigma(x), f_x = \prod (T - \sigma(x))$ where $\sigma$ ranges over the distinct $K$-homomorphisms of $L$ into a normal closure $M$ for $L/K$. If $L/K$ is finite and Galois, the $\sigma$ can be taken to be the elements of the Galois group.
- $\mathrm{Tr}$ is the zero map or surjective as it maps to $K$ and is $K$-linear.
- Finite extensions $L/K$ are separable iff $\mathrm{Tr}$ is surjective. (trivial in characteristic zero by considering $\mathrm{Tr}(1) \neq 0$)