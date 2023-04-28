- $f_{M,k} \colon \mathbb W^k \to \mathbb W$ has $f_{M,k}(\mathbf w) \uparrow$ if it does not halt on input $\mathbf w$, and $f_{M,k}(w) = v_0$ if $\mathbf v$ is the register content at time of halting.
- $W_M = \mathrm{dom}\, f_{M,1}$.
- $f \colon \mathbb W^k \rightharpoonup \mathbb W$ is computable if there is an RM with $f_{M,k} = f$.
- Only countably many computable functions. Computable functions are closed under concatenation and case distinction.

Characteristic functions.
- A total function is a characteristic function for $X \subseteq \mathbb W^k$ if $f(\mathbf w) \neq \varepsilon$ iff $\mathbf w \in X$.
- A total function $\chi_X$ is *the* characteristic function for $X \subseteq \mathbb W^k$ if $f(\mathbf w) = a$ if $\mathbf w \in X$, $f(\mathbf w) = \varepsilon$ else.
- A set is computable if $\chi_X$ is computable.
- A partial function is a pseudocharacteristic function for $X$ if its domain is $X$.
- A partial function $\psi_X$ is *the* pseudocharacteristic function for $X$ if its domain is $X$ and it takes the value $a$ on $X$.
- A set is computably enumerable if $\psi_X$ is computable.
Will show:
- Computable set => CE set
- CE set =/> computable set
- CE <=> type 0 language (has grammar)
- Computable sets lie properly between type 1 and type 0

Computability of languages.
- Computable sets are closed under complement.
- CE <=> the domain of a register machine: $\mathrm{dom}\, f_{M,k}$.
- Regular languages are computable (simulate a DFA).

Shortlex order.
- $w < v$ iff $|w| < |v|$ or $w_n < v_n$ for the least $n$ where they differ.
- This is a total computable order on $\mathbb W$, order-isomorphic under $\#$ to $\mathbb N$.
- The successor function $\#(s(w)) = \#(w) + 1$ is computable.

Church's recursive functions.
- $\pi_{k,i} \colon \mathbb W^k \to \mathbb W$ is the $i$th projection, $c_{k,\varepsilon} \colon \mathbb W^k \to \mathbb W$ is the constant $\varepsilon$, $s \colon \mathbb W \to \mathbb W$ is the successor.
- $\pi, c, s$ are the basic functions.
- Definition by composition: $h(\mathbf w) = f(g_1(\mathbf w), \dots, g_m(\mathbf w))$.
- Definition by recursion: $h(\mathbf w, \varepsilon) = f(\mathbf w)$ and $h(\mathbf w, s(v)) = g(\mathbf w, v, h(\mathbf w, v))$.
- Definition by minimisation: $h(\mathbf w)$ is the minimal $v$ with $f(\mathbf w, v) = \varepsilon$, and all $u < v$ have $f(\mathbf w, u) \downarrow$.
- The class of partial functions is closed under composition, recursion, and minimisation.
- The class of recursive functions is the smallest set containing the basic functions and closed under composition, recursion, and minimisation.
- The class of primitive recursive functions is the smallest set containing the basic functions and closed under composition and recursion.
- Encode recursive functions as labellings of finitely-branching trees. Each node has an arity and a branching number; basic functions do not branch. A partial function is (primitive) recursive iff there is a (primitive) recursion tree encoding it.
- Partial recursive functions are computable; computable functions are closed under composition (already known), recursion, and minimisation.

Merging and splitting. Cantor zigzag function is $$z(i,j) = \frac{(i+j)(i+j+1)}{2} + j \colon \mathbb N \times \mathbb N \to \mathbb N$$
- Define $\#(v \ast w) = z(\#v, \#w)$.
- Define $u = w_{(0)}$ and $v = w_{(1)}$ where $\#w = z(\#u, \#v)$.

Universality.
- Can encode RMs, word sequences, configurations with $\mathbf 0, \mathbf 1, \mathbf +, \mathbf -, \mathbf ?, \mathbf (, \mathbf ), \mathbf ,, \mathbf \mapsto, \mathbf \square$.
- $h(\mathrm{code}(M),\mathrm{code}(\mathbf w),v) = \mathrm{code}(C(M,\mathbf w, \#v))$ (and $\uparrow$ otherwise) is computable.
- $t_{M,k}(\mathbf w, v)$ is the (computable) truncated computation function, taking values in $\{\varepsilon, a\}$.
- **Software principle**. $g(\mathrm{code}(M), \mathrm{code}(\mathbf w)) = f_{M,|\mathbf w|}(\mathbf w)$ (and $\uparrow$ otherwise) is computable.
- A register machine $U$ computing $g$ is called a universal register machine. This has only finitely many registers and states, but can simulate any amount of registers and states.
- Write $f_{v,k}(\mathbf w) = f_{U,2}(v,\mathrm{code}(\mathbf w))$.
- Write $W_v = \mathrm{dom}\,f_{v,1}$.
- $\{W_v \mid v \in \mathbb W\}$ is the set of CE sets.
- **s-m-n theorem**. If $g$ computable, there is a total computable $h$ such that $f_{h(v),k}(\mathbf w) = g(\mathbf w, v)$.

The halting problem.
- $\mathbb K_0 = \{(w,v) \mid f_{w,1}(v)\downarrow\}$ is CE (domain of $f_{U,2}$).
- $\mathbb K = \{w \mid f_{w,1}(w)\downarrow\}$ is CE (domain of $f_{U,2} \circ \Delta$ where $\Delta$ is the (computable) diagonal function).
- **Halting problem**. $\mathbb K_0, \mathbb K$ are not computable.

The arithmetical hierarchy.
- $X$ is $\Sigma_1$ if $\mathbf w \in X \iff \exists y,\,(\mathbf w, y) \in Y$ for a computable set $Y$.
- $X$ is $\Pi_1$ if $\mathbf w \in X \iff \forall y,\,(\mathbf w, y) \in Y$ for a computable set $Y$.
- $\Pi_1$ iff complement of $\Sigma_1$.
- Write $\Delta_1$ if $\Sigma_1$ and $\Pi_1$.
- CE iff $\Sigma_1$. Computable iff $\Delta_1$. Hence $\Sigma_1$ not closed under complementation.
- Type 0 implies CE. Converse true but not proven.

Closure properties.
- Computable sets are closed under intersection, union, complement, difference, concatenation.
- CE sets are closed under intersection, union, and concatenation. Not complement or difference.
- CE iff the image of a partial computable function. Indeed, CE iff the image of a total computable function.

Church-Turing thesis. Register-machine computable iff partial recursive iff "Turing computable" iff "while computable".

Solvability of decision problems.
- Write $G_w$ for the grammar associated to a word. Phrase decision problems as sets that could be computable; say the problem is solvable if the set is computable.
- Word problem: $\{(w,v) \mid w \in \mathcal L(G_v)\}$.
- Emptiness problem: $\{w \mid \mathcal L(G_w) = \varnothing\}$.
- Equivalence problem: $\{(w,v) \mid \mathcal L(G_w) = \mathcal L(G_v)\}$.
- The word problem for type 0 grammars is unsolvable: let $f(w) \uparrow$ iff $w \in \mathcal L(G_w)$, then let $d$ be a word encoding a grammar for $\mathrm{dom}\,f$, then $d \in \mathcal L(G_d) \iff d \not\in \mathcal L(G_d)$ .

Reductions.
- A total computable $f \colon \mathbb W \to \mathbb W$ is a reduction from $A$ to $B$ if $w \in A$ iff $f(w) \in B$.
- $A \leq_m B$. is a preorder; a partial order on equivalence classes.
- $A \leq_m B$ if $A$ is "at most as complicated as" $B$.
- $\varnothing, \mathbb W$ are incomparable and $\leq_m$-minimal. Excluding these, computable sets are $\leq_m$-minimal.
- $A \leq_m B$ and $A$ noncomputable implies $B$ noncomputable. $\mathbb K \leq_m A$ implies $A$ noncomputable.
- $A \leq_m B$ and $A$ not CE implies $B$ not CE. $\mathbb W \setminus \mathbb K \leq_m A$ implies $A$ not CE.
- $\mathbb W \setminus \mathbb K \not\leq_m \mathbb K$ otherwise $\mathbb K$ not CE. Hence $\mathbb K \not\leq_m \mathbb W \setminus \mathbb K$ by complement.
- Turing join $A \oplus B = 0A \cup 1B$, $A \leq_m A \oplus B, B \leq_m A \oplus B$ is the LUB (not proven).
- $A$ is $\mathcal C$-hard if everything in $\mathcal C$ reduces to $A$.
- $A$ is $\mathcal C$-complete if it is in $\mathcal C$ and everything in $\mathcal C$ reduced to $A$.
- $\Delta_1$ sets excluding $\varnothing, \mathbb W$ are $\Delta_1$-complete as they are exactly the nontrivial computable sets.
- (!) $\mathbb K$ is $\Sigma_1$-complete.

Rice's theorem.
- Machines are weakly equivalent if they halt on the same inputs, so $W_M = W_{M'}$.
- Words are weakly equivalent if their corresponding machines are weakly equivalent.
- A language is an index set if it is closed under weak equivalence.
- Index sets are unions of weak equivalence classes.
- $\varnothing, \mathbb W$ are the trivial index sets. Others correspond to properties of CE sets (domains of computable functions).
- (!) **Rice's theorem**. No nontrivial index set is computable. Let $W_e = \varnothing$, then $e \in I$ implies $\mathbb W \setminus \mathbb K \leq_m I$ and $e \not\in I$ implies $\mathbb K \leq_m I$.
- Emp, Fin, Inf, Tot are noncomputable.