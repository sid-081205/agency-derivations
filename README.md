# Derivations

**Payoff.**
$$
u_i(a_i, a_j) = \alpha \frac{a_i}{a_i + a_j} - c \theta a_i^{2}
$$
$\alpha>0$: value of edge; $c$: cost of a mistake; $\theta$: accountability.

**Two-option game** ($\alpha=1,\ c=1,\ a\in\{1,\ 0.5\}$; payoffs in 24ths).

For $\theta=\tfrac16$:
$$
u_i(\text{high},\text{low}) = \frac{1}{1.5} - \frac{1}{6}(1)^2 = \frac{16}{24}-\frac{4}{24} = \frac{12}{24}
$$

|            | j: high | j: low  |
|------------|---------|---------|
| **i: high**| (8, 8)  | (12, 7) |
| **i: low** | (7, 12) | (11, 11)|

$8>7,\ 12>11 \Rightarrow$ high dominant. Nash $=(8,8)$, yet $(11,11)$ dominates it — a prisoner's dilemma.

For $\theta=\tfrac13$:
$$
u_i(\text{high},\text{low}) = \frac{2}{3} - \frac{1}{3}(1)^2 = \frac{16}{24}-\frac{8}{24} = \frac{8}{24}
$$

|            | j: high | j: low  |
|------------|---------|---------|
| **i: high**| (4, 4)  | (8, 6)  |
| **i: low** | (6, 8)  | (10, 10)|

$6>4,\ 10>8 \Rightarrow$ low dominant. Nash $=(10,10)$, the best symmetric cell. Raising $\theta$ flips the dominant strategy from high to low.

**Continuous equilibrium.**
$$
\frac{\partial u_i}{\partial a_i} = \alpha \frac{a_j}{(a_i + a_j)^2} - 2c\theta a_i = 0
$$
Symmetry $a_i = a_j = \hat a$:
$$
\frac{\alpha \hat a}{(2\hat a)^2} = 2c\theta \hat a
\quad\Rightarrow\quad
\frac{\alpha}{4\hat a} = 2c\theta \hat a
\quad\Rightarrow\quad
\alpha = 8c\theta \hat a^{2}
$$
$$
\boxed{\ \hat a = \sqrt{\frac{\alpha}{8 c \theta}}\ }
$$
Check: $\theta=\tfrac16 \Rightarrow \hat a\approx0.87$; $\ \theta=\tfrac13 \Rightarrow \hat a\approx0.61$.

**Comparative statics.** Writing $\hat a = (\alpha)^{1/2}(8c\theta)^{-1/2}$,
$$
\frac{\partial \hat a}{\partial \alpha} > 0, \qquad
\frac{\partial \hat a}{\partial c} = -\tfrac12\sqrt{\tfrac{\alpha}{8\theta}}\,c^{-3/2} < 0, \qquad
\frac{\partial \hat a}{\partial \theta} = -\tfrac12\sqrt{\tfrac{\alpha}{8c}}\,\theta^{-3/2} < 0
$$
Autonomy rises in $\alpha$, falls in $c$, falls in $\theta$.

**Improving models ($c\downarrow$).** Since $\hat a \propto c^{-1/2}$, a fall in $c$ raises $\hat a$ — though only as a square root, so the response is dampened, not one-for-one. Taking harm $H$ to be increasing in $\hat a$ ($\partial H/\partial \hat a>0$), falling $c$ pushes $\hat a$ up and $H$ with it; the reliability gain is spent on wider deployment rather than banked as caution.

**Levers.** $\alpha$ is fixed by the competitive environment and $c$ falls on its own; $\theta$ is the term an actor can deliberately raise, with natural ceiling $\theta=1$ (a country bears the full cost of its own mistakes).

---
*This assumes the contest form $a_i/(a_i+a_j)$, under which strategic value is purely positional. An absolute edge $a_i-a_j$ changes the result.*
