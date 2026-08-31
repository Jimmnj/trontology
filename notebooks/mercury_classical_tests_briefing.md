# MERCURY / CLASSICAL-TESTS BRIEFING FOR EXTERNAL AI (tron lane)
# 2026-08-26. Drafted by Claude at JM's request. [UNRATIFIED]
# LANE: trontology / substrate mechanics. NOT GPRF.
# GPRF claims NOTHING here (see F3 in GPRF_SPEC_FOR_EXTERNAL_AI.md:
# GR already owns 43"/cy; GPRF's required contribution is zero).

## 0. THE ASSIGNMENT
Can substrate mechanics derive the classical solar-system tests
from mechanism, without tuning to the answers?

## 1. THE TARGET TERM (perihelion)
The perturbing potential per unit mass that reproduces GR is

    delta_Phi = - G M L^2 / (c^2 r^3)

Equivalently, since L/r = v_perp:

    delta_Phi = - (GM/r) * (v_perp/c)^2

FOUR LOCKS, all must be hit:
  L1. Form: 1/r^3.
  L2. Scaling: coefficient carries L^2 (= GM a(1-e^2)).
  L3. Magnitude: 1/c^2.
  L4. Coefficient: exactly 1. (1/2 -> 21"/cy; 3/2 -> 65"/cy.)

## 2. WHY L2 IS NON-NEGOTIABLE (verified computation)
A STATIC 1/r^3 potential has a constant coefficient, so its
precession scales as 1/[a(1-e^2)]^2, while GR's scales as
1/[a(1-e^2)]. Fit at Mercury and the rest fail:

  planet   GR("/cy)  static-1/r^3 fraction   shortfall
  Mercury   42.998        1.000 (fitted)         --
  Venus      8.626        0.513              4.2 "/cy
  Earth      3.840        0.371              2.4 "/cy
  Mars       1.351        0.245              1.0 "/cy

Against EPM2011 residual budgets (Pitjev & Pitjeva 2013, Table 5:
Venus 1.6, Earth 0.19, Mars 0.037 mas/cy) these are excluded by
~2.6e3, ~1.3e4, ~2.7e4 respectively.

CONSEQUENCE (structural, not numerical): NO STATIC MASS/DENSITY
DISTRIBUTION CAN PRODUCE THE TERM. A static source knows position,
not the orbiting body's angular momentum. Any rho(r) whatsoever
lands in the table above. The mechanism must be VELOCITY-
DEPENDENT.

## 3. THE OPTICAL-MEDIUM FORM AND ITS SPLIT
The medium/refractive-index formulation (Eddington; Schwarzschild
in isotropic coordinates) uses

    n(x) = 1 + 2 delta_Phi / c^2      [delta_Phi = GM/r > 0]

VERIFIED against observation:
  - Light deflection at solar limb: alpha = 4GM/(b c^2)
    = 1.7516 arcsec.  [GR/observed 1.75]  PASS
  - Shapiro delay, Earth-Venus grazing superior conjunction:
    one-way 116 us, round trip 233 us.  [observed ~200 us
    order] PASS
  - Gravitational redshift: FAILS if you use this index.
    Coefficient 2 gives 4.25e-6 at the solar surface; observed
    is 2.12e-6 = GM/(R c^2), i.e. COEFFICIENT 1.

WHY: redshift is not a propagation effect. A static medium does
not change frequency. Redshift is a clock-rate comparison and
reads the TEMPORAL part alone: delta_nu/nu = delta_Phi/c^2.

THE DECOMPOSITION (the key structural fact):
The 2 in the index is 1 (temporal, g_00) + 1 (spatial, g_ij).

  observable            reads                coefficient
  ---------------------------------------------------------
  gravitational redshift  temporal only          1
  light deflection        temporal + spatial     2
  Shapiro delay           temporal + spatial     2
  perihelion precession   spatial (via L^2)      1

The four classical observables are FOUR PROJECTIONS OF TWO
COEFFICIENTS. They are not four independent targets.

## 4. THE ACCEPTANCE TEST
The substrate must produce THE SPLIT: a temporal response
(clock-rate law) and a spatial response, each at coefficient 1,
from one set of assumptions with NO RE-TUNING BETWEEN THEM.
Get the split and all four observables follow.

KNOWN FAILURE MODE: a medium that only slows clocks (temporal
only) gives redshift correctly, deflection at HALF (0.87"), and
perihelion precession wrong. This is the scalar-theory graveyard,
and it is the default trap for a "refractive ether" picture,
because refraction reads as a propagation story while the clock
law is a separate ingredient.

## 4b. SU'S STATUS (verified 2026-08-26 from primary sources)
Read: Su 2001 (Eur. Phys. J. B 24, 231) [clock law]; Su 2001
light-deflection paper [propagation]; Su 2008 Quantum
Electromagnetics Ch.5 [gravity sector].

  observable            status in Su's framework
  ------------------------------------------------------------
  gravitational redshift  DERIVED, coefficient 1. Perturbation
                          on bounded matter wave; Eq.(25):
                          f = f0(1 - Phi_g/c^2 - v^2/2c^2).
                          Shift is at the SOURCE (transition
                          frequency), not in propagation.
  light deflection        Index POSTULATED. Su's own words:
                          "it is postulated", "proposed as".
                          n_g = 1 + 2*Phi_g/c^2, giving c/n_g.
                          Yields GR's 1.75" — his conclusion:
                          "agrees with that predicted from the
                          general relativity."
  Shapiro / radar echo    Same postulate, GR's values.
  perihelion precession   NOT ATTEMPTED. Ch.5 [T1]: the term
                          "is of the second order and could be
                          accounted for IF the gravitational
                          refinement of the wave equation is
                          extended from the present first order
                          to the second order." Not done.
                          Evolution eq. (5.9) explicitly
                          discards the higher-order terms.

STRUCTURAL VERDICT: n_g = 1 + 2 Phi_g/c^2 IS Eddington's
weak-field GR index in isotropic coordinates. Su imports GR's
weak-field metric as a postulate about a medium. Therefore
Su == weak-field GR for all propagation observables, BY
CONSTRUCTION — same numbers, different ontology, no new
empirical ground in the photon sector. His distinctive content
is the FRAME structure (ECI, local-ether hierarchy) and the
source-side quantum account of redshift.

SU'S OWN NAMED FALSIFIER (live, and in the derived sector):
Because his redshift arises from bound-state quantum energy
rather than a clock rate, he predicts the shift is TRANSITION-
DEPENDENT ("where the wavefunctions of the two involved quantum
states have different spatial distributions, the dependence of
the frequency shift on gravity is expected to be of a more
complicated form"), plus stellar spectra depending on stellar
mass. He offers this as "a means to test the local-ether wave
equation." This is a predicted VIOLATION OF THE UNIVERSALITY OF
GRAVITATIONAL REDSHIFT — exactly what null-redshift experiments
bound (different clock species vs annual solar-potential
variation). CHECK THOSE BOUNDS. This is the honest place to
test Su, because it is where his theory derives rather than
postulates.

INTERNAL TENSION TO RESOLVE: Ch.6 derives UNIVERSALITY in the
velocity sector (whole spectrum scales by one common factor,
species-blind); Ch.5 predicts NON-UNIVERSALITY in the
gravitational sector. No argument for the asymmetry is given
in the text as read. [T3 — Claude's reading, verify.]

## 5. THE GERBER CRITERION (honesty check)
Gerber (1898) produced a velocity-dependent potential giving
exactly 43"/cy, decades before GR, from a derivation later judged
unjustified. His light-deflection prediction was inconsistent with
observation (factor commonly quoted as 3/2 -- VERIFY BEFORE
CITING; Claude's recollection, not sourced).

Therefore: Mercury alone proves nothing. A single number can be
hit by construction. The question to answer is:

  Does the substrate mechanism produce the L^2/c^2 term AND
  1.75" AND the Shapiro delay AND the coefficient-1 redshift,
  from the same assumptions, with nothing adjusted between them?

If yes: a real result in the tron lane.
If it can only do Mercury: it is Gerber again, and knowing that
early saves months.

## 6. WHERE 1/c^2 MAY LEGITIMATELY ENTER
Two physically motivated (non-fitted) routes, both historical:
  (i) RETARDATION: finite propagation speed means the source's
      influence arrives lagged, generating v/c and (v/c)^2 terms.
      [Gerber's route -- delivers velocity dependence naturally,
      but historically fails the deflection test.]
  (ii) FIELD-ENERGY SELF-GRAVITATION: the field's own energy
      density gravitates; nonlinear correction of relative order
      Phi/c^2. [Closer to Beckmann's route.]
Either can in principle supply (v_perp/c)^2. The burden is to
show the mechanism is independently motivated, not reverse-
engineered onto 43.

## 7. INSTRUCTIONS TO THE EXTERNAL AI
- Do not fit. Derive, then compare.
- Report the coefficient you obtain, including its sign and any
  numerical prefactor, BEFORE comparing to 43"/cy.
- Run the full four-observable table. A Mercury-only success is
  reported as a FAILURE of the acceptance test.
- If a step requires an assumption, name it and state whether it
  is independently motivated or introduced to reach the target.
- Report conflicts to JM verbatim; do not resolve them by
  adjusting the framework.
# END
