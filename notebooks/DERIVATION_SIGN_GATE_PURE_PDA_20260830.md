# DERIVATION — SIGN GATE UNDER PURE PDA
# trontology\notebooks\DERIVATION_SIGN_GATE_PURE_PDA_20260830.md
# Written 2026-08-30 late (~23:00 EDT). Status: RATIFIED —
# B7 stamped KEEP by JM 2026-08-30 late session.
# DATING NOTE: all dates in this file are JM-LOCAL (EDT), matching the
# repo convention. An earlier draft was stamped 2026-08-31 from a UTC
# clock; corrected. The 8/30 AFTERNOON session and this 8/30 LATE
# session are distinct — see timeline below.
# FIREWALL: Tron-side. Never enters GPRF-facing materials.

## WHY THIS FILE EXISTS

R7 was recorded in SESSION_HANDOFF_20260830_TRON_QUANT.md as a one-line
result with no working behind it. The derivation itself existed only in
the 2026-08-30 session transcript and was recoverable only because JM
kept the share link. That is a single point of failure for a result the
entire PDA chain runs through. This file makes it durable.

PROVENANCE NOTE, and it matters for how much weight this file carries:
the derivation below is recovered from the transcript of the 2026-08-30
TRON-QUANT session, read 2026-08-30 late via the share link JM supplied. It
is a transcription of work done in that session, not a fresh re-derivation
in this one. Marked [RECOVERED] throughout. A cold re-derivation from the
axioms is still worth doing and is NOT what this file is.

TIMELINE, for the record — a snap/handoff conflict that cost a round trip:
  ~20:24  SNAP_001 written. Its NEXT ACTIONS list item (1) reads
          "re-run sign gate pure-PDA rigorously (flux asymmetry)."
  ~20:5x  Three further exchanges.
  ~21:0x  Sign gate re-run EXECUTED, plus conservation theorem and the
          adaptive-kernel toy numerics.
  ~21:26  Handoff written, recording R7 as PASS [T2].
The snap's action list was therefore STALE AT WRITE TIME relative to the
handoff, and the 8/30 late session misread it as evidence that the
re-run had not happened. See PROCESS NOTE at the end.

## PREMISES [T1 — from the 2019 Tron paper, Axioms 3-5]

P1. CONTIGUITY. Tron size a and number density d are locked:
    a ~ d^(-1/3). Denser tronos <=> smaller trons. (Fig. 2/3 witness.)
P2. PDA (potential-difference attraction). The elemental law is
    DIFFERENCE-driven: trons seek equilibrium with their neighbours.
    JM/Richard axiom; JM's words recovered from the copilot transcript
    (~line 26340): "the potential difference attraction axiom - trons
    seek equilibrium"; "the value of this pda is proportional to 1/r -
    it gets stronger as you approach the core" (the latter is a FIELD
    PROFILE statement, not a coupling law).
P3. CORE. A baryon is a collective bound structure of maximally
    compressed trons at fixed small size a_c, interfaced to the ambient
    tronos through the Axiom-5 boundary condition (peripheral rons
    matching ambient).

## THE DERIVATION [T2, RECOVERED]

Interfacial energy of a core sitting in an ambient gradient. Sum over
boundary contacts:

    E(x_c) = SUM_boundary  (1/2) * kappa * (a_c - a(x))^2

Expand a(x) about the core centre x_c. The isotropic (zeroth-order)
part of the shell sum contributes no net force — a core in a UNIFORM
tronos feels nothing, which is the correct null result. The linear term
survives the shell sum:

    F = N_b * kappa * (a_c - a(x_c)) * grad a

SIGN. Cores are compressed, so a_c < a everywhere in the ambient medium.
Hence (a_c - a) < 0 and

    F  points along  -grad a

By P1, -grad a points toward smaller ambient trons, i.e. toward HIGHER
density. The force is toward density. GATE PASSES.

INPUTS REQUIRED — only two, and both are cheap:
  (i)  kappa > 0. Mismatch costs energy. This IS the equilibrium-seeking
       content of PDA; it is not an extra postulate.
  (ii) a_c < a_ambient. Definitional for a compressed core.

WHAT IS NOT REQUIRED, and this is the whole point of the re-run: no
bond-strength monotonicity assumption. The ORIGINAL sign gate used
sigma'(a) > 0 — an ABSOLUTE bond strength — which is a non-PDA
ingredient, since PDA is difference-driven and contains no absolute
reference. That ingredient is gone. The argument also got shorter,
which is the usual sign that scaffolding was removed rather than hidden.

## SOURCE-SIGN CLOSURE AND THE THIRD LAW [T2, RECOVERED]

The same axiom supplies the other half of the loop, so no second
postulate is needed to make gravity attractive.

Ambient trons adjacent to a core shed rons (PDA drives larger -> smaller
toward the compressed neighbour), shrink, and therefore pack denser:

    delta_d > 0 around mass.

So one rule yields BOTH:
  - pile-up of ambient density around core A (source sign), and
  - migration of core B toward that pile-up (force sign).

Symmetric under A <-> B, so the third law holds by construction rather
than by assumption. Gravity is one PDA rule seen twice.

## WHAT THIS DOES AND DOES NOT ESTABLISH

ESTABLISHES:
  - Attraction, with the correct sign, from PDA alone.
  - The null result in a uniform medium (no force without a gradient).
  - Third law by symmetry.
  - The interfacial coupling constant kappa and the core count N_b as
    the only free ingredients at this level.

DOES NOT ESTABLISH:
  - Magnitude. kappa is not derived here; g (the source coupling in
    (-A grad^2 + B) delta_d = g rho_b) is step (4) and remains owed.
  - Anything about B. This gate is sign-only. B = 0 under pure PDA
    (R3), and the whole anomaly lives in the breaking term.
  - The 1/r^2 force law. That follows separately from B = 0 (see R3),
    not from this gate.

## APPENDIX — CONSERVATION THEOREM [T2, RECOVERED]
## STATUS: [UNRATIFIED]. B6 is pending a RESTATE, not stamped keep.
## Recorded here because its derivation has the same durability problem.

In the pure phase (B = 0) the response to a single core is

    delta_d ~ 1/r     =>     INT delta_d d^3r  ~  INT (1/r) r^2 dr  ~  R^2

which diverges. One nucleon in a pure-PDA tronos would demand infinite
ron redistribution. Global tron conservation is violated. And a
per-core divergent response is Neumann-Seeliger seen locally.

So conservation <=> static-background existence <=> B > 0 <=> finite
lambda, and candidates (b) and (d) collapse to one condition.

RESTATE RIDER (flagged 2026-08-30 late, JM ruling pending): the collapse is
valid at the level of "B > 0 is REQUIRED." It is NOT valid at the level
of a single VALUE of B. Conservation needs only that lambda be finite.
The static cosmos wants lambda ~ c/H0 ~ 4.3 Gpc. Galactic phenomenology
wants r_M ~ 14 kpc. Those last two differ by ~3e5. Writing it as "one
condition" conceals exactly the gap that wall (alpha) is made of.

## PROCESS NOTE — snap/handoff staleness

A snapshot's NEXT ACTIONS list is a to-do list timestamped at the moment
of writing. A later handoff may discharge those items without saying so.
A future session then reads the snap's open items as live and
second-guesses ratified results. This happened on 2026-08-30 late and cost a
round trip on B7.

FIX, proposed for the session mechanics in gprf\SESSION_BOOT.md: every
handoff carries an explicit close-out line against the snapshot it
supersedes, e.g. "SNAP_001 NEXT ACTIONS: (1) discharged; (2),(3) open."
Cheap to write, and it removes the ambiguity entirely.

## POINTERS
- SESSION_HANDOFF_20260830_TRON_QUANT.md — R3, R6, R7, R8; ballot.
- autosave\SESSION_SNAP_20260830_001.md — per-step detail; STALE on the
  sign-gate item specifically (see timeline above).
- DRAFT_TRON_SUBSTRATE_CONSERVATION_20260830.md — identification note,
  [UNRATIFIED], post-PDA revision owed (B11).

# END
