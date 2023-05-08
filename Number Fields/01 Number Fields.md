- A number field is a finite extension of $\mathbb Q$.
- An algebraic integer is a root of a monic polynomial over $\mathbb Z$.
- If $R \subseteq S$ are rings,
	- $\alpha \in S$ is integral over $R$ if it is a root of a monic polynomial over $R$;
	- $S$ is integral over $R$ if its elements are integral over $R$;
	- $S$ is finitely generated over $R$ if it is finitely generated as an $R$-module ($R$-linear combination of finitely many $\alpha_i \in S$).
- An algebraic integer is an element of a number field that is integral over $\mathbb Z$.
- $\mathcal O_L$ is integral over $\mathbb Z$.
- $R[s]$ is finitely generated over $R$ if $s$ integral over $R$.
- $S$ finitely generated over $R$ implies $S$ integral over $R$. Proof: let $s \in S$ and consider the matrix $B$ of $m_s \colon S \to S$ in the $R$-basis; then $sI - B$ acting on the vector of basis elements is zero, so its determinant vanishes.
- $C/B/A$ integral implies $C/A$ integral.

Minimal polynomials.
- Minimal polynomials divide all polynomials that have a common root.
- An element is an algebraic integer iff its minimal polynomial over $\mathbb Z$ is monic.
- For all $\alpha \in L$ there is $n \in \mathbb Z \setminus \{0\}$ such that $n\alpha \in \mathcal O_L$.

Integral basis.
- $\alpha \in L$ is an algebraic integer iff its minimal polynomial has integer coeffs, iff the characteristic polynomial of $m_\alpha$ has integer coeffs.
- $\mathcal O_L = \mathbb Z[\sqrt d]$ for $d \equiv 2, 3$; $\mathcal O_L = \mathbb Z[\frac{1}{2}(1 + \sqrt d)]$ for $d \equiv 1$.
- A basis $\alpha_1, \dots, \alpha_n$ of $L$ is an integral basis if $\mathcal O_L = \bigoplus_{i=1}^n \mathbb Z \alpha_i$.
- Integer bases are related by $GL_n(\mathbb Z)$.
- There are $[L:\mathbb Q]$ embeddings of $L$ into $\mathbb C$; use primitive element theorem and separability.
- Trace and norm are given by sums and products of the Galois conugates.
- If $L/K$ separable, $(x,y)\mapsto\mathrm{Tr}(xy)$ is a nondegenerate inner product.
- $\Delta(\alpha_1, \dots, \alpha_n) = \det \mathrm{Tr}(\alpha_i \alpha_j)$ is nonzero for a basis as trace is nondegenerate.
- The inner product of algebraic integers is an integer.
- If $\alpha_i$ is an integral basis, $\Delta(\alpha_1, \dots, \alpha_n)$ is an integer.
- There is an integral basis for any number field (minimality of $\Delta$ over all bases of $L$ using only algebraic integers).
- $D_l = \Delta(\alpha_1, \dots, \alpha_n)$ for an integral basis $\alpha_1, \dots, \alpha_n$.