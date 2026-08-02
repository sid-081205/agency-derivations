# Derivations for my piece on (agency)[https://sid081205.substack.com/p/agentic-agency-and-games]

**Payoff.**

$$u_i(a_i, a_j) = \alpha \cdot \frac{a_i}{a_i + a_j} - c\,\theta\, a_i^2$$

$\alpha$: value of edge; $c$: cost of a mistake; $\theta$: accountability.

**Two-option game** ($\alpha = 1$, $c = 1$, $a \in \{1, 0.5\}$; payoffs in 24ths).

For $\theta = 1/6$:

$$u_i(\text{high}, \text{low}) = \frac{1}{1.5} - \frac{1}{6}(1)^2 = \frac{12}{24}$$

|             | j: high | j: low   |
|-------------|---------|----------|
| **i: high** | (8, 8)  | (12, 7)  |
| **i: low**  | (7, 12) | (11, 11) |

High dominant. Nash $= (8, 8)$, yet $(11, 11)$ dominates it: a prisoner's dilemma.

For $\theta = 1/3$:

$$u_i(\text{high}, \text{low}) = \frac{2}{3} - \frac{1}{3}(1)^2 = \frac{8}{24}$$

|             | j: high | j: low   |
|-------------|---------|----------|
| **i: high** | (4, 4)  | (8, 6)   |
| **i: low**  | (6, 8)  | (10, 10) |

Low dominant. Nash $= (10, 10)$. Raising $\theta$ flips the dominant strategy from high to low.

**Continuous equilibrium.**

$$\frac{\partial u_i}{\partial a_i} = \alpha \cdot \frac{a_j}{(a_i + a_j)^2} - 2c\,\theta\, a_i = 0$$

Symmetry $a_i = a_j = \hat{a}$:

$$\alpha = 8c\,\theta\,\hat{a}^2 \quad\Rightarrow\quad \boxed{\;\hat{a} = \sqrt{\dfrac{\alpha}{8c\theta}}\;}$$

Check: $\theta = 1/6 \Rightarrow \hat{a} \approx 0.87$; $\theta = 1/3 \Rightarrow \hat{a} \approx 0.61$.

**Comparative statics.** With $\hat{a} = \alpha^{1/2}(8c\theta)^{-1/2}$:

$$\frac{\partial \hat{a}}{\partial \alpha} > 0, \qquad \frac{\partial \hat{a}}{\partial c} < 0, \qquad \frac{\partial \hat{a}}{\partial \theta} < 0$$

Autonomy rises in $\alpha$, falls in $c$ and $\theta$.

**Total harm.** Autonomy is exposure to mistakes, each costing $c$. Summing both countries:

$$H = 2c\,\hat{a} = 2c\sqrt{\frac{\alpha}{8c\theta}} = \boxed{\;\sqrt{\dfrac{\alpha c}{2\theta}}\;}$$

**Statics of harm.** With $H = \alpha^{1/2}c^{1/2}(2\theta)^{-1/2}$:

$$\frac{\partial H}{\partial \alpha} > 0, \qquad \frac{\partial H}{\partial c} > 0, \qquad \frac{\partial H}{\partial \theta} < 0$$

Since $H \propto c^{1/2}$, halving $c$ cuts $H$ by only $\approx 29\%$. The reliability gain rebounds into wider deployment ($\hat{a} \propto c^{-1/2}$): a Peltzman offset ([Peltzman 1975](https://doi.org/10.1086/260352)).

**Direction of $c$ is unfixed.** Better calibration lowers $c$; greater capability invites autonomy over higher-stakes decisions, raising it. The likelier pull is $c \uparrow$, so $H \uparrow$. Either way $c$ is at best weak, at worst adverse, and never a control variable (set by technology). Likewise $\alpha$ is set by the adversary.

**Only $\theta$ is a lever.** It enters as $\theta^{-1/2}$ and cannot be arbitraged back: it raises the *price* of autonomy, not its safety, so deployment falls.

$$\boxed{\;\theta^* = 1\;}$$

At $\theta = 1$, private cost $=$ social cost. $\theta > 1$ is impossible. The game-theoretic optimum meets the moral one.

