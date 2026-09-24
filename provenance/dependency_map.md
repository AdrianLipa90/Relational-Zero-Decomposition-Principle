# RZDP Dependency Map

```text
A0
|
+-- Relational-Zero core
    |
    +-- RH: location ---------------------- CONDITIONAL ON A0
    |
    +-- Multiplicity-index transfer ------- THEOREM
    +-- Bockstein crossing ---------------- THEOREM
    +-- Smith multiplicity spectrum ------- THEOREM
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
        |   +-- A1 complex L -> determinant ---- OPEN_BRIDGE
        |   +-- A2 kernel/coker -> MW/MW* ------ OPEN_BRIDGE
        |   +-- A3 crossing = Neron-Tate height  OPEN_BRIDGE
        |   +-- A1+A2+A3 -> BSD --------------- CONDITIONAL THEOREM
        |
        +-- Route S: p-adic Selmer
            +-- D1 determinant/Stark carrier --- CONDITIONAL STANDARD CARRIER
            +-- D2a exceptional factor --------- LOCAL / SETTING DEPENDENT
            |   +-- raw section = E_exc*corr
            |   +-- e_exc = ord(E_exc) >= 0
            +-- D2b corrected interpolation ---- OPEN_BRIDGE
            |   +-- eta = r_an - ord(s_corr)
            |   +-- target eta=0
            +-- D3 determinant registration ---- OPEN_BRIDGE
            |   +-- rho=ord(s_corr/s_ar)
            |   +-- target rho=0
            +-- D4 contact depths d_i>=0 ------- LOCAL THEOREM; GLOBAL OPEN
            +-- D5 specialization/control ------ OPEN_BRIDGE
            +-- D6 Sha defect s_p>=0 ----------- OPEN_BRIDGE
            |
            +-- corrected full defect
                delta_BSD = eta + rho + sum_i d_i + s_p
                -------------------------------- CONDITIONAL NORMAL FORM
```

Exceptional/trivial zeros are not counted as Mordell--Weil rank. They are removed at D2a before the corrected interpolation defect `eta` is defined.

`eta` measures complex-to-corrected-p-adic order mismatch; `rho` measures corrected-p-adic-to-arithmetic determinant mismatch; `d_i` measure higher zero-mode contact; `s_p` measures hidden p-primary Sha corank.

The split-multiplicative Mazur--Tate--Teitelbaum / Greenberg--Stevens theorem is the canonical sanity check that raw p-adic vanishing can contain a local interpolation zero.

Kato's Euler-system divisibility attacks the p-adic analytic-to-Selmer comparison layer, not by itself the complex-to-p-adic corrected interpolation layer.

A0 controls relational zero support. It does not determine interpolation order, determinant valuation, jet/contact depth, or hidden Selmer quotient.
