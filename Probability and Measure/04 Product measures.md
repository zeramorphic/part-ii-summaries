- Let $\mathcal A = \{A_1 \times A_2 \mid A_1 \in \mathcal E_1, A_2 \in \mathcal E_2\}$. Then let $\mathcal E_1 \otimes \mathcal E_2 = \sigma(\mathcal A)$.
- $\mathcal B(E_1 \times E_2) = \mathcal B(E_1) \otimes \mathcal B(E_2)$ if $E_1, E_2$ have countable bases.
We will show that iterated operations (such as integration) agree with applying the operation on a product space. Then the iterated operations will clearly commute.
- Bounded/nonnegative functions on finite product spaces can be integrated along one variable, and retain the property.
- There is a unique product measure (on the measure space given by $\mathcal E_1 \otimes \mathcal E_2$) such that $\mu(A_1 \times A_2) = \mu_1(A_1) \mu_2(A_2)$ for measurable $A_1, A_2$.

> [!theorem]
> **Fubini's theorem**. Iterated integrals of nonnegative measurable functions commute. Now suppose $f$ is (product-measure-)integrable. If $A_1$ is the set of $x_1 \in E_1$ such that $|f(x_1, x_2)|$ has infinite $x_2$-integral (i.e. $f|_{x_1}$ is not integrable), it is a null set and can be freely removed from the integral calculation. 

"Measurable" means in the product measure space. Can extend finite to $\sigma$-finite.

Product probability spaces are analogous to independent r.vs. TFAE:
- $X_1, \dots, X_n$ are independent
- the product of the laws is the law of the product
- expectation of product is product of expectation (for all bounded measurable test functions $f_i \colon E_i \to \mathbb R$)
For the last one, think: PDFs factorise. Can use Fubini on the product space to prove this because 1 is finite.