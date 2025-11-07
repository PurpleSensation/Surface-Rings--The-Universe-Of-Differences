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

---

## A longer introduction

Surface Rings (S‑rings) are a boundary‑first way to describe physics. Instead of beginning with a bulk PDE and then adding boundary conditions, we start on the oriented surface \`S\` itself and fold every field’s boundary traces into two natural slots:

- the “difference” across \`S\` (jump), and
- the “consensus” (average).

The law relating value and flux on \`S\` is forced—under standard assumptions of causality, passivity, and surface isotropy—to have exactly two pieces:

1) a causal/passive “persistence” operator that acts identically on both slots; and
2) a lossless, orientation‑odd “handed rotation” that couples the slots.

That’s the split–skew canon. Its consequences are surprisingly rich: in the joint frequency–tangential‑wavenumber plane \`(ω, K)\`, the lossless sets organize into spectral bands (rings). Quantizing a mode on a ring yields a particle‑like boundary excitation—a surfeon. Chains of rings give composites, and familiar observables (GR optics/timing in the IR, hydrogenic momentum integrals in the UV) arise as linear functionals of the same static kernel \`Ξ(K) = Re Z(0, K)\`. The upshot: surface physics, done right, carries direction, energy, and even geometry—without presupposing a bulk metric or adding ad‑hoc spectral “knees”.

## Derivation and analysis (sketch)

Let \`(q, p)\` be power‑conjugate boundary variables with instantaneous power \`⟨p, ẋ⟩_S\`. Fold traces across \`S\`:

- \`Ψ = ([q], {q})ᵀ\`, \`Θ = ([p], {p})ᵀ\`, with \`[·]\` the jump and \`{·}\` the average.
- Tangential dispersion is governed by \`K := √(−Δ_S)\` (plane → tangential Fourier magnitude; sphere → \`κ_ℓ = √(ℓ(ℓ+1))/R\`).

Under causality (convolution in \`t\`, analytic in \`iω\`), passivity (nonnegative time‑integrated power), tangential stationarity and local isotropy (no preferred point/direction on \`S\` after polarization), one proves the representation theorem:

```
Θ(ω) = [ Z(ω, K) I + s(K) J ] Ψ(ω),   J = [[0, 1], [-1, 0]]
```

with these properties:

- \`Z(ω, K)\` is Herglotz in \`iω\` and Stieltjes (complete Bernstein) in \`K²\`: it admits positive spectral measures in both variables. This is the mathematical expression of causality + passivity. Thresholds and dispersion arise as positive measures—not as heuristic knees.
- \`s(K)\` is real, lossless, and orientation‑odd: flipping the normal flips \`s\`. It is the unique anti‑Hermitian direction consistent with the boundary power pairing.

Further structure follows immediately:

- J‑complex algebra: per polarization channel, \`a(K) I + b(K) J\` composes like complex numbers with \`J² = −I\`; operators form a commutative \`*\`‑algebra over functions of \`K²\`.
- Automodes/rings: lossless bands are precisely where \`ker Re Z(ω, K) ≠ {0}\`. Under isotropy, these loci organize as closed rings in \`(ω, K)\`.
- Edge codes bulk: integrating out a passive/causal bulk (Schur complement/Dirichlet‑to‑Neumann) produces the same split–skew form. The canon lives on the boundary, regardless of how you factor edge vs. bulk.
- Induced geometry: the energy form \`⟨f, Ξ(K) f⟩\` (with \`Ξ = Re Z(0, K)\`) is a regular Dirichlet form; its high‑\`K\` asymptotics encode spectral dimension (dimensional flow) via standard subordination.

## Euclidean faces (how to compute)

- Plane \`z=0\`: Fourier along \`x, y\`; the scalar DtN symbol is \`γ(K) = √(k₀² + K²)\`. EM admittances (TE/TM) are Herglotz/Stieltjes in \`K²\`. Optional magnetoelectric skew adds a tiny \`s(K)\).
- Sphere \`|r|=R\`: diagonalize in \`Y_{ℓm}\`; \`K\` eigenvalues are \`κ_ℓ\`. Any kernel \`Z(ω, K)\` acts as \`Z(ω, κ_ℓ)\` on each \`(ℓ, m)\).

Hydrogenic momentum‑space integrals use spherical‑Bessel transforms of radial wavefunctions to produce weights \`W_{nℓ}(K)\`. Leading shifts are linear in \`Ξ(K)\`:

```
ΔE_2S→2P = C ∫ Ξ(K) [ W_2S(K) − W_2P(K) ] dK
ΔE_1S      = C ∫ Ξ(K) W_1S(K) dK
```

One constant \`C\` fixes a centroid (e.g., FOSOF 2S→2P). If 1S needs UV suppression, add a positive spectral density with a Compton‑scale threshold in the Stieltjes representation of \`Ξ\`—no change to IR constants or GR fits.

## Particles and the spin‑2 sector

- Surfeons: quantized modes on S‑ring bands; S‑chains (graphs of rings) give composites. Light chains (lepton‑like), photon‑like EM modes, heavy cores (proton‑like) follow from simple ring couplings.
- Graviton (spin‑2 surfeon): in TT gauge the boundary law is
  \`[K_ab − K γ_ab]^TT = 8πG ( Y^(2)(ω, K) I + s^(2)(K) J ) h^TT\`, with \`Y^(2) ∝ Ξ(K)\` at small \`K\`. Quantizing the TT edge field on a lossless band gives \`+, ×\` graviton modes; a tiny \`s^(2)(K)\` flips under normal reversal.
- Newton’s 1/r: the static propagator induced by \`Ξ\` is \`∫ d³q e^{iq·r}/q² = 1/(4πr)\`; normalize with Cassini/Shapiro to recover \`V(r) = −GM/r\`. Cassini’s \`γ\`‑corridor constrains how flat \`Ξ\` must be near \`K=0\`.

## Discussion and positioning

- Boundary‑first vs. boundary conditions: the canon is the constitutive law \emph{on} \`S\`, not an afterthought to a bulk PDE. It captures causality/passivity and direction at the boundary, then lets you glue to any compatible bulk.
- No ad‑hoc knees: thresholds, onsets, and screening are built from positive measures (Herglotz/Stieltjes). This keeps causal structure intact across domains.
- Algebraic clarity: the J‑complex split makes power accounting and chirality explicit, while passivity narrows the admissible set to a convex cone.
- Where it lands: closest neighbors are Dirichlet‑to‑Neumann/Calderón methods, port‑Hamiltonian/positive‑real systems, and impedance/scattering networks.

Limitations and open items:

- Measure identification: selecting spectral measures from data is an inverse problem—solvable, but it needs discipline (priors, convexity, cross‑domain constraints).
- Gauge/diffeo handling: EM and spin‑2 examples must remain explicitly gauge‑aware (done in the formal note, highlighted in the accessible track).
- Numerics: knee‑based legacy overlays are being replaced with measure‑based recomputations; results will be swapped in as they converge.

## Roadmap

- Finalize measure‑based recomputation of hydrogen integrals (centroids + 1S) and GR IR calibrations.
- Publish edge anisotropy templates and parity‑odd diagnostics for GW datasets (LVK/PTA).
- Package a minimal library: DtN kernels → split–skew form; positive‑measure fitting; Euclidean plane/sphere helpers.
- Worked examples beyond scalars/EM: elasticity, acoustics, and spin‑2 in curved backgrounds.
