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
    |   +-- beta = q A'(0)|ker
    |   +-- epsilon = ord(det)-dim H1 >= 0
    |   +-- epsilon = 0 iff beta iso
    |
    +-- Smith multiplicity spectrum ------- THEOREM
    |   +-- invariant factors T^{a_i}
    |   +-- contact depth d_i=a_i-1
    |   +-- epsilon = sum d_i
    |
    +-- Determinant relative valuation ---- THEOREM
    |
    +-- BSD: multiplicity/index
        |
        +-- common exact input
        |   +-- analytic order = winding -------- THEOREM
        |   +-- analytic order = local length --- THEOREM
        |   +-- MW rank = exterior degree ------- THEOREM
        |   +-- analytic/Selmer parity mod 2 ---- THEOREM
        |   +-- Neron-Tate pairing nondeg. ------ THEOREM
        |   +-- rank <= 1 derivative-height ----- THEOREM / SANITY CHECK
        |
        +-- Route A: archimedean direct
        |   +-- A1 L-germ -> determinant family - OPEN_BRIDGE
        |   +-- A2 kernel/coker -> MW/MW* ------- OPEN_BRIDGE
        |   +-- A3 crossing = Neron-Tate height - OPEN_BRIDGE
        |   +-- A1+A2+A3 -> BSD ---------------- CONDITIONAL THEOREM
        |
        +-- Route S: p-adic Selmer
            +-- determinant/Stark carrier ------- CONDITIONAL STANDARD CARRIER
            +-- Selmer/Sha defect split -------- THEOREM
            +-- D2 complex L -> zeta section --- OPEN_BRIDGE
            +-- D3 zeta -> Selmer determinant -- OPEN_BRIDGE
            +-- D4 contact-depth/Bockstein ------ LOCAL THEOREM; GLOBAL OPEN
            +-- D5 specialization/control ------- OPEN_BRIDGE
            +-- D6 Sha-divisible control -------- OPEN_BRIDGE
            +-- registered BSD defect
                = sum_i d_i(E,p) + s_p(E) >= 0 - CONDITIONAL NORMAL FORM
```

The two BSD routes are intentionally separate.

**Route A** works directly on Mordell--Weil geometry. Once the crossing is independently identified with the Neron--Tate height map, transversality is automatic because the canonical height pairing is nondegenerate.

**Route S** works through a p-adic Selmer complex. Its specialized dimension is the Selmer corank, not automatically the Mordell--Weil rank, so the explicit Sha-divisible obstruction remains.

Gross--Zagier--Kolyvagin supplies a rank-one sanity check for Route A: a first L-derivative/height relation controls an arithmetic zero mode in the known simple-zero case. It does not furnish the arbitrary-rank comparison.

The determinant-line carrier is standard arithmetic structure; proving the universal complex-L/zeta registration remains unresolved.

The existing PNCS/Infinities Fredholm shift seam remains only an index grammar: no canonical elliptic-curve comparison map to that shift model has been proved.
