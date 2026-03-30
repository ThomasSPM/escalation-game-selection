# escalation-game-selection
Lean 4 / Mathlib formalization of "Escalation by Game Selection" (Pitz &amp; Gardian). Verifies brinkmanship thresholds, transformation operators, and equilibrium results for 2×2 symmetric games. Compatible with Aristotle (harmonic.fun).

# escalation-game-selection

Lean 4 / Mathlib formalization of the theorems in:

> Thomas Pitz & Wolf Gardian: *Escalation by Game Selection:  
> A Meta-Game Theory of De-escalation via Game Transformations* (2026)  
> SSRN: [link einfügen nach Upload]

## What is verified

| Result | Description |
|--------|-------------|
| Prop. 3.1 | Existence of pure-strategy Bayesian Nash equilibria |
| Thm. 3.2  | Resistance threshold p̄ characterizes equilibrium switch |
| Prop. 3.3 | Mixed-strategy equilibrium under Bayesian Chicken |
| Prop. 4.1 | T₁ eliminates capitulation |
| Thm. 4.2  | U_{c,b} induces Peace dominance |
| Prop. 4.3 | T₄ creates fight-coordination risk (overshoot hazard) |
| Prop. 4.5–Thm. 4.6 | Two-stage de-escalation path and restoration |

## Quick Start (Aristotle)

1. Go to [aristotle.harmonic.fun](https://aristotle.harmonic.fun/dashboard/)
2. Select **"Fill Sorries in a Lean file"**
3. Upload proofs individually (one theorem per session works most reliably)
4. Wait ~10–30 min per proof for completion

> **Note:** Although uploading the full `GameSelection.lean` at once is possible in principle,
> uploading individual theorems separately has proven more reliable in practice.

## Local Setup
```bash
# Requires Lean 4 and Mathlib
lake build
```

Dependencies: Lean 4.24.0, Mathlib (commit `f897ebc`)

## License

MIT — see companion paper on SSRN for full theoretical context.
