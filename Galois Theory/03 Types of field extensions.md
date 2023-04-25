Fields from polynomials.
- Let $L_f = K[T]/(f)$ where $f$ irreducible. Then $(f)$ maximal so $L_f$ a field, so $L_f/K$ is a finite extension of degree $\deg f$ where $f$ is the minimal polynomial for $t$.
- A K-homomorphism between L/K and M/K is $\sigma \colon L \to M$ restricting to the identity on $K$.
- If $x \in L$ is a root of $f$, there exists a unique K-homomorphism $L_f \to L$ mapping $T + (f) \mapsto x$. Every K-homomorphism $L_f \to L$ arises in this way.
- If $L = K(x)$, there is a unique K-isomorphism $\sigma \colon L_f \to K(x)$ with $\sigma(T + (f)) = x$.
- Elements are K-conjugate if they have same minimal polynomial. Hence K-conjugate iff there is a K-isomorphism $K(x) \to K(y)$ mapping $x$ to $y$.
- Previous theorem phrased another way with $\sigma \colon K \to L$: if $x \in L$ is a root of $f$, there is a unique $\sigma$-homomorphism $\tau \colon L_f \to L$ mapping $\tau(T + (f)) = x$, and every $\sigma$-homomorphism is of this form.
- By previous point, there is a bijection between $\sigma$-homomorphisms $L_f \to L$ and roots of $f$ in $L$.

Splitting fields.
- L is a splitting field for $f$ if L = K(roots). So $f$ splits into linear factors, and this is the smallest such field.
- Every nonzero polynomial has a splitting field (induction on irreducible factors, use $L_f$ idea).
- Let $L/K$, $\sigma \colon K \to M$. Let $L$ be a splitting field for $f$, and $\sigma f$ split in $\sigma K$. Then $\sigma$ can be extended into a homomorphism $L \to M$, and if $M$ is a splitting field for $\sigma f$, such an extension is an isomorphism. So any two splitting fields are K-isomorphic.

Normal extensions.
- L/K is normal if it is algebraic and the minimal polynomial of every element splits. Equivalently L has a splitting field for all of its elements.
- L/K is normal iff L is a splitting field for some (not necessarily irreducible) polynomial.
- Any finite L/K has a unique (up to L-isomorphism) normal closure M (so M/K is normal and M contains L), which is finite over L.

Separable polynomials.
- A root is simple iff the derivative at that point is nonzero.
- A polynomial is separable iff it splits into distinct linear factors in a splitting field. Equivalently, has $\deg f$ distinct roots.
- $f$ separable iff $f, f'$ coprime.
- Irreducible $f$ separable iff $f' \neq 0$.
- Every irreducible is separable in char zero. Irreducibles are separable in char $p$ iff $f(T) = g(T^p)$.

Separable extensions.
- $x \in L$ separable over $K$ if algebraic and min poly separable. L separable iff all elements separable.
- Suppose $m_{x,K}$ splits in $L$. Then $x$ is separable over $K$ iff exactly $\deg x$ K-homomorphisms $K(x) \to L$.
- **Counting embeddings**. Let $L = K(x_1, \dots, x_k$) be finite over $K$. Let M/K. Then $|\mathrm{Hom}_K(L,M)| \leq [L:K]$ with equality iff
	-  for all i, $m_{x_i}$ splits in $M$; and
	- all $x_i$ are separable over $K$.
- Separably generated implies separable (take normal closure).
- Separability closed under sum, product, inverse.
- **Primitive element theorem**.
	- Infinite: If $K$ is an infinite field and $L = K(x_1, \dots, x_k)$ is separable and finite over $K$, there exists $x$ such that $L = K(x)$.
	- Finite: If $L/K$ is an extension of finite fields, $L = K(x)$ as $L^\times$ is cyclic.