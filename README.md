# Andrews–Curtis: Lean-certified AC-classes in the SAIR ACC unsolved pool

Lean 4 / Mathlib contribution to the [SAIR ACC Challenge](https://competition.sair.foundation/competitions/acc) Proof Track.
Extracted from [yachi/lean-playground](https://github.com/yachi/lean-playground) (`LeanPlayground/AndrewsCurtis/`, commit 8b0a9173227433ddd9f13dd9934328cdd4028852).

Everything is stated against the official `AC.lean`, which is copied verbatim into `AndrewsCurtisLean/Defs.lean` (Apache-2.0, from SAIRcompetition/Andrews-Curtis at a0fd6e6f52d82c93ccc06ab91d81e8fa3678256e). The only axioms used are propext, Quot.sound and Classical.choice. There is no `sorry` and no `native_decide`.

| File | Content |
|---|---|
| `Checker.lean` | Sound checker for the rank-2 move table `ac-r2-v1`; `AC.Reachable.symm`; relator swap (`reachable_swap`) |
| `Symmetry.lean` | `AC.Reachable.map` (free-group endomorphisms); triviality invariant under signed generator permutations |
| `AK3Class.lean` | 47 unsolved pool presentations are AC-trivial iff AK(3) is (`triv_iff_AK3`) |
| `PoolClasses.lean` | 731 unsolved pool presentations in 228 certified classes (`poolClasses_triv_iff`) |

Build: `lake exe cache get && lake build` (Lean v4.35.0, Mathlib v4.35.0). Search code and data: `scripts/`.

Search code and Lean formalization written with AI assistance (Claude Code, Anthropic).
