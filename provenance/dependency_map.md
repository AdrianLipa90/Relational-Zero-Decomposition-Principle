# RZDP Dependency Map

```text
A0
|
+-- Relational-Zero core
    |
    +-- RH: location ---------------------- CONDITIONAL ON A0
    |
    +-- Multiplicity-index transfer ------- THEOREM
    |   +-- transverse crossing
    |       -> ord(det A) = dim ker A
    |
    +-- Bockstein crossing ---------------- THEOREM
    |   +-- 2-term perfect complex
    |   +-- beta = q A'(0)|ker
    |   +-- beta iso -> ord(det)=dim H1
    |
    +-- BSD: multiplicity/index
    |   +-- analytic order = winding ------ THEOREM
    |   +-- analytic order = local length - THEOREM
    |   +-- MW rank = exterior degree ----- THEOREM
    |   +-- analytic/Selmer parity mod 2 -- THEOREM
    |   +-- Selmer/Sha defect split ------- THEOREM
    |   +-- B3 = height/Bockstein gate ---- CONDITIONAL CROSSWALK
    |   |
    |   +-- C1 complex L -> p-adic/zeta --- OPEN_BRIDGE
    |   +-- C2 zeta -> Selmer determinant - OPEN_BRIDGE
    |   +-- C3 regulator nondegeneracy ----- OPEN_BRIDGE
    |   +-- C4 specialization/control ------ OPEN_BRIDGE
    |   +-- C5 Sha-divisible control ------- OPEN_BRIDGE
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
