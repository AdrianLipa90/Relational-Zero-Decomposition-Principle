# RZDP Dependency Map

```text
A0
|
+-- Relational-Zero core
    |
    +-- RH: location ---------------------- CONDITIONAL ON A0
    |
    +-- Multiplicity-index transfer ------- THEOREM
    |   +-- ord(det A) >= dim ker A
    |   +-- excess epsilon >= 0
    |   +-- epsilon = 0 iff crossing iso
    |
    +-- Bockstein crossing ---------------- THEOREM
    |   +-- 2-term perfect complex
    |   +-- beta = q A'(0)|ker
    |   +-- epsilon = ord(det)-dim H1 >= 0
    |   +-- epsilon = 0 iff beta iso
    |
    +-- Determinant relative valuation ---- THEOREM
    |   +-- two sections differ by scalar q
    |   +-- order difference = ord(q)
    |
    +-- BSD: multiplicity/index
    |   +-- analytic order = winding ------ THEOREM
    |   +-- analytic order = local length - THEOREM
    |   +-- MW rank = exterior degree ----- THEOREM
    |   +-- analytic/Selmer parity mod 2 -- THEOREM
    |   +-- Selmer/Sha defect split ------- THEOREM
    |   +-- determinant/Stark carrier ------ CONDITIONAL STANDARD CARRIER
    |   +-- B3 = height/Bockstein gate ---- CONDITIONAL CROSSWALK
    |   +-- registered excess epsilon >= 0 - CONDITIONAL
    |   +-- BSD defect = epsilon + Sha ----- CONDITIONAL NORMAL FORM
    |   |
    |   +-- D2 complex L -> zeta section --- OPEN_BRIDGE
    |   +-- D3 zeta -> Selmer determinant -- OPEN_BRIDGE
    |   +-- D4 regulator nondegeneracy ----- OPEN_BRIDGE
    |   +-- D5 specialization/control ------ OPEN_BRIDGE
    |   +-- D6 Sha-divisible control ------- OPEN_BRIDGE
    |   +-- all gates -> BSD --------------- CONDITIONAL THEOREM
    |
    +-- Yang-Mills: spectral isolation ---- OPEN_BRIDGE
    +-- Hodge: algebraic realization ------ OPEN_BRIDGE
    +-- Navier-Stokes: dynamical avoidance  OPEN_BRIDGE
    +-- P vs NP: resource separation ------ OPEN_BRIDGE
```

The map is descriptive, not a proof of equivalence between branches.

The Bloch-Kato / Tamagawa-number determinant-line formalism identifies the canonical standard search space for BSD. The Bockstein-crossing theorem closes the local multiplicity mechanism only; universal analytic registration, main-conjecture comparison, regulator nondegeneracy, control, and Sha-divisible gates remain separate.

The existing PNCS/Infinities Fredholm shift seam is not promoted into BSD: no canonical arithmetic-analytic comparison map has yet been proved.

The strongest current BSD normal form is conditional on global registration:

```text
BSD defect = Bockstein multiplicity excess + Sha corank
           = epsilon_{E,p} + s_p(E),
with both terms nonnegative.
```

The determinant-line carrier is standard arithmetic structure; proving the universal complex-L/zeta comparison remains the unresolved analytic registration.
