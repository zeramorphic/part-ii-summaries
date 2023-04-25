A field is algebraically closed if every non-constant polynomial splits, or equivalently, the irreducible polynomials are the linear polynomials.
TFAE:
- K algebraically closed;
- for all L/K, $x \in L$ algebraic, $x \in K$;
- L/K algebraic implies $L = K$.

If L/K is algebraic and every irreducible splits, it is algebraically closed. Such a field is called an algebraic closure.
- If $K$ is a countable field, it has an algebraic closure, as we can enumerate the monic irreducibles, inductively define $L_i$ to be a splitting field for $f_i$ over $L_{i-1}$, and take unions. So for example $\mathbb F_p$ has an algebraic closure.
- If L/K is algebraic and M is algebraically closed, $\sigma \colon K \to M$ extends to some $\overline\sigma \colon L \to M$ by Zorn.
- **Maximal ideal theorem**. Every nonzero commutative ring with 1 has a maximal ideal, by Zorn.
- Every field has an algebraic closure. (difficult proof using maximal ideal theorem)
- We can extend an isomorphism $K \to K'$ to an isomorphism $\overline K \to \overline K'$ (not uniquely).