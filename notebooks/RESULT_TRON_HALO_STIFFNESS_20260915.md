# RESULT — THE 10^10: WHAT THE HALO DATA REQUIRE OF THE TRON POSTULATE
# trontology\notebooks\RESULT_TRON_HALO_STIFFNESS_20260915.md
# 2026-09-15. Status: [UNRATIFIED]. T2 unless marked. Tron-side.
# Origin: GPRF session of 2026-09-08..15 that rejected the Yukawa
# exterior (gprf\notebooks\RESULT_BRANCHA_SPARC_POPULATION_20260915.md)
# and established the empirical target profile. This file carries the
# TARGET across the firewall and asks what the seven axioms must supply.
# Source for the axioms: "The Tron Theory: A novel concept for the
# Aether and Matter" (R. & J. Marsen), OneDrive\Physics\Share\Marsen.

## 0. THE TARGET (from GPRF-side data; T1/T2 references in the GPRF file)
A real, positive, non-baryonic density rho_nb(r) around a galaxy of
baryonic mass M_b that:
  (1) goes as r^-2 from a few kpc to >= 300 kpc (SPARC: Bariego-Quintana
      & Llanes-Estrada 2026; lensing: Meduri & Desai 2026, pseudo-
      isothermal preferred over NFW and Burkert in all four mass bins);
  (2) has a core R_c ~ 5-7 kpc, nearly independent of M_b (Meduri);
  (3) has deep-regime amplitude rho_nb = sqrt(a0 G M_b)/(4 pi G r^2),
      i.e. v_flat^4 = a0 G M_b with universal a0 (BTFR);
  (4) is real mass co-located with galaxies (Bullet: Cha+2025 ICL
      tracing; Famaey 2026 residual mass at galaxy peaks);
  (5) merges into the ambient value where the galaxy's influence ends
      (environmental edge, ~1 Mpc for isolated galaxies);
  (6) [set aside for now, JM 2026-09-15] is quiet at solar-system scale.
JM's standing rule (2026-09-15): rho_nb,local may fall BELOW rho_nb,env
but never below zero. Tron count is conserved; trons are variable in
size; higher |potential| -> smaller trons, higher number density.

## 1. WHAT THE AXIOMS ALREADY FIX
Axiom 7 (contiguous everywhere) + conserved count  =>  n = 1/s^3
exactly: number density is a function of tron size alone, and
rho_env = N/V is a global constant. JM's below-ambient-not-below-zero
rule is then bookkeeping on a fixed total. Halos are drawn from
elsewhere; voids sit below ambient.
Axiom 6 (ron transmission speed = c near Earth; LOWER where tron
density is HIGHER) => c is a decreasing function of n. Write
c ~ n^(-alpha) near ambient; alpha unspecified by the axioms.
Axioms 4+5 (attraction ~ 1/outer-radius; size stabilises against
neighbours' boundary rons) => a local mechanical equilibrium. This
IS a pressure balance in different words. The medium is not a gas of
fixed-size particles, but it is not free of hydrostatics either.

## 2. THE MEASUREMENT THAT PINS IT (T1 input)
Gravitational light-speed variation is measured: Shapiro delay and
deflection give delta c / c = 2|phi|/c^2 (PPN gamma=1 to 1e-5). Across
a galactic halo 2|phi|/c^2 ~ 5e-6; at the Sun's surface ~4e-6.
Combine with Axiom 6:
        delta n / n_env = (2|phi|/c^2) / alpha .
So the tron NUMBER-density excess in a galaxy is ~5e-6/alpha.

## 3. THE 10^10
A halo needs rho_nb ~ 1e-22 kg/m^3 at ~10 kpc. Sciama-normalised
rho_env (canon) ~ 1.3e-26 kg/m^3. Required excess: delta rho / rho_env
~ 1e4. Two ways to get it, and they are the SAME number:
  (a) mass per tron fixed, so delta rho/rho = delta n/n:
        alpha = 5e-6 / 1e4 = 5e-10 .
      The medium must be ~10^10 more compliant to gravity than to light.
  (b) alpha ~ 1, so delta n/n ~ 5e-6 (the medium is optically stiff and
      barely compresses), and the halo mass is carried by MASS PER TRON:
        m(s) must rise by ~1e4/5e-6 ~ 2e9-1e10 while s shrinks by one
        part in 1e6.
  (c) a mixture; the product of the two sensitivities is 1e10.
This is the first quantitative demand the halo places on the Tron
Postulate, and it is the same one however it is split. The earlier
"macroscopic fluid" objection (JM, 2026-09-15) was correct that the
FLUID derivation was inappropriate; the number survives because it
now comes from Axiom 6 + a measured PPN quantity, not from an equation
of state.
Check on (a) via mass instead: if delta n/n ~ 5e-6 and mass per tron
is fixed, rho_env would need to be ~2e-17 kg/m^3 for the halo to
gravitate -- ~1 Msun/pc^3, 100x the local dark-matter density
everywhere. Excluded by the Oort limit. So (a) with a Sciama-scale
rho_env is out unless alpha really is ~1e-10; (b) is where the
axioms have room.

## 4. THE TWO UNDEFINED FUNCTIONS
The Postulate as written contains no response law. To become
quantitative it needs exactly two functions:
  F1: tron size as a function of local conditions -- s(phi) or
      s(grad phi) or s(n_neighbours). Axioms 4+5 say there is an
      equilibrium; they do not say what it is.
  F2: gravitating mass per tron as a function of size -- m(s). Axioms
      1-3 say mass sits in a core of compressed rons and size is the
      number of ron layers; they do not say whether rons are conserved
      within a tron or flow between trons.
Then rho_nb = m(s) / s^3 with s from F1, and c(n) from Axiom 6 is a
third constraint on F1 via Sec. 2. The GPRF-side SPARC loop tests any
(F1, F2) pair against 175 galaxies in an evening.

## 5. WHERE THE 10^10 CAN LIVE: RON BORROWING
If rons are conserved WITHIN a tron, m(s) is constant (core gains what
cloud loses) and route (b) is closed; only alpha ~ 1e-10 remains.
If rons FLOW BETWEEN trons (Axiom 6 says they do; Figs. 2-5 of the
paper show ron flux from outer, larger trons to inner, smaller ones),
then a compressed tron can accrete core mass from its neighbours, and
the halo is BORROWED RON MASS CONCENTRATED INTO CORES. Number density
stays within 1e-6 of ambient (so light is barely affected, Sec. 2),
while mass density rises by 1e4. This is the 8/31 conserving-kernel
idea (DRAFT_TRON_SUBSTRATE_CONSERVATION_20260830.md) restated in ron
vocabulary, with the important difference that what is conserved is
RON count, and what is borrowed is ron MASS from a large surrounding
volume into a small central one.
CONSEQUENCE worth checking: if the borrowing volume scales with M_b,
the amplitude can scale non-linearly with M_b even if F1 is linear.
That is the only route seen so far by which a fixed-count medium can
produce v^4 ~ M_b without an explicit a0 in the local law. Not shown.
COST: the outer region is DEPLETED in mass (not in number). A real
depletion shell at hundreds of kpc is a lensing prediction with the
opposite sign to a two-halo term. Mistele/Meduri see no depletion to
300 kpc; so the borrowing volume must be >> 300 kpc, i.e. of order
the environmental edge. Consistent with (5) but not free.

## 6. WHAT THIS DOES NOT DO
- Does not derive a0. The acceleration scale must come out of F1/F2
  or the borrowing geometry; nothing in the seven axioms contains it.
- Does not address (6), by JM's instruction.
- Does not decide alpha. A laboratory or astrophysical bound on
  d(ln c)/d(ln n) for the tronos would settle (a) vs (b); PPN gamma
  gives only the product.

## 7. RATIFICATION
  H1  n = 1/s^3 and rho_env global, from Axiom 7 + conserved count (T2)
  H2  Axiom 6 + PPN gamma pin delta n/n ~ 5e-6/alpha in a galaxy (T2)
  H3  Halo requires delta rho/rho ~ 1e4; the sensitivity product is
      ~1e10 however split between alpha and m(s) (T2)
  H4  Route (a) with Sciama rho_env fails the Oort limit unless
      alpha ~ 1e-10; route (b) = mass-per-tron is where the axioms
      have room (T2/T3)
  H5  Two undefined functions F1, F2 are all that is missing for a
      testable R (T3)
  H6  Ron borrowing between trons is the candidate mechanism for
      route (b); implies an outer depletion shell beyond ~300 kpc (T3)

## 8. WHERE a0 CAN COME FROM (added same session, T2)
The 10^10 of Sec. 3 is NOT a0 (its SI exponent match is units):
  S(r) = c^2 / (8 pi G rho_env r^2) = (L/r)^2 / 6  ~ 3e10 at r = 10 kpc,
with L the length in the Sciama condition Phi_env = -c^2, i.e.
rho_env = 3c^2/(4 pi G L^2). Velocity cancels; S depends on r and
rho_env only.
BUT the acceleration scale the target (Sec. 0, item 3) needs is
available from constants the framework already has:
  a0 ~ c sqrt(G rho_env) = c^2 sqrt(3/4pi) / L  ~  c^2 / (2 L).
Numerically, with the canon Sciama density 1.33e-26 kg/m^3:
  c sqrt(G rho_env) = 2.8e-10 m/s^2 = 2.3 a0.  Order unity. (T2)
This is Milgrom's a0 ~ c H0 / 2pi coincidence, restated. TWO READINGS:
  - conventional: L = c/H0 with H0 a rate; a0 tied to cosmic
    expansion (hence the dark-energy talk in the MOND literature).
  - JM (2026-09-15): H0 is a redshift-per-distance ratio, not a
    velocity or a time. Then L = L_z is the redshift length (~4 Gpc),
    the Sciama condition is purely static, and
        a0 ~ c^2 / (2 L_z)
    is an acceleration built from c and a LENGTH of the medium -- no
    expansion, no time. One fewer concept than the conventional
    reading, and it connects a0 to the same length the tired-light /
    BH2 side of the program already uses.
MECHANISM SLOT: a0 = c / t_dyn(ambient), with t_dyn = 1/sqrt(G rho_env).
A response that changes character when the LOCAL dynamical time
exceeds the AMBIENT one is a response that switches at g ~ a0. That is
a place F1 (Sec. 4) could acquire the acceleration scale without it
being inserted. Not derived; located.
  H7  a0 ~ c sqrt(G rho_env) ~ c^2/(2L) to a factor ~2 with the canon
      rho_env; L is a length, static under JM's reading of H0 (T2)
  H8  a0 = c/t_dyn(ambient) is the candidate switching criterion for
      F1 (T3)

## 9. TWO POTENTIALS, NOT ONE (JM, same session) -- CORRECTS SEC. 3, 8
JM: the Sciama calculation gives Phi_bg, a UNIVERSAL CONSTANT. Phi_env
is the local sum of EXTERNAL masses (cluster, neighbours, filament)
and varies galaxy to galaxy. Read every "rho_env" in Sec. 3 and 8 as
rho_bg (the Sciama density, universal); the numbers are unchanged, the
labels were wrong. A galaxy's response is to phi_gal measured against
Phi_bg + Phi_env.
Division of labour:
  Phi_bg / rho_bg (universal)  -> a0 ~ c sqrt(G rho_bg) ~ c^2/(2 L_z);
                                  zero of the response; the not-below-
                                  zero floor; the same profile SHAPE
                                  for every galaxy.
  Phi_env / rho_env (local)    -> where the halo MERGES (constraint 5);
                                  the EFE-like term; the reference
                                  level that rho_nb,local may fall
                                  below. Isolated galaxy: edge at
                                  L_z-scale distance. Cluster member:
                                  cut off where Phi_env dominates.
This is constraint (5) with a mechanism, and it is why MOND needs the
EFE as an add-on while a two-level potential gives it natively.
  H9  Phi_bg (universal, Sciama) and Phi_env (local, external masses)
      are distinct; a0 and the profile shape come from the first, the
      halo edge from the second (JM, T3 -> to be ratified)

## 10. THE FLOOR IS rho_bg, NOT ZERO (JM, same session)
JM: deep voids asymptotically approach Phi_bg but never reach it,
because every point has some Phi_env from external masses. So the
physical floor on rho_nb,local is rho_bg (> 0), tighter than the
logical "not below zero" of Sec. 0.
CONSEQUENCES FOR RON BORROWING (Sec. 5):
  (a) Voids cannot be the source: they are already at the floor. A
      galaxy borrows from regions with rho_env > rho_bg -- its own
      group / filament / cluster outskirts. Budget per galaxy:
      (rho_env - rho_bg) x drawable volume. Finite and environment-
      dependent (fits constraint 5).
  (b) The depletion shell is bounded below by rho_bg.
  (c) TENSION: isolated galaxies have rho_env ~ rho_bg and hence the
      smallest budget, yet they show the flattest, most extended
      halos (Mistele/Meduri, isolated-lens selection). So EITHER the
      drawable volume is enormous (L_z-scale, i.e. the galaxy draws on
      the universe, and "isolated" is never isolated at that scale),
      OR the halo mass is not borrowed from the surrounding count at
      all and the count rule does not bound it (which reopens the
      mass-per-tron question of Sec. 4, F2, in a form where the ADDED
      mass is not drawn from neighbouring trons). This is the
      sharpest objection to borrowing so far and it follows from JM's
      own floor rule.
  H10 rho_bg is the physical floor; voids approach it asymptotically
      (JM, T3 -> to be ratified)
  H11 Borrowing budget = (rho_env - rho_bg) x volume; isolated
      galaxies have the least budget and the biggest halos -- borrowing
      needs an L_z-scale drawable volume or is not the mechanism (T3)

## 11. LENSING IS grad(n), NOT ENCLOSED MASS (JM, same session)
JM: in the refractive picture deflection ~ grad(n), n a function of
local tron density; lensing tracks DENSITY GRADIENTS, not enclosed
mass as such. Correct. Qualification that decides whether it is a
loophole:
  Axiom 6 + PPN gamma give delta n / n ~ 2|Phi_total|/c^2 with
  Phi_total sourced by ALL mass (Sun, baryons, rho_nb). So
  grad(n) ~ grad(Phi_total), and for spherical / azimuthally averaged
  systems that is G M_enc / r^2 via Poisson. Enclosed mass re-enters
  through Poisson, not through optics.
  => Mistele/Meduri (stacked, isolated, effectively spherical): the
     refractive and GR pictures give the SAME Delta-Sigma and the same
     deprojected V_c. No loophole; flat-to-300-kpc stands.
  => Bullet (non-spherical): grad(Phi) at the galaxy peaks is set by
     the LOCAL concentration; a broad gas slab contributes a weak
     gradient. This is the correct form of the Paper I Fig. 6
     argument -- not "uniform gas does not lens" (it does) but
     "compact concentrations produce steep grad(Phi) and dominate the
     convergence peaks." Same point as the freshlook Sec. 4 objection.
  => NEW TEST: if the tron index responded to LOCAL rho_nb rather than
     to Phi_total, lensing would be more localised than GR predicts
     and lensing-RAR would diverge from kinematic-RAR where the halo
     is diffuse. Brouwer+2021 find them consistent => the index tracks
     Phi_total to that precision. A measured constraint on Axiom 6's
     functional form.
  H12 Lensing ~ grad(n) ~ grad(Phi_total); equals enclosed-mass
      lensing for spherical systems, differs only in geometry (Bullet).
      Brouwer 2021 bounds any local-density optical response (T2/T3)

## 12. THE MATTER BUDGET DECIDES AGAINST BORROWING (same session)
Definitions (no LCDM parameters; ratios to the Sciama density
rho_S = 3c^2/(4 pi G L_z^2) ~ 1.3e-26 kg/m^3, JM's L_z reading of H0):
  rho_matter,dyn ~ 2-3e-27 kg/m^3  -- what clusters, lensing and galaxy
      dynamics SEE: baryons + non-baryonic mass bound in structures.
      Measured without cosmology (M/L x luminosity density, lensing
      mass in volumes). A uniform component is invisible to it.
  rho_matter,dyn = rho_b + <rho_nb,excess>  ~ 6 rho_b
  rho_S           = rho_b + rho_bg + <rho_nb,excess>,   rho_bg ~ 85%.
Sciama's Phi_bg = -c^2 is NOT satisfied by known matter (baryons give
-0.025 c^2; baryons + 5x DM give -0.15 c^2); the medium must be 5-7x
all dynamically measured matter. Option kept: the substrate supplies
the shortfall (canon). Note dark energy plays no role anywhere here.
WHETHER <rho_nb,excess> IS A SEPARATE TERM DEPENDS ON F2:
  BORROWED halos (count conserved, m per tron fixed): universe-average
    excess = 0; every overdense halo is paid for by an underdense
    region -- which must then sit BELOW rho_bg. Forbidden by the floor
    rule (Sec. 10).
  MADE halos (m per tron rises in a well; F2 does the work): excess is
    real additional mass, <excess> ~ 5 rho_b > 0, voids stay at rho_bg,
    floor rule holds.
=> The floor rule (H10) and the measured rho_matter,dyn jointly select
   F2 (mass created / increased per tron in wells) over borrowing. This
   is the clean form of the isolated-galaxy objection in Sec. 10(c).
  H13 Floor at rho_bg + measured rho_matter,dyn ~ 6 rho_b are jointly
      inconsistent with count-conserving borrowing; the halo channel
      must ADD mass (F2), not redistribute it (T2/T3)

## 13. CORRECTION (JM, same session): THE DENSITY FLOOR IS ZERO
JM revises: regions CAN dip below rho_bg -- "into" it -- but not below
zero. The Sec. 10 statement that voids approach Phi_bg asymptotically
stands as a statement about the POTENTIAL; it does not imply a density
floor at rho_bg. So:
  H10 WITHDRAWN as a density floor; keep only: Phi_env -> Phi_bg in
      deep voids.
  H13 WITHDRAWN: with the floor at zero, count-conserving borrowing
      is consistent with the matter budget again. Universe-average
      excess can be zero with underdense regions below rho_bg.
  H11 survives in weakened form: the borrowing budget is now up to
      rho_env x volume (not rho_env - rho_bg), so isolated galaxies
      have MORE to draw on than Sec. 10(c) assumed; the objection
      becomes "the drawable volume must be large," not "impossible."
STATUS AFTER CORRECTION: both F2 routes are open again -- borrowing
(count conserved, mass redistributed) and mass-per-tron increase
(mass added). The matter budget (Sec. 12, definitions) no longer
discriminates between them. What would: a measured depletion (or its
absence) at 300 kpc - few Mpc around isolated galaxies. Borrowing
predicts a shell BELOW rho_bg there; mass-per-tron predicts none.
  H14 Density floor is zero; voids may sit below rho_bg (JM). Borrowing
      predicts a sub-ambient shell around galaxies; mass-per-tron does
      not. Lensing at 0.3-3 Mpc discriminates (T3)

## 14. THE OTHER HELMHOLTZ BRANCH IS THE JEANS BRANCH (JM's question)
JM: original design was "rho_nb begets more rho_nb" (self-sourcing);
the gapped operator turned that into SCREENING (negative feedback ->
Yukawa cutoff); maybe the +k^2 branch is the borrowing.
T2: For ANY response rising with the bump, rho_nb = rho_bg[1 + f(phi)]
with f'(0) > 0, self-consistent Poisson linearises to
      grad^2 phi + k_J^2 phi = 4 pi G rho_b,   k_J^2 = 4 pi G rho_bg f'(0).
Boltzmann is the case f'(0) = 1/sigma^2, giving the JEANS wavenumber
k_J = sqrt(4 pi G rho_bg)/sigma. So:
  -k^2 (gapped)   = negative feedback = screening = no halo (Paper I)
  +k^2 (Helmholtz)= positive feedback = Jeans = the amplifier
Solutions phi ~ cos(k_J r)/r: positive core, NEGATIVE shell (below
ambient) at the first node, decaying oscillation beyond. That IS the
compensated / borrowed profile. Scale: sigma ~ 100-160 km/s, rho_bg ~
1.3e-26 => lambda_J = 2 pi sigma / sqrt(4 pi G rho_bg) ~ 6-9 Mpc;
first depletion shell at ~3-4 Mpc. Beyond Mistele; consistent with
H14; and the borrowing scale is DERIVED (Jeans length of the medium),
not fitted.
RECONCILIATION WITH 9/1 OPERATOR-SIGN TEST: cos(kr)/r fit SPARC worse
than Yukawa (5.20 vs 2.06) because at k_J r << 1 the LINEAR +k^2
solution is Newtonian -- no halo at 10 kpc in the linear regime. The
halo is the NONLINEAR saturated interior (for Boltzmann: the r^-2
sphere). The 9/1 test was a linear-regime test and correctly found
nothing there; it does not bear on the nonlinear branch.
STRUCTURE THAT FALLS OUT:
  linear Jeans branch, Mpc scales  -> oscillation, depletion shells,
                                      borrowing
  nonlinear saturation, inner      -> r^-2 core + halo (the 10^4)
  gapped branch                    -> stable sign, loses both
CAVEAT (corrected per JM): JM's position is only that the substrate
does not necessarily behave like a STANDARD macroscopic fluid (no
fixed-size particles, no ordinary pressure, compression by shrinkage,
count conserved). The STRUCTURE above uses none of those: it needs
only (i) f'(0) > 0 at the background (amplifying) and (ii) saturation
at large f (bounded), plus self-gravity. Those hold for any responsive
medium with finite capacity. What Boltzmann adds -- the exponential
form, sigma as temperature, hydrostatic balance -- gives the specific
NUMBERS (lambda_J ~ 6-9 Mpc, King core ~5 kpc) and those are
ILLUSTRATIVE until F2 is written in Tron terms.
  H15 +k^2 = Jeans branch of any bump-rising response; k_J from
      rho_bg and f'(0); depletion shells at ~lambda_J/2 ~ 3-4 Mpc (T2)
  H16 F2 must be amplifying at ambient and saturating in the bump;
      the halo is the saturated regime, the shells are the linear
      regime (T3)

# END — [UNRATIFIED]
