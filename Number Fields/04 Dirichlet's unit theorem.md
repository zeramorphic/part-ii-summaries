Define $\ell \colon \mathcal O_L^\star \to \mathbb R^{r+s}$ by
$$\ell(x) = (\log |\sigma_1(x)|, \dots, \log|\sigma_r(x)|, 2\log|\sigma_{r+1}(x)|, \dots, 2\log|\sigma_{r+s}(x)|)$$
- $\mathrm{Im}\,\ell$ is a discrete subgroup of $\mathbb R^{r+s}$.
- $\ker \ell = \boldsymbol\mu_L$ is a finite cyclic group.
- If $L \hookrightarrow \mathbb R$ (i.e. $r > 0$) then $\boldsymbol\mu_L = \{\pm 1\}$.
- $\mathrm{Im}\,\ell$ is contained in the set of $(y_1, \dots, y_{r+s})$ with $y_1 + \dots + y_{r+s} = 0$, so it is discrete in $\mathbb R^{r+s-1}$ (hence is isomorphic to $\mathbb Z^a$ for $a \leq r + s - 1$).

> [!theorem]
> **Dirichlet's unit theorem**. $\mathrm{Im}\,\ell \subseteq \mathbb R^{r+s-1}$ is a lattice.

To prove this, we use:
- If $1 \leq k \leq s$ and $\alpha \in \mathcal O_L \setminus \{0\}$, there exists $\beta \in \mathcal O_L$ with $|N(\beta)| \leq \left(\frac 2\pi\right)^s \sqrt{|D_L|}$ and $b_i < a_i$ for all $i \neq k$, where $\ell(\alpha) = (a_1, \dots, a_{r+s}), \ell(\beta) = (b_1, \dots, b_{r+s})$.
- Fix $k$. Repeatedly apply this result and obtain $\alpha_1, \alpha_2, \dots \in \mathcal O_L$ with bounded norm and strictly decreasing $i$th coordinates for $i \neq k$. Then $(\alpha_t) = (\alpha_{t'})$ for some $t < t'$.
- Let $u_k = \alpha_t \alpha_{t'}^{-1}$, then $\ell(u_k) = \ell(a_t) - \ell(a_{t'})$ so it has negative non-$k$ coordinates and positive $k$th coordinate.
- Perform this for each coordinate. Then $\ell$ of these units are linearly independent, so the rank of $\ell(\mathcal O_L^\star)$ is $r + s - 1$.
- The regulator is $R_L = \operatorname{covol}(\ell(\mathcal O_L^\star))$ where $\ell(\mathcal O_L^\star)$ is treated as a lattice in $\mathbb R^{r+s-1}$.