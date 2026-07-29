# Derivations

**Payoff.**

    u_i(a_i, a_j) = α · a_i/(a_i + a_j) − c·θ·a_i²

α > 0: value of edge; c: cost of a mistake; θ: accountability.

**Two-option game** (α = 1, c = 1, a ∈ {1, 0.5}; payoffs in 24ths).

For θ = 1/6:

    u_i(high, low) = 1/1.5 − (1/6)(1)² = 16/24 − 4/24 = 12/24

|             | j: high | j: low   |
|-------------|---------|----------|
| **i: high** | (8, 8)  | (12, 7)  |
| **i: low**  | (7, 12) | (11, 11) |

8 > 7 and 12 > 11 ⇒ high dominant. Nash = (8, 8), yet (11, 11) dominates it — a prisoner's dilemma.

For θ = 1/3:

    u_i(high, low) = 2/3 − (1/3)(1)² = 16/24 − 8/24 = 8/24

|             | j: high | j: low   |
|-------------|---------|----------|
| **i: high** | (4, 4)  | (8, 6)   |
| **i: low**  | (6, 8)  | (10, 10) |

6 > 4 and 10 > 8 ⇒ low dominant. Nash = (10, 10), the best symmetric cell. Raising θ flips the dominant strategy from high to low.

**Continuous equilibrium.**

    ∂u_i/∂a_i = α · a_j/(a_i + a_j)² − 2c·θ·a_i = 0

Symmetry a_i = a_j = â:

    α·â / (2â)² = 2c·θ·â   ⇒   α/(4â) = 2c·θ·â   ⇒   α = 8c·θ·â²

    ┌─────────────────────┐
    │  â = √( α / 8cθ )    │
    └─────────────────────┘

Check: θ = 1/6 ⇒ â ≈ 0.87;  θ = 1/3 ⇒ â ≈ 0.61.

**Comparative statics.** Writing â = α^(1/2) · (8cθ)^(−1/2),

    ∂â/∂α > 0,    ∂â/∂c < 0,    ∂â/∂θ < 0

Autonomy rises in α, falls in c, falls in θ.

**Improving models (c falls).** Since â ∝ c^(−1/2), a fall in c raises â — though only as a square root, so the response is dampened, not one-for-one. Taking harm H to be increasing in â (∂H/∂â > 0), falling c pushes â up and H with it; the reliability gain is spent on wider deployment rather than banked as caution.

**Levers.** α is fixed by the competitive environment and c falls on its own; θ is the term an actor can deliberately raise, with natural ceiling θ = 1 (a country bears the full cost of its own mistakes).

---
*This assumes the contest form a_i/(a_i + a_j), under which strategic value is purely positional. An absolute edge a_i − a_j changes the result.*
