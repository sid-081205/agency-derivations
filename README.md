# Derivations

## 1. Payoff function

$$U_i(a_i, a_j) = \alpha \frac{a_i}{a_i + a_j} - \theta c \, a_i^2$$

Share of prize minus expected failure cost.

## 2. Values chosen for the 2×2

$$\alpha = 1, \qquad c = 1, \qquad a_H = 1, \qquad a_L = \tfrac{1}{2}$$

Two regimes: $\theta = 1/6$ and $\theta = 1/3$.

## 3. Shares

Equal choices:

$$\frac{a_i}{a_i+a_j} = \frac{1}{2} = \frac{12}{24}$$

High against low:

$$\frac{1}{1+\tfrac{1}{2}} = \frac{2}{3} = \frac{16}{24}, \qquad \frac{\tfrac{1}{2}}{1+\tfrac{1}{2}} = \frac{1}{3} = \frac{8}{24}$$

## 4. Costs

Cost is quadratic and $a_L = a_H/2$, so low costs one quarter of high:

$$\theta c\, a_H^2 = \theta, \qquad \theta c\, a_L^2 = \frac{\theta}{4}$$

| | $\theta = 1/6$ | $\theta = 1/3$ |
|---|---|---|
| cost of high | 4/24 | 8/24 |
| cost of low | 1/24 | 2/24 |

## 5. Cells (share − cost)

For $\theta = 1/6$:

$$(L,L): \tfrac{12}{24} - \tfrac{1}{24} = \tfrac{11}{24} \text{ each}$$

$$(H,H): \tfrac{12}{24} - \tfrac{4}{24} = \tfrac{8}{24} \text{ each}$$

$$(H,L): i = \tfrac{16}{24} - \tfrac{4}{24} = \tfrac{12}{24}, \quad j = \tfrac{8}{24} - \tfrac{1}{24} = \tfrac{7}{24}$$

For $\theta = 1/3$:

$$(L,L): \tfrac{12}{24} - \tfrac{2}{24} = \tfrac{10}{24} \text{ each}$$

$$(H,H): \tfrac{12}{24} - \tfrac{8}{24} = \tfrac{4}{24} \text{ each}$$

$$(H,L): i = \tfrac{16}{24} - \tfrac{8}{24} = \tfrac{8}{24}, \quad j = \tfrac{8}{24} - \tfrac{2}{24} = \tfrac{6}{24}$$

## 6. Matrices

$\theta = 1/6$:

| | j: low | j: high |
|---|---|---|
| **i: low** | 11/24, 11/24 | 7/24, 12/24 |
| **i: high** | 12/24, 7/24 | **8/24, 8/24** (Nash) |

$\theta = 1/3$:

| | j: low | j: high |
|---|---|---|
| **i: low** | **10/24, 10/24** (Nash) | 6/24, 8/24 |
| **i: high** | 8/24, 6/24 | 4/24, 4/24 |

## 7. Dominance

Gain to $i$ from switching low → high.

If $j$ plays low:

$$\left( \tfrac{2}{3} - \theta \right) - \left( \tfrac{1}{2} - \tfrac{\theta}{4} \right) = \tfrac{1}{6} - \tfrac{3\theta}{4}$$

If $j$ plays high:

$$\left( \tfrac{1}{2} - \theta \right) - \left( \tfrac{1}{3} - \tfrac{\theta}{4} \right) = \tfrac{1}{6} - \tfrac{3\theta}{4}$$

Same in both columns, so one strategy is always strictly dominant and no mixed equilibrium exists.

## 8. Threshold

Setting the gain to zero:

$$\tfrac{1}{6} - \tfrac{3\theta}{4} = 0 \quad \Longrightarrow \quad \theta = \tfrac{2}{9}$$

$$\theta < \tfrac{2}{9}: \quad \text{high dominant, Nash} = (H,H)$$

$$\theta > \tfrac{2}{9}: \quad \text{low dominant, Nash} = (L,L)$$

Check: $1/6 < 2/9 < 1/3$.

## 9. General form

Restoring $\alpha$, $c$, $a_H$ with $a_L = a_H/2$, the race condition is

$$\frac{\theta c\, a_H^2}{\alpha} < \frac{2}{9}$$

No capability term appears.

## 10. Note

The fractions depend on $a_H = 2a_L$. Any other ratio shifts the numbers but a threshold $\theta$ still exists, which is all the argument needs.
