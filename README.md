# Surface Rings (S‑rings)

A boundary‑first framework for physics where “difference” and “consensus” across an interface carry the dynamics. The canon is a minimal, symmetry‑driven 2×2 split–skew law on an oriented surface that is causal, passive, and knee‑free by construction (via positive spectral measures). Particle‑like excitations are lossless spectral bands on the surface — surfeons — and their chains build composites.

- Split–skew canon: `Θ = [ Z(ω, K) I + s(K) J ] Ψ`, with `K = √(−Δ_S)`
- Z is Herglotz in `iω` and Stieltjes in `K²` (positive measures); `s(K)` is lossless, orientation‑odd.
- S‑rings (lossless bands in (ω, K)) host surfeons; chains of rings (S‑chains) form composites.
- One kernel, two windows: IR → GR optics/timing; UV (via spectral density) → QED‑like screening.

## Why it’s different

- Two slots, one law: fold boundary traces into “difference” and “consensus”; that’s enough.
- Causality/passivity baked in: thresholds and dispersion are encoded as positive measures, not ad‑hoc knees.
- Direction without dissipation: a single skew term captures handedness and flips under normal reversal.
- Algebraic clarity: per channel, operators form a commutative J‑complex algebra over functions of `K²`.

## Reading order (3 steps)

1) Front‑end (3 pages): narrative + figures
- Research Journal/Surfeon_Frontend.tex → Surfeon_Frontend.pdf

2) Accessible Euclidean track (hands‑on)
- Research Journal/SR_Accessible_Euclidean_Examples.tex → SR_Accessible_Euclidean_Examples.pdf
  - Plane `z=0` (Fourier) and sphere `|r|=R` (spherical harmonics)
  - Photon/scalar across a flat interface
  - Hydrogenic integrals in momentum space
  - Spin‑2 (graviton): TT boundary law → Newton’s 1/r

3) Formal note (proofs + structure)
- Research Journal/SR_Formalization_and_Validations.tex → SR_Formalization_and_Validations.pdf
  - Representation theorem (split–skew inevitability)
  - Herglotz/Stieltjes (positive‑measure) kernels
  - Dirichlet forms and induced geometry
  - Boundary triples / DtN and “edge codes bulk”

Optional: legacy long‑form context
- Research Journal/Surface_Rings_front_paper.tex (older, detailed narrative)

## Validations (among more to be posted)

- GR (IR window): weak‑field lensing/time‑delay (Cassini corridor) constrains the small‑K neighborhood of `Ξ(K) = Re Z(0, K)`.
- Hydrogen overlays: `ΔE_2S→2P = C ∫ Ξ(K) [W_2S − W_2P] dK`, `ΔE_1S = C ∫ Ξ(K) W_1S dK`; same `Ξ`, one `C`; optional UV spectral density for 1S suppression.
- GW backgrounds: S‑ring edge templates for anisotropy fractions; tiny parity‑odd signatures flip under normal reversal (skew `s(K)`).

## Repo layout

- Research Journal/
  - Surfeon_Frontend.tex — 3‑page narrative and figures
  - SR_Accessible_Euclidean_Examples.tex — hands‑on Euclidean track
  - SR_Formalization_and_Validations.tex — formal results and proofs
  - Surface_Rings_front_paper.tex — legacy long‑form front paper
- S‑rings/ (optional) — alternate location for a compiled front‑end draft

## Contributing

Feedback and PRs welcome — especially on:
- Measure‑based recomputation of hydrogen integrals (centroids, 1S scaling)
- Cassini‑tight IR calibrations and GW anisotropy overlays
- Worked examples (Maxwell, elasticity, linearized gravity) in varied geometries

Please open an issue with concise context, the file path(s) you’re targeting, and any proposed equations or figures.

## Cite

“Surface Rings: The Universe of Differences”, H. Salval, v0.1, (2025).

## License

TBD. Until a LICENSE is added, treat the materials as © the author(s) and shared for review and feedback.

