- A register machine has finitely many LIFO registers each containing a word $w \in \mathbb W$.
- A snapshot/configuration is a tuple $(q, w_0, \dots, w_n) \in Q \times \mathbb W^{n+1}$ where $Q$ is a nonempty finite set of states.
- $\delta \colon Q \times \mathbb W^{n+1} \to Q \times \mathbb W^{n+1}$.
- $+(k,a,q), ?(k,a,q,q'), ?(k,\varepsilon,q,q'),-(k,q,q')$ are the $(\Sigma, Q)$-instructions.

A $\Sigma$-RM is $M = (\Sigma, Q, P)$ where $q_S, q_H \in Q$ are the start and halt states, and $P \colon Q \to \mathrm{Instr}(\Sigma,Q)$ is the program.
- Can describe a program as a finite list of program lines.
- The upper register index is the largest register referenced in a program (exists by finiteness).
- Define computation sequence as usual. The computation sequence is infinite.
- Halts at time $k$ / in $k$ steps. Register content at time of halting.
- RMs are strongly equivalent if they have the same register content at all time, and halt at the same time, all for every input.
- **Padding lemma**. There are infinitely many RMs in each strong equivalence class.
- There are only countably many strong equivalence classes of RMs.

Performing operations and answering questions.
- An operation is a partial $\mathbb W^{n+1} \rightharpoonup \mathbb W^{n+1}$.
- A question with $k+1$ answers is a partition of $\mathbb W^{n+1}$ into $k+1$ sets $A_i$.
- An RM answers a question if it has $k+1$ answer states $\overline q_i$ and always reaches one after finitely many steps, and the register content cannot be different.
- Operations performable by RMs are closed under concatenation and case distinction.