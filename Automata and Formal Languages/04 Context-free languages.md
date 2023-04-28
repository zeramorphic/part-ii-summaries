Trees.
- A set $T \subseteq \mathbb N^\star$ is called a finitely-branching tree if it is closed under initial segments, and for all $t \in T$ there is a branching number $n \in \mathbb N$ such that $tk \in T$ iff $k < n$.
- Nodes with no successors are leaves.
- The empty sequence is the root.
- A node las level $k$ if the length of the sequence is $k$.
- There is a maximum level called the height.
- The sequence $t|_0, t|_1, \dots, t|_{|t|}$ is the branch leading to $t$.
- $T_t = \{s \mid ts \in T\}$ is the subtree starting from $t$.
- The left-to-right order on $T$ is $t < s$ if the minimal $k$ such that $t(k) \neq s(k)$ has $t(k) < s(k)$.

Parse trees. Let $G$ be a CFG.
- $(T, \ell)$ is a $G$-parse tree if $T$ is a tree and $\ell \colon L \to \Omega$ is a labelling function such that $\ell(\varepsilon) \in V$; $\ell(t) \in \Sigma$ implies $t$ has no successors; if $t$ has $n+1$ successors and $\ell(t) = A$, then $\ell(t) \to \ell(t0) \dots \ell(tn) \in P$.
- The string $\sigma_{\mathbb T}$ parsed by a parse tree $\mathbb T$ are its leaves in left-to-right order.
- $t \in T$ gives $\sigma_{\mathbb T} = \alpha \sigma_{\mathbb T_t} \beta$ where $\mathbb T_t = (T_t, \ell_t)$ and $\ell_t(s) = \ell(ts)$.
- $w \in \mathcal L(G)$ iff there is a $G$-parse tree $\mathbb T$ starting from $S$ such that $\sigma_{\mathbb T} = w$.
- Let $\mathbb T$ be a tree, $t \in \mathbb T$. Graft $\mathbb T'$ onto $\mathbb T$ at $t$ if $\ell(t) = A$ and $\mathbb T'$ starts from $A$. Get $\mathsf{graft}(\mathbb T, t, \mathbb T')$.

Chomsky normal form.
- A grammar is in CNF if its rules are of the form $A \to BC$ (binary) or $A \to a$ (unary).
- CNF implies context-free.
- Any derivation of a word in a CNF grammar has length $2|w|-1$.
- Any context-free grammar can be converted to CNF. Fix $A \to \alpha$ where $\alpha$ has a letter and is length at least 2. Unit closure. Remove unit rules. Fix rules with more than one output variable.

Pumping lemma for CFGs.
- A language satisfies the pumping lemma if each word of length at least $n$ can be split into $xuvyz$ where $|uyv| \leq n$ and $|uv| > 0$, and we can pump $u$, $v$ simultaneously.
- Regular pumping lemma implies context-free pumping lemma. (long proof with simple ideas)
- Context-free languages are not closed under intersection (take $a^nb^nc^k$ and $a^kb^nc^n$), so not closed under complement or difference (because they are closed under union).
- CFGs correspond to pushdown automata.
- Emptiness problem is solved by pumping lemma, since no word with length at most $n$ can be the shortest word.