# LIT / HYPOTHESIS — A NON-RELIC CMB: OLBERS-REDSHIFT + CONTIGUOUS-MEDIUM FOG
# trontology\notebooks\LIT_CMB_ALTERNATIVE_20260918.md
# 2026-09-18. Status: [UNRATIFIED]. Tron/cosmology-side (separate from the
# GPRF rotation-curve program, which stands without any of this). Origin:
# JM's contention that the CMB is not a Big Bang relic but arises from the
# integrated, redshifted radiation of an infinite uniform universe, with a
# contiguous space-filling medium setting the observed spectrum. Worked
# through with Claude 2026-09-18. Calculations are order-of-magnitude shape
# tests, NOT a fit to FIRAS. Everything to VERIFY before any manuscript use.

## 0. THE HYPOTHESIS (JM)
- The universe is unbounded and roughly uniform in density far beyond
  14 Gly (no edge, no Big Bang).
- H0 is redshift-per-distance (an inverse length), not an expansion rate;
  redshift accumulates with distance, 1+z ~ exp(r/L_z) or similar monotonic
  law.
- Light from ever-more-distant sources is redshifted ever-more, piling up
  into the microwave. The CMB is that integrated background, NOT a relic of
  a hot dense phase.
- A contiguous, space-filling medium (the Tron substrate) is present at the
  ambient density everywhere including here.

## 1. OLBERS, RESOLVED BY REDSHIFT (this part WORKS)
In an infinite uniform static universe each equal-thickness shell contributes
EQUALLY to the sky brightness: flux per source ~ 1/r^2, sources per shell ~
r^2, the r^2 CANCELS. Without redshift this diverges -> bright sky (Olbers).
WITH cumulative redshift 1+z=exp(r/L_z), each shell's energy is dimmed by
1/(1+z)=exp(-r/L_z), so the integral INT exp(-r/L_z) dr CONVERGES to a finite
background ~ n L L_z. So:
  - the r^-2 inverse-square law IS accounted for (it cancels the shell volume);
  - redshift is not optional decoration -- it is the ONLY thing preventing an
    infinitely bright sky. This is Olbers' paradox resolved by redshift in a
    static infinite universe, the classical alternative to the finite-age
    resolution. Sound and standard as far as it goes.

## 2. THE SPECTRAL-SHAPE WALL (the central problem)
FIRAS: the CMB is a single-temperature Planck spectrum, 2.725 K, deviations
< 1e-5. A Planck curve has low-frequency (Rayleigh-Jeans) slope EXACTLY +2 and
a sharp exponential (Wien) high-frequency cutoff.
CALCULATION (shape test, source BB at Ts, integrated over u=1+z in [1,1e4]):
  bare superposition of redshifted sources:  low slope +1.6, high slope +1.0,
    peak at wrong frequency. NOT Planck.
Reason: summing blackbodies over a continuous range of redshifts = summing a
range of temperatures = a spectrum BROADER than any single Planck curve. You
cannot add Planck curves of different T and recover a Planck curve.
=> A bare redshifted-superposition CMB is EXCLUDED by FIRAS on shape. This is
the same wall the Hoyle/Lerner/tired-light thermalization models hit; JM
reaches it from the infinite-universe direction.

## 3. THERMALIZATION: LOCAL WORKS, EN-ROUTE FAILS (the key result)
Test: let a medium absorb and re-emit the radiation (thermalize it). WHERE it
happens decides the spectrum.
  CASE A, en-route (re-emission happens out at distance, so the re-emitted
    photon ALSO redshifts on its way to us): fixes the low slope to +2 but the
    high slope stays ~+2 and the peak lands at ~2000 GHz, NOT 160. Fails --
    because thermalizing to BB(T_m) and then redshifting BB(T_m) over a range
    of distances just re-creates the superposition one level down (now in the
    medium's spectrum instead of the sources').
  CASE B, local (thermalization in the last mean-free-path before arrival, at
    z~0): a single clean BB(T_m). low slope +1.9, sharp Wien cutoff, PEAK 160
    GHz at 2.725 K. This is essentially FIRAS.
CONCLUSION: a non-relic CMB matches the FIRAS blackbody IF AND ONLY IF the
thermalization is LOCAL, not distributed along the path.
=> This selects a CONTIGUOUS space-filling medium over a sparse absorber or a
nearby shell: a sparse/distributed absorber thermalizes en-route (Case A,
fails); a contiguous medium present at our location thermalizes in the last
optical depth (Case B, works). The Tron substrate is a Case-B thermalizer by
construction. The CMB temperature is then a LOCAL property of the medium's
equilibrium -- 2.725 K = the substrate temperature here, now -- fed by the
integrated redshifted radiation from the infinite universe (global energy
reservoir) but emitted locally as a clean blackbody (local spectrum).
FOG ANALOGY: looking into infinite fog, the light you see is from the fog one
mean-free-path in front of you, at the fog's temperature, even though the fog
is endless and lit from far away. Photosphere local, reservoir global.

## 4. THE SZ CONSTRAINT (discriminator + sharpest burden, JM 2026-09-18)
Thermal Sunyaev-Zel'dovich: CMB photons scatter off hot cluster electrons, so
the CMB must be a BACKLIGHT originating BEHIND the clusters. SZ is measured
against clusters to z~1-2.
  => KILLS the nearby-shell models: Zwicky-tired-light (arXiv:2504.10510) puts
     the source at z<=0.051 / 240 Mpc; clusters beyond that are IN FRONT of the
     source and could not produce the observed SZ decrement. Nearby-shell
     version FAILS SZ.
  => FAVORS the contiguous-fog version: with medium everywhere, there is always
     reservoir BEHIND any cluster (SZ ok), while the spectrum is still set in
     the last mean-free-path here (blackbody ok). SZ needs the SOURCE far; the
     blackbody needs the SPECTRUM set local; only an optically-thick
     space-filling medium delivers both (energy far, photosphere local).
  => SHARPEST FORM OF THE OPACITY BURDEN: space is OBSERVED highly transparent
     at microwave frequencies -- we see the dipole, the acoustic-scale
     structure, and SZ imprints THROUGH to distant clusters. A medium optically
     thick enough to thermalize (tau >> 1 over cosmological paths) is in tension
     with one transparent enough to see SZ through. The needle to thread: a
     tau(nu) that is >>1 over cosmological distance for thermalization yet leaves
     cluster SZ imprints and small-scale structure visible. Whether such a
     tau(nu) exists is THE calculation; unaddressed. Every opaque-universe model
     since Eddington has had to thread this and none has cleanly.

## 5. THE POWER SPECTRUM (the standing UNSOLVED burden)
The angular power spectrum C(l) -- first acoustic peak at l~220 (~1 deg), the
2nd/3rd peak height ratios that pin Omega_matter ~ 5-6x Omega_baryon -- is NOT
explained by ANY superposition / tired-light / fog model, including the
published ones (Zwicky-TL 2504.10510 addresses the MONOPOLE spectrum and
foregrounds, not the peaks). This is the hardest open item.
Two escape routes, BOTH someone else's open argument, neither a result:
  (a) INSTRUMENTAL: Hossenfelder (Backreaction, 2007) argued the high-l 2nd
      peak could be an artifact of the differential twin-beam telescope design
      -- for a homogeneous background the differenced signal's beam profile is
      the sqrt of the single-beam profile, which can manufacture apparent power
      at those scales. A specific instrument-level version of the "extracting
      pattern from a Gaussian field" worry. Narrow claim (one peak), not "CMB
      is galaxy light."
  (b) STRUCTURAL: the ~1 deg scale and harmonic pattern reflect real structure
      in the source/medium distribution. Nobody has derived this.
HONEST STATUS: the peaks were PREDICTED pre-1970 (Peebles-Yu, Sunyaev-
Zel'dovich) and detected at the predicted scales -- so they survive the
"just-so / noise / Rorschach" family of objections (they are global averages,
not spotted features, and were called in advance). A non-relic CMB must either
DERIVE the peaks from the medium or make a real systematics case. Not done.
This is where the alternative is furthest behind and must not overclaim.

## 6. WHERE THE DATA MIGHT FAVOR THE ALTERNATIVE
- ARCADE-2 / extragalactic radio background: the radio background at 3-90 GHz
  is several times brighter than known sources predict, unexplained. An
  integrated/superposition model NATURALLY predicts excess power on the
  low-frequency (radio) side from the most-redshifted distant pile-up; the
  relic model does not. Candidate POSITIVE signature. VERIFY current status
  (ARCADE-2 Fixsen+2011; later LWA/radio-background work).
- Foregrounds prove galaxies DO emit microwaves (the monopole-removal step in
  every CMB pipeline). Empirical toehold that galaxy microwave emission is
  real and non-negligible.
- CMB dipole as motion through the LOCAL medium rest frame -- ties to the
  ECI/ether thread (BH2). In this picture the dipole frame IS the substrate
  rest frame, a physical rather than merely kinematic statement.

## 7. NEAREST PUBLISHED NEIGHBORS (read/verify before citing)
- arXiv:2504.10510, "CMB within the Zwicky Tired Light Hypothesis" (2025):
  CMB = superposition of galaxy microwave radiation from an opaque region,
  z<=0.051, <=240 Mpc, <=5% energy loss. SAME family as JM's idea but NEARBY-
  shell -> fails SZ (Sec. 4). Also a 2025 result: intergalactic dust mimics a
  blackbody at 2.776 K vs observed 2.725 K (close). Read full text.
- Hoyle-Wickramasinghe (iron whiskers), Lerner (plasma/tired light), Marmet:
  the thermalization-by-sparse-absorber lineage. All Case-A (en-route) -> the
  broadening problem. JM's contiguous-medium is Case-B and distinct.
- Hossenfelder 2007 Backreaction post on the differential-beam artifact (blog,
  not a paper; find if it was ever written up formally).

## 8. SCORECARD
  Olbers / r^-2 / redshift convergence ............ WORKS (Sec.1)
  Blackbody monopole shape ........................ WORKS iff thermalization
                                                    is LOCAL (contiguous
                                                    medium); en-route fails
                                                    (Sec.3)
  SZ (source behind clusters) ..................... FAVORS contiguous-fog,
                                                    KILLS nearby-shell (Sec.4)
  Microwave opacity vs observed transparency ...... OPEN, the tau(nu) needle
                                                    (Sec.4) -- the central
                                                    physical burden
  Angular power spectrum / acoustic peaks ......... UNSOLVED (Sec.5) -- the
                                                    hardest item; must derive
                                                    or make a systematics case
  Low-freq radio (ARCADE-2) ....................... POSSIBLE POSITIVE signature
                                                    (Sec.6)

## 9. RATIFICATION
  C1  Olbers resolved by redshift in an infinite static universe; r^-2
      cancels shell volume; redshift makes the background finite (T2)
  C2  Bare redshifted-superposition CMB is NOT Planck (low slope ~+1.6 vs
      required +2); excluded by FIRAS on shape (T2)
  C3  LOCAL thermalization recovers a clean 2.725 K Planck (peak 160 GHz,
      Wien cutoff); EN-ROUTE thermalization re-broadens and fails (T2)
  C4  => a CONTIGUOUS space-filling medium is required (Case-B thermalizer);
      sparse absorbers and nearby shells are Case-A and fail (T3)
  C5  SZ requires the source behind clusters => kills nearby-shell TL models,
      favors contiguous-fog (energy global, photosphere local) (T2/T3)
  C6  microwave-opacity-vs-transparency is the central unmet burden: need a
      tau(nu) >>1 over cosmological path yet SZ- and structure-transparent (T3)
  C7  the acoustic power spectrum is UNSOLVED by all superposition models;
      escapes (instrumental a la Hossenfelder; structural) are unproven (T3)
  C8  ARCADE-2 radio excess is a candidate positive signature of the
      integrated pile-up (T3, verify)
  C9  independent of the GPRF rotation-curve result, which stands without any
      CMB model (T1)

# END — [UNRATIFIED]
