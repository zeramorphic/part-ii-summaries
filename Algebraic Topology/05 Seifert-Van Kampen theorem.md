Free groups.
- A free group with generating set $S$ is a group $F_S$ with $S \subseteq F_S$ such that when $G$ is a group and $\varphi \colon S \to G$ is any map of sets, there is a unique homomorphism $\Phi \colon F_s \to G$ restricting to $\varphi$ on $S$.
- The fundamental group of $S_1 \vee S_1$ is the free group on two elements.
- Free groups on bijective sets are isomorphic.

Presentations.
- $\langle S \rangle$ is the smallest subgroup containing $S$.
- $\langle\!\langle S \rangle\!\rangle$ is the smallest normal subgroup containing $S$.
- $\langle S \mid R\rangle = F_S/\langle\!\langle R \rangle\!\rangle$.
- Let $S$ generate $G$ and $\Phi_S \colon F_S \to G$. If $\langle\!\langle R \rangle\!\rangle = \ker \Phi_S$ then $G \simeq \langle S \mid R \rangle$. This is a presentation of $G$.
- Any group admits a presentation.
- For $a \not\in S$ and $w \in F_S$, $\langle S \mid R \rangle \simeq \langle S \cup \{a\} \mid R \cup \{a w^{-1}\} \rangle$.
- There is no algorithm to determine if a finite presentation presents the trivial group.

Covering with a pair of open sets.
- Suppose $X$ is covered by open sets $U_1, U_2$, and $U_1 \cap U_2$ is path-connected and contains $x_0$. Then the union of the two fundamental groups $\pi_1(U_i, x_0)$ (under appropriate inclusions $\iota_{i\star}$) generates $\pi_1(X, x_0)$. (uses Lebesgue covering lemma, $\gamma^{-1}(U_1), \gamma^{-1}(U_2)$ forms an open cover of $I$)
- The union of two simply connected spaces with path-connected intersection is simply connected.
- The fundamental group of the $n$-sphere for $n>1$ is trivial by taking the two open sets to be the complements of the poles.
- If $f \colon S^1 \to X$, define $X \cup_f D^2 = X \amalg D^2 / \sim$ where $z \sim f(z)$ for $z \in S^1$. Then $\pi_1(X \cup_f D^2) \simeq \pi_1(X)/\langle\!\langle f_\star(1) \rangle\!\rangle$.

Amalgamated free products.
- $\iota_1 \colon H \to G_1$ and $\iota_2 \colon H \to G_2$ push out to form the amalgamated free product $G_1 \ast_H G_2$.
- Amalgamated free products always exist (considering presentations) and are unique up to isomorphism.

> [!theorem]
> **Seifert-Van Kampen**. Let $X = U_1 \cup U_2$ where $U_i$ are open and $U_1 \cap U_2$ path-connected and contains $x_0$. Then $\pi_1(X) = \pi_1(U_1) \ast_{\pi_1(U_1 \cap U_2)} \pi_1(U_2)$.

For example $\pi_1(T^2) = \mathbb Z^2$.