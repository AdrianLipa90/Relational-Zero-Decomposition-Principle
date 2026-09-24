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
        |   +-- A1 L-germ -> determinant family - OPEN_BRIDGE
        |   +-- A2 kernel/coker -> MW/MW* ------- OPEN_BRIDGE
        |   +-- A3 crossing = Neron-Tate height - OPEN_BRIDGE
        |   +-- A1+A2+A3 -> BSD ---------------- CONDITIONAL THEOREM
        |
        +-- Route S: p-adic Selmer
            +-- D1 determinant/Stark carrier ---- CONDITIONAL STANDARD CARRIER
            +-- D2 complex L -> analytic/zeta --- OPEN_BRIDGE
            +-- rho = ord(s_an/s_ar) ------------ CONDITIONAL REGISTRATION DEFECT
            +-- D3 unit comparison rho=0 -------- OPEN_BRIDGE
            +-- D4 contact depths d_i>=0 -------- LOCAL THEOREM; GLOBAL OPEN
            +-- D5 specialization/control ------- OPEN_BRIDGE
            +-- D6 Sha defect s_p>=0 ------------ OPEN_BRIDGE
            +-- full defect
                delta_BSD = rho + sum_i d_i + s_p
                --------------------------------- CONDITIONAL NORMAL FORM
            +-- after rho=0
                delta_BSD = sum_i d_i + s_p >=0
```

The three Route-S defects are typed and distinct:

- `rho` is the relative determinant-registration valuation and can have either sign until a divisibility theorem is proved;
- `d_i` are nonnegative Smith contact depths;
- `s_p` is the nonnegative p-primary Tate-Shafarevich corank.

Equality of analytic and arithmetic determinant ideals is exactly the unit condition `rho=0`. One-sided Iwasawa divisibilities give one-sided inequalities for `rho`; the two-divisibility strategy squeezes the same registration defect to zero.

Route A remains separate: it targets Mordell--Weil geometry directly and uses Neron--Tate nondegeneracy only after an independent crossing-height identification.

A0 controls relational zero support; it does not by itself determine determinant valuation, zero-mode jet/contact order, or hidden Selmer quotient.
