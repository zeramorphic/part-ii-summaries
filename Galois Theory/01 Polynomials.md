- A ring is considered commutative, nonzero, with 1.
- Polynomials of degree $n$ in a certain field have at most $n$ roots in that field.
- A polynomial in $n$ variables is symmetric if fixed under the (right-)action of $S_n$.
- The set of symmetric polynomials form a subring of $R[X_1, \dots, X_n]$.
- Elementary symmetric functions/polynomials are $$s_r(X_1, \dots, X_n) = \sum_{i_1<\dots<i_r} X_{i_1}\dots X_{i_r}$$
- A monomial is an expression of the form $X_1^{i_1}\dots X_n^{i_n}$, its degree is the sum of the powers.
- A term is a scalar multiple of a monomial. Monomials are (totally) lexicographically ordered.

> [!theorem]
> **Fundamental theorem of symmetric polynomials**. Every symmetric polynomial is expressible as a unique polynomial in the elementary symmetric polynomials.

> [!theorem]
> **Newton's formulae**. Let $n \geq 1$. Then for all $k \geq 1$, $$p_k - s_1 p_{k-1} + \dots + (-1)^{k-1} s_{k-1} p_1 + (-1)^k ks_k = 0$$ where $s_0 = 1$ and $s_r = 0$ if $r > n$, and $p_j = \sum_i X_i^j$.

- The discriminant polynomial is $D(X_1, \dots, X_n) = \Delta(X_1, \dots, X_n)^2$ where $\Delta(X_1, \dots, X_n) = \prod_{i < j} (X_i - X_j)$. $D$ is symmetric, and we write $$D(X_1, \dots, X_n) = d(s_1, \dots, s_n)$$
- The discriminant of a polynomial $f = T^n + \sum_{i=0}^{n-1} a_{n-i} T^i$ is $$\mathrm{Disc}(f) = d(-a_1, a_2, \dots, (-1)^n a_n) \in R$$