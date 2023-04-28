Let $G$ be a regular grammar.
- $A \to a$ is a terminal rule. $A \to aB$ is a nonterminal rule.
- $S \xrightarrow G \alpha$ gives $\alpha \in \mathbb W \cup \mathbb W V$.
- $S \xrightarrow G \alpha$ for $\alpha \in \mathbb W$ has derivation of length $|w|$: $|w|-1$ nonterminal rules then a terminal rule. Derivation can be non-unique.
- Regular languages closed under concatenation.

DFAs.
- A deterministic automaton is a tuple $(\Sigma, Q, \delta, q_0, F)$, $Q$ is the set of states, $q_0$ is the start state, $F$ is the set of accept states (Think: $F$ for "final" states) (cannot contain $q_0$ as regular languages can't accept the emplty word), $\delta \colon Q \times \Sigma \to Q$ is the transition function.
- Tuple order: Basic things, transition, start states, stop states.
- Define the functorial lift $\hat \delta \colon Q \times \mathbb W \to Q$.
- Language accepted by $D$ is $\mathcal L(D) = \{w \mid \hat \delta(q_0,w) \in F\}$.
- State sequence is the states produced from $q_0$ when reading $w$.
- $f \colon Q \to Q'$ is a DFA homomorphism if $\delta'(f(q), a) = f(\delta(q,a))$, $f(q_0) = q_0'$, $q \in F$ iff $f(q) \in F'$.
- DFA homomorphisms given by bijective $f$ are isomorphisms and have inverses.
- Homomorphic DFAs accept the same language.
- Languages accepted by DFAs are regular. We will show later that regular languages are accepted by DFAs.

NFAs.
- A nondeterministic automaton instead has $\delta \colon Q \times \Sigma \to \mathcal P(Q)$.
- Produces a state set sequence, not a state sequence.
- DFAs are NFAs. NFAs can be simulated by DFAs using exponentially many states.
- Regular grammars are accepted by NFAs. So they are accepted by DFAs.

Pumping lemma.
- $L$ satisfies the regular pumping lemma with pumping number $n$ if every word with length at least $n$ can be split into three parts, and the middle part can be pumped down or up.
- If any word can be pumped, the language is infinite.
- Regular languages satisfy the regular pumping lemma: pigeonhole on states of a DFA.
- (!) Example of nonregular language satisfying pumping lemma.
- If $L$ has pumping number $n$, it has a word of length less than $n$.
- The emptiness problem for regular grammars is solvable by checking its pumping number.

Regex.
- Kleene star $L^\star$. Kleene plus $K^+$.
- Regular expressions are defined to contain $\varnothing, \varepsilon$, letters, closed under union ($+$) and concatenation, Kleene plus and star.
- Assign a regular language to each regex.
- Languages are essentially regular if they have a regular grammar (excluding the empty word).
- Regexes produce essentially regular languages. Converse not required for the course.

Minimisation.
- A state is accessible if it can be reached on some input.
- States are distinguished by a word if the automaton accepts or rejects differently depending on which state they start with.
- Distinguishable states are mapped to distinct states under a homomorphism.
- Accessible states lie in the range of a homomorphism.
- If all pairs of nonequal states in $D$ are distinguishable, $f$ is injective.
- If all states in $D'$ are accessible, $f$ is surjective.
- $D$ is irreducible if all pairs of nonequal states are distinguishable, and all states are accessible.
- Hence, a homomorphism between irreducible automata is an isomorphism.
- Define the quotient automaton by the quotient with indistinguishability.
- After quotienting and removing inaccessible states, we obtain an irreducible DFA for the same language.
- The number of states in the irreducible DFA is at most the number of states in the original.
- Irreducible DFAs that produce the same language are isomorphic. So there is a unique irreducible DFA accepting a regular language.

Equivalence problem (word problem solved for noncontracting grammars, emptiness already solved by pumping lemma).
- It is decidable whether a state is accessible.
- It is decidable if two states are distinguishable (table filling algorithm, iteratively check which states are distinguishable and fill each cell with a word distinguishing them, what remains is indistinguishable).
- Equivalence problem for regular grammars is decidable.