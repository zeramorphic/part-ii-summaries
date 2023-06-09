- $x \in \mathcal O_L$ is a unit iff its norm is $\pm 1$.
- Prime ideals are taken to be nonzero.
- $\mathfrak a \triangleleft \mathcal O_K$ contains an integer (the degree 0 term $a_0$ of the min poly of any of its elements).
- $\mathcal O_K/\mathfrak a$ is finite as $\mathcal O_K / a_0 \mathcal O_k$ surjects onto it.
- Nonzero ideals are isomorphic to $\mathbb Z^n$ as abelian groups.
- $\mathcal O_K$ is an integral domain and Noetherian.
- $\mathcal O_K$ is integrally closed in $K$; $x \in K$ integral over $\mathcal O_K$ implies $x \in \mathcal O_K$.
- Every (nonzero) prime ideal is maximal.

Unique factorisation of ideals.
- $\mathfrak a \mathfrak b \subseteq \mathfrak p$ implies $\mathfrak a \subseteq \mathfrak p$ or $\mathfrak b \subseteq \mathfrak p$ by definition of prime.
- A nonzero ideal contains a product of prime ideals.
- The inverse of $\mathfrak a$ is $\{y \in K \mid y\mathfrak a \subseteq \mathcal O_K\}$.
	- $x\mathfrak a \subseteq \mathfrak a$ implies $x \in \mathcal O_K$ ($xI - A$ has det zero as a linear map $\mathfrak a \to \mathfrak a$).
	- (!) $\mathcal O_K \subsetneq \{y \in K \mid y \mathfrak a \subseteq \mathcal O_K\}$ if $\mathfrak a \neq \mathcal O_K$ is proper.
- A fractional ideal is a finitely generated $\mathcal O_K$-module in $K$.
- $\mathfrak q$ is a fractional ideal iff there is $c \in K$ with $c\mathfrak q \trianglelefteq \mathcal O_K$. This multiplication is an isomorphism of $\mathcal O_K$-modules.
- Fractional ideals are isomorphic to $\mathbb Z^n$ as abelian groups.
- $\mathfrak q^{-1} = \{x \in K \mid x\mathfrak q \subseteq \mathcal O_K\}$. Equivalently, for every integral ideal there is another such that their product is principal.
Conclusions:
- $\mathfrak b \subseteq \mathfrak a \iff \mathfrak b \mathfrak c \subseteq \mathfrak a \mathfrak c$ (multiply by $\mathfrak c^{-1}$ for reverse direction)
- $\mathfrak a \mid \mathfrak b \iff \mathfrak a \mathfrak c \mid \mathfrak b \mathfrak c$ (multiply by $\mathfrak c^{-1}$ for reverse direction)
- $\mathfrak a \mid \mathfrak b \iff \mathfrak b \subseteq \mathfrak a$ (easy if $\mathfrak a$ principal; reduce to this case)
- A nonzero ideal can be written uniquely as a product of prime ideals.
- The nonzero fractional ideals form the group $I_K$ under multiplication. This is the free abelian group generated by the prime ideals in $\mathcal O_K$. An element is integral iff all exponents are nonnegative.

Class group: $\mathrm{Cl}_K = I_K/P_K$ is the cokernel of the map $K^\star \to I_K$.
TFAE ((i) iff (iii) by definition):
- $\mathcal O_K$ is a PID;
- $\mathcal O_K$ is a UFD;
- the class group is trivial.

Norms.
- $N(\mathfrak a) = |\mathcal O_L/\mathfrak a|$. $N(\mathfrak a) \in \mathfrak a \cap \mathbb Z$ as $N(\mathfrak a) \cdot 1 = 0$ in $\mathcal O_L/\mathfrak a$.
- (difficult proof) $N(\mathfrak a \mathfrak b) = N(\mathfrak a)N(\mathfrak b)$.
- If $M \leq \mathbb Z^n$ is a subgroup isomorphic to $\mathbb Z^n$, then $|\mathbb Z^n/M| = \det A$ where $A$ maps a basis of $\mathbb Z^n$ to a basis of $M$.
- $\mathfrak a = \bigoplus_{i=1}^n \mathbb Z\alpha_i$ for some basis $\alpha_i$ of $L/\mathbb Q$ (holds for $\mathcal O_L$, extend by multiplying by $d \in \mathfrak a \cap \mathbb Z$).
- If $\mathfrak a = \bigoplus_{i=1}^n \mathbb Z\alpha_i$ then $\Delta(\alpha_1, \dots, \alpha_n) = N(\mathfrak a)^2 D_L$.
- If $\alpha_i$ generate $\mathfrak a$ as a $\mathbb Z$-module and $\Delta(\alpha_1, \dots, \alpha_n)$ square-free, then $\mathfrak a = \mathcal O_L$ and $D_L$ square-free.
- If $L = \mathbb Q(\alpha)$ and $\alpha \in \mathcal O_L$ has $\Delta(1, \alpha, \dots, \alpha^{n-1})$ square-free, then $\mathbb Z[\alpha] = \mathcal O_L$.
- If $L = \mathbb Q(\alpha)$ and $\alpha \in \mathcal O_L$, and $d \in \mathbb Z$ is maximal such that $d^2 \mid \Delta(1, \alpha, \dots, \alpha^{n-1})$, then $\mathbb Z[\alpha] \subseteq \mathcal O_L \subseteq \frac{1}{d} \mathbb Z[\alpha]$.
- $N((\alpha)) = |N(\alpha)|$.

Prime ideals.
- For $\mathfrak p$ prime, there is a unique $p$ prime such that $\mathfrak p \mid (p)$.
- $N(\mathfrak p) = p^f$ for some $1 \leq f \leq n$.
- Suffices to only factorise $(p)$ for $p \in \mathbb N$ prime to find all prime ideals in $\mathcal O_L$.

> [!theorem]
> **Dedekind's criteria**. Let $p \nmid |\mathcal O_L/\mathbb Z[\alpha]|$. Then if
> $$\overline m_\alpha(x) = \overline\varphi_1^{e_1} \dots \overline \varphi_r^{e_r};\quad \overline\varphi_i \text{ irreducible mod } p$$
> we have
> $$(p) = \mathfrak p_1^{e_1} \dots \mathfrak p_r^{e_r};\quad \mathfrak p_i = (p, \varphi_i(\alpha))$$

- We say that
	- $p$ ramifies if some $e_i > 1$;
	- $p$ inert if $(p)$ prime;
	- $p$ splits if all $e_i = 1$.
- Let $p \nmid |\mathcal O_L/\mathbb Z[\alpha]|$. If $p < n$, then $p$ does not split completely.
- In general, $(p) = \mathfrak p_1^{e_1} \dots \mathfrak p_r^{e_r}$ with $\mathcal O_L/\mathfrak p_i = \mathbb F_p[x]/\overline\varphi_i(x)$ where $\overline\varphi_i$ is irreducible and $N(\mathfrak p_i) = p^{f_i}$, and $\mathcal O_L/(p) \simeq \prod_{i=1}^r \mathbb F_p[x]/\overline\varphi_i(x) = \prod_{i=1}^r \mathbb F_{p^{f_i}}$.
- $p$ ramifies in $L$ iff $p \mid D_L$.