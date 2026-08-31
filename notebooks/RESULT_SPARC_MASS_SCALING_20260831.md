# RESULT — SPARC MASS-SCALING TEST OF THE ADAPTIVE KERNEL
# trontology\notebooks\RESULT_SPARC_MASS_SCALING_20260831.md
# 2026-08-31 afternoon. Status: [UNRATIFIED] — JM stamp required.
# Executes next-action 6 of SESSION_HANDOFF_20260830_TRON_QUANT.md.
# FIREWALL: Tron-side. Data and method are GPRF-facing-safe; the
# candidate (d) framing is not.

## HEADLINE

Candidate (d) as stated — B(x) proportional to a coarse-grained baryon
density, lambda(x) ~ rho^(-alpha/2) with alpha > 0 — CANNOT reproduce
the BTFR mass scaling. The failure is a SIGN failure, not a magnitude
failure, and it is robust across every variant tried.

The magnitude wall (alpha) was a factor-of-100 problem. This is worse:
the required alpha comes out NEGATIVE, which the mechanism forbids.

## DATA AND METHOD

Source: gprf\sparc_galaxy_data\SPARC_Lelli2016c.mrt (Lelli, McGaugh &
Schombert 2016), 175 disk galaxies. Parsed 175/175.
Cuts: Q <= 2, inclination > 30 deg, Vflat > 0, sizes > 0 => 118 galaxies.
M_b = 0.5*L[3.6] + 1.33*M_HI (Upsilon = 0.5 at 3.6um; 1.33 = helium).
r_M = Vflat^2 / a0, a0 = 1.2e-10 m/s^2.
NOTE: SPARC distances assume H0 = 73 km/s/Mpc — the distance-ladder
value, which is the admissible one under cosmology-file 4.1b(ii). No
adjustment needed; dataset and framework agree.

PIPELINE SANITY CHECK (passed): r_M ~ M_b^0.527, scatter 0.120 dex,
R^2 = 0.931. That is BTFR, recovered. The machinery is sound.

## THE MEASUREMENT THAT DOES THE DAMAGE

Galaxy size vs mass, R ~ M_b^beta:

    Rdisk   beta = 0.317   scatter 0.193   R^2 0.65
    Reff    beta = 0.291   scatter 0.199   R^2 0.60
    RHI     beta = 0.343   scatter 0.148   R^2 0.79

Robustness (beta from Rdisk / r_M slope):
    baseline Q<=2 inc>30 ups=0.5   N=118   0.527 / 0.317
    ups = 0.7                      N=118   0.509 / 0.304
    ups = 0.3                      N=118   0.557 / 0.340
    Q == 1 only                    N= 81   0.523 / 0.321
    all Q, inc > 45                N=109   0.539 / 0.329
    M_b > 1e10 only                N= 62   0.554 / 0.428
Stable. beta is ~0.29-0.43, never 0.5.

**RETRACTION.** The 2026-08-30 late-session note (handoff next-action 6)
assumed Freeman's law, beta = 1/2, and concluded alpha ~ 2.0 with a
"three-way convergence" toward coarse smoothing. THAT ASSUMPTION IS
WRONG FOR THIS SAMPLE. Freeman's law holds for bright spirals; SPARC
spans LSBs and dwarfs, and measured central surface density RISES with
mass (rho_surface ~ M_b^+0.365). The convergence was an artifact of the
assumption. Retracted in full. Recorded because it is exactly the kind
of borrowed regularity that must be measured, not assumed.

## THE STRUCTURAL RESULT

alpha(3*beta - 1) = 1 requires beta > 1/3 to have a positive solution.
Measured beta sits AT or BELOW 1/3, i.e. galaxies are close to constant
mean density, which is the degenerate case where the relation has no
solution at all.

Stated without the beta intermediary — how each density measure scales
with M_b, and the alpha that would be needed for lambda ~ rho^(-alpha/2)
to deliver r_M ~ M_b^0.527:

    volume, Rdisk     rho ~ M_b^+0.048   alpha needed = -21.9   IMPOSSIBLE
    volume, Reff      rho ~ M_b^+0.128   alpha needed =  -8.2   IMPOSSIBLE
    volume, RHI       rho ~ M_b^-0.028   alpha needed = +37.5   absurd
    surface, Rdisk    rho ~ M_b^+0.365   alpha needed =  -2.9   IMPOSSIBLE
    surface, RHI      rho ~ M_b^+0.315   alpha needed =  -3.4   IMPOSSIBLE

THE SENTENCE THAT KILLS IT: every baryonic density measure in SPARC is
FLAT or RISING with M_b, while r_M RISES with M_b. A kernel that
SHORTENS lambda where density is high therefore gives massive galaxies
SHORTER lambda exactly where the data demand LONGER. Wrong sign.

alpha < 0 is not available as a rescue: the mechanism is "matter cores
at contiguity saturation are absolute rulers," so more matter means MORE
symmetry breaking, means larger B, means shorter lambda. alpha > 0 is
intrinsic to the story. Reversing it discards the mechanism.

Direct regression confirms: ln(r_M/lambda_c) vs ln(rho/rho_bar) gives
alpha = -0.19 (sphere/Rdisk, R^2 0.014), -0.35 (Reff, R^2 0.055),
-0.07 (RHI, R^2 0.001), -1.18 (disk h=0.3kpc, R^2 0.409). All negative,
essentially no correlation.

## THE ONE ESCAPE ROUTE, TESTED — ALIVE BUT IN POOR HEALTH

Evaluate rho LOCALLY AT r_M on an exponential disk rather than as a
mean. Massive galaxies sit further out in scale lengths (r_M/Rdisk ~
M_b^+0.210, median 1.89), so the exponential can make rho(r_M) FALL with
mass and flip the sign.

    h = 0.2*Rdisk     rho(r_M) ~ M_b^-0.319 (R^2 0.30)  alpha needed +3.30
                      direct fit                        alpha       +1.20 (R^2 0.41)
    h = 0.3 kpc fixed rho(r_M) ~ M_b^-0.002 (R^2 0.00)  alpha needed +481
                      direct fit                        alpha       +0.47 (R^2 0.03)

Verdict: NOT DEAD, NOT HEALTHY.
 - Works only for h proportional to Rdisk. Fixed scale height gives
   nonsense.
 - The two estimators disagree badly (3.30 vs 1.20). That gap is
   regression attenuation and it is a symptom: the relation is not
   tight. They would agree if it were.
 - R^2 ~ 0.3-0.4, scatter 0.35 dex.
 - The entire sign flip is carried by exp(-r_M/Rdisk), which spans 3.9
   DEX across the sample. A 3.9-dex exponential lever arm amplifies
   every error in r_M and Rdisk, and r_M is the quantity being
   predicted — so the construction is close to circular and is fragile
   by inspection.
Not a route to bank. A route to test properly if anyone wants to spend
the time, with the self-consistency (lambda appears on both sides)
solved rather than fitted.

## SCOPE OF THE KILL — STATE THIS CAREFULLY

What died: {adaptive kernel with mean baryon density} AND {C8: lambda =
r_M}, jointly. The test cannot kill either conjunct alone.

C8 is an UNDERIVED CLOSURE CONDITION by canon's own notation law, not an
identity. If lambda is universal (C8.1 lensing fit: ~78 kpc) and r_M
arises some other way, this test does not bind the kernel.

BUT: the adaptive kernel's entire purpose was to supply a microphysical
origin for C8 — "legal pass (iii)" in the 8/30 handoff. A kernel that
cannot deliver the per-galaxy scaling C8 asserts has lost its job. It
was invented for this and it fails at this.

## CONSEQUENCES

1. Wall (alpha) is superseded. Do not spend further effort on
   B ~ rho^alpha magnitude tuning; the exponent cannot be positive.
2. The smoothing-scale derivation (l_s, the standing opening move) is
   DEMOTED. It was to be the make-or-break step for candidate (d). With
   (d) failing on data first, deriving l_s no longer decides anything
   unless the local-rho-at-r_M variant is revived. Cheaper kill landed
   first, exactly as hoped — it just landed on the kill side.
3. Trunk-exam consequence: candidate (d) was the live route to keeping
   an environment-dependent kernel. Its failure pushes the A/B/C fork
   further toward BRANCH C BY ELIMINATION. Flag for the GPRF trunk
   session.
4. Wall (gamma) (chameleon family) is MOOT for the mean-density form.
   An environment-dependent range is not merely awkward to name — it is
   contradicted by the mass scaling.
5. POSITIVE CONTENT, and it points somewhere: the data say r_M is set by
   M_b and a UNIVERSAL acceleration a0, with 0.12 dex scatter and
   R^2 = 0.93 — and NOT by local density (R^2 ~ 0.01-0.06 against every
   density measure). Whatever sets the falloff scale is global and
   universal, not environmental. That is evidence FOR the universal-a0
   picture and therefore for the a0 <-> c*H0 line of attack (handoff
   next-action 7), and evidence AGAINST density-adaptive kernels of any
   kind. The strongest datum in this file is arguably not the kill but
   this.

## REPRODUCIBILITY
Scripts (device-local, session scratch — copy into the repo if wanted):
  ~/sparc_alpha.py    parse, BTFR sanity, beta, direct regression
  ~/sparc_kill.py     robustness table, structural scaling result
  ~/sparc_escape.py   local-rho-at-r_M escape route
All use only numpy. Deterministic; no fitting beyond np.polyfit.

## RATIFICATION
  S1  Mean-density adaptive kernel dies on BTFR mass scaling (sign)
  S2  Retraction of the 2026-08-30 beta=0.5 / alpha~2 convergence
  S3  Local-rho-at-r_M variant: alive, fragile, not banked
  S4  Scope statement: kills (kernel AND C8) jointly, not either alone
  S5  l_s derivation demoted from make-or-break
  S6  Branch C pressure increased — flag to GPRF trunk
  S7  Positive content: falloff scale is global/universal, not local

# END — [UNRATIFIED]
