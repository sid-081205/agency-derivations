# Appendix: Derivations

**Payoff.**

$$
u_i(a_i, a_j) = \alpha\,\frac{a_i}{a_i + a_j} - c\,\theta\,a_i^{2}
$$

$\alpha>0$: value of edge; $c$: cost of a mistake; $\theta$: accountability.

**Two-option game** ($\alpha=1,\ c=1,\ a\in\{1,\,0.5\}$; payoffs in 24ths).

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

$6>4,\ 10>8 \Rightarrow$ low dominant. Nash $=(10,10)$, the best symmetric cell.

**Continuous equilibrium.**

$$
\frac{\partial u_i}{\partial a_i} = \alpha\,\frac{a_j}{(a_i + a_j)^2} - 2c\theta\,a_i = 0
$$

Symmetry $a_i = a_j = a^{*}$:

$$
\frac{\alpha\,a^{*}}{(2a^{*})^2} = 2c\theta\,a^{*}
\;\Rightarrow\;
\frac{\alpha}{4a^{*}} = 2c\theta\,a^{*}
\;\Rightarrow\;
\alpha = 8c\theta\,(a^{*})^2
$$

$$
a^{*} = \sqrt{\frac{\alpha}{8\,c\,\theta}}
$$

Check: $\theta=\tfrac16 \Rightarrow a^{*}\approx0.87$; $\ \theta=\tfrac13 \Rightarrow a^{*}\approx0.61$.

**Two options with** high $=2L$.

$$
\Delta(a_j) = \alpha\!\left[\frac{2L}{2L + a_j} - \frac{L}{L + a_j}\right] - c\theta\,(4L^2 - L^2)
$$

The bracket $=\tfrac16$ for either opponent choice:

$$
a_j=2L:\ \frac{2L}{4L}-\frac{L}{3L}=\frac12-\frac13=\frac16,
\qquad
a_j=L:\ \frac{2L}{3L}-\frac{L}{2L}=\frac23-\frac12=\frac16
$$

$$
\Delta = \frac{\alpha}{6} - 3c\theta L^{2} = 0
\;\Rightarrow\;
\theta^{*} = \frac{\alpha}{18\,c\,L^{2}}
$$

$\theta<\theta^{*}$: both high; $\ \theta>\theta^{*}$: both restrain.

Check ($\alpha=1,\ c=1,\ L=0.5$): $\ \theta^{*} = \dfrac{1}{18(0.25)} = \dfrac{2}{9} \approx 0.222$; so $\tfrac16<0.222$ gives an arms race and $\tfrac13>0.222$ gives restraint.

**Summary.**

$$
a^{*} = \sqrt{\frac{\alpha}{8c\theta}}, \qquad \theta^{*} = \frac{\alpha}{18cL^{2}}
$$

Both fall in $\theta$: accountability drives restraint. This assumes the contest form $a_i/(a_i+a_j)$; an absolute edge $a_i-a_j$ changes the result.
