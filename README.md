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

**Total harm.** Autonomy is exposure to mistakes, each costing c; summing both symmetric countries,
    H = c·â_i + c·â_j = 2c·â
Substituting â = √( α / 8cθ ):
    H = 2c · √( α / 8cθ ) = √( 4c²·α / 8cθ ) = √( αc / 2θ )
    ┌─────────────────────┐
    │  H = √( αc / 2θ )    │
    └─────────────────────┘

**Comparative statics of harm.** Writing H = α^(1/2) · c^(1/2) · (2θ)^(−1/2),
    ∂H/∂α > 0,    ∂H/∂c > 0,    ∂H/∂θ < 0
Harm rises in α, rises in c, falls in θ. Note H ∝ c^(1/2): a fall in c lowers harm only as a square root (halving c cuts H by ≈ 29%, not 50%), because â ∝ c^(−1/2) rebounds upward and spends most of the reliability gain on wider deployment — a Peltzman offset ([Peltzman 1975](https://doi.org/10.1086/260352)).

**Direction of c is not fixed.** Model changes can push c either way: better calibration and tighter guardrails lower it; but greater capability invites autonomy over higher-stakes decisions, raising the damage per mistake. The likelier pull is c ↑. Then H ↑ too — so c is at best a weak ally (√c), at worst adverse, and never a control variable (set by technology, not policy). Likewise α is set by the adversary.

**Only θ is a lever.** θ enters H^(−1/2) and cannot be arbitraged back: it raises the *price* of autonomy, not its safety, so deployment falls rather than expands. Harm-minimising choice is the ceiling
    ┌─────────────┐
    │  θ* = 1     │
    └─────────────┘
θ = 1 ⇒ private cost = social cost (full internalisation); θ > 1 is impossible (no actor is more than fully responsible). The game-theoretic optimum coincides with the moral one.

---
*This assumes the contest form a_i/(a_i + a_j), under which strategic value is purely positional. An absolute edge a_i − a_j changes the result. H is taken linear in deployment (H = c·â); if harm tracks the convex cost term (H ∝ c·â³ ⇒ H ∝ c^(−1/2)), a falling c raises H outright. Under either form: ∂H/∂θ < 0 and θ* = 1.*
