- Let $C$ be cyclic of order $n > 1$, and $a \in \mathbb Z$ coprime to $n$. Then $[a] \colon C \to C$ given by $[a](g) = g^a$ is an automorphism of $C$. $(\mathbb Z/n\mathbb Z)^\times \to \mathrm{Aut}(C)$ given by $a \mapsto [a]$ is an isomorphism.
- $\boldsymbol\mu_n(K)$ is the group of $n$th roots of unity in $K$. Cyclic as a subgroup of $K^\times$. Order divides $n$, as each element has order dividing $n$.
- $\zeta \in \boldsymbol\mu_n(K)$ is primitive if it has order $n$, and if one exists, it generates the group.
- If there is a primitive root, $f = T^n - 1$ has $n$ distinct roots and is hence separable. In general $f$ is separable iff $f$ coprime with $f'$, so iff $n \neq 0$.

Assume $K$ has characteristic not dividing $n$, so $T^n - 1$ separable.
- A splitting field L for $T^n - 1 \in K[T]$ is Galois over K as $f$ is separable. In this case, there is a primitive root $\zeta \in L$, and $L$ is called a cyclotomic extension.
- There is an injective homomorphism $\chi \colon \mathrm{Gal}(K(\zeta)/K) \to (\mathbb Z/n\mathbb Z)^\times$ where $\chi(\sigma) = a$ implies $\sigma(\zeta) = \zeta^a$; this homomorphism is called the cyclotomic character.
- $\chi$ is an isomorphism iff $G$ is transitive on $\boldsymbol\mu_n(L)$.

The $n$th cyclotomic polynomial is $$\Phi_n(t) = \prod_{a \in (\mathbb Z/n\mathbb Z)^\times} (T - \zeta_n^a)$$ in a splitting field of $T^n - 1$.
- The roots of $\Phi$ are precisely the primitive $n$th roots of unity.
- $G$ permutes the primitive $n$th roots of unity in $L$, so $\Phi$ has coefficients in $L^G = K$.
- $T^n - 1 = \prod_{d \mid n} \Phi_d$.
- The $\Phi_n$ do not depend on $K$, since they are the image in $K[T]$ of a polynomial in $\mathbb Z[T]$ using the formula $\Phi_n = \frac{T^n - 1}{\prod_{d \mid n, d \neq n} \Phi_d}$.
- $\deg \Phi_n = (\mathbb Z/n\mathbb Z)^\times = \varphi(n)$.

We have the following theorem on the cyclotomic character.
- Rationals: For $K = \mathbb Q$,: $\chi_n$ is an isomorphism for all $n > 1$. In particular, $[\mathbb Q(\zeta_n) : \mathbb Q] = \varphi(n)$, and $\Phi_n$ is irreducible over $\mathbb Q$.
- Finite fields: Let $K = \mathbb F_p$, $(n, p) = 1$, $L$ a splitting field for $T^n - 1$. Then $\chi_n$ is an isomorphism from $\mathrm{Gal}(L/K)$ to $\langle p \rangle \leq (\mathbb Z/n\mathbb Z)^\times$. In particular, $\chi(\varphi_p) = p$.
- Further, in this case, $[L:K] = r$ where $r$ is the order of $p$ mod $n$. $\varphi_p$ has cycle type $(r, \dots, r)$ as a permutation on the roots of $\Phi_n$.

Construction of regular polygons.
- $2^m + 1$ is prime implies $m$ is a power of two.
- The Fermat numbers are $2^{2^k}+1$. Fermat primes are prime Fermat numbers.
- (difficult proof) A regular $n$-gon is constructible iff $n$ is a power of two multiplied by a product of distinct Fermat primes.

Linear independence.
- **Linear independence of characters**. Let $G$ a group, $L$ a field, $\sigma_1, \dots, \sigma_n \colon G \to L^\times$ distinct group homomorphisms. Then $\sigma_1, \dots, \sigma_n$ are $L$-linearly independent.
- **Linear independence of field embeddings**. Let $K, L$ be fields, and let $\sigma_1, \dots, \sigma_n \colon K \to L$ distinct field homomorphisms. Then $\sigma_1, \dots, \sigma_n$ are $L$-linearly independent.

Let $\zeta_n \in K, L = K(x), x^n = a \in K^\times$. Such extensions are called Kummer extensions.
- $L/K$ is a splitting field for $f = T^n - a$.
- $L/K$ is Galois as $f$ is separable.
- $L/K$ has cyclic Galois group.
- $[L:K]$ is the least $m \geq 1$ with $x^m \in K$.
- $f = T^n - a$ is irreducible over $K$ iff $a$ is not a $d$th power in $K$ for any $1 \neq d \mid n$.
- Any Galois extension $L/K$ with $\zeta_n \in K$ and cyclic Galois group of order $n$ is a Kummer extension. Uses Lagrange resolvents:$$x = R(y) = \sum_{j=0}^{n-1} \zeta^{-j} \sigma^j(y) \in L$$and then $L = K(x)$ as $\sigma(x) = \zeta(x)$. A suitable $y$ exists by linear independence of field embeddings.