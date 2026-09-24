# BSD Corrected Interpolation / Exceptional-Zero Split v0.7

Status: **EXACT FACTORIZATION ALGEBRA / CONDITIONAL GLOBAL REGISTRATION / BSD STILL OPEN**

Date: 2026-09-24

## 1. Why raw p-adic order is not the analytic rank

A p-adic L-function may acquire zeros from local interpolation factors that are not zeros of the complex L-function.

Therefore the raw statement

\[
\operatorname{ord} L_p(E)=r_{\rm an}(E)
\]

is not a safe universal registration target.

The split-multiplicative exceptional-zero phenomenon is the standard warning example.

## 2. Exceptional-factor removal

Work locally over a one-dimensional p-adic analytic ring and suppose the raw p-adic analytic section admits a factorization

\[
s_p^{\rm raw}
=
\mathcal E_{E,p}\,s_p^{\rm corr},
\]

where \(\mathcal E_{E,p}\) is the explicit local interpolation factor responsible for the declared exceptional/trivial zero contribution.

Define

\[
e_{\rm exc}(E,p)
:=
\operatorname{ord}(\mathcal E_{E,p})
\ge0.
\]

Then exact valuation additivity gives

\[
\boxed{
\operatorname{ord}(s_p^{\rm raw})
=
e_{\rm exc}(E,p)
+
\operatorname{ord}(s_p^{\rm corr}).
}
\]

This is algebraic and does not invoke BSD.

## 3. Corrected interpolation defect

Define the signed corrected interpolation defect

\[
\boxed{
\eta_{E,p}
:=
r_{\rm an}(E)
-
\operatorname{ord}(s_p^{\rm corr}).
}
\]

Thus

\[
\operatorname{ord}(s_p^{\rm corr})
=
r_{\rm an}(E)-\eta_{E,p},
\]

and

\[
\boxed{
\operatorname{ord}(s_p^{\rm raw})
=
e_{\rm exc}(E,p)
+
r_{\rm an}(E)
-
\eta_{E,p}.
}
\]

The desired corrected complex-to-p-adic order registration is

\[
\boxed{\eta_{E,p}=0.}
\]

The exceptional-zero contribution \(e_{\rm exc}\) is not counted as a BSD rank defect after the declared local factor has been removed.

## 4. Combination with the determinant registration defect

Let \(s_{\rm ar}\) be the arithmetic/Selmer determinant section on the common rank-one carrier and define

\[
s_p^{\rm corr}
=
q_{E,p}\,s_{\rm ar},
\]

\[
\rho_{E,p}
:=
\operatorname{ord}(q_{E,p})
=
\operatorname{ord}(s_p^{\rm corr})
-
\operatorname{ord}(s_{\rm ar}).
\]

For the Smith/Selmer arithmetic side,

\[
\operatorname{ord}(s_{\rm ar})
=
r_p(E)
+
\sum_i d_i(E,p),
\]

with

\[
r_p(E)
=
r_{\rm MW}(E)+s_p(E).
\]

Substituting

\[
\operatorname{ord}(s_p^{\rm corr})
=
r_{\rm an}(E)-\eta_{E,p}
\]

gives

\[
\rho_{E,p}
=
r_{\rm an}
-
\eta_{E,p}
-
r_{\rm MW}
-
s_p
-
\sum_i d_i.
\]

Therefore

\[
\boxed{
r_{\rm an}(E)-r_{\rm MW}(E)
=
\eta_{E,p}
+
\rho_{E,p}
+
\sum_i d_i(E,p)
+
s_p(E).
}
\]

This is the **corrected four-defect normal form**.

## 5. Meaning of the four terms

### D2b — corrected interpolation defect

\[
\eta_{E,p}
=
r_{\rm an}
-
\operatorname{ord}(s_p^{\rm corr}).
\]

It measures failure of the corrected p-adic analytic section to carry the same central order as the complex L-germ.

It may have either sign until an independent comparison theorem is proved.

### D3 — determinant registration defect

\[
\rho_{E,p}
=
\operatorname{ord}(s_p^{\rm corr}/s_{\rm ar}).
\]

It measures mismatch between corrected p-adic analytic and arithmetic determinant sections.

### D4 — higher-contact spectrum

\[
d_i(E,p)\ge0.
\]

It measures higher-order persistence of already registered arithmetic zero modes.

### D6 — hidden arithmetic modes

\[
s_p(E)
=
\operatorname{corank}_{\mathbb Z_p}\Sha(E/\mathbb Q)[p^\infty]
\ge0.
\]

It measures Selmer directions not represented by the free Mordell--Weil group.

The local exceptional factor

\[
e_{\rm exc}(E,p)
\]

is tracked separately and removed before D2b.

## 6. Exceptional-zero sanity check

For a modular elliptic curve with split multiplicative reduction at \(p\), the interpolation property forces

\[
L_p(E,1)=0
\]

even when the complex central value need not vanish.

Greenberg--Stevens prove, for \(p\ge5\), the Mazur--Tate--Teitelbaum formula

\[
L_p'(E,1)
=
\mathcal L_p(E)
\frac{L(E,1)}{\Omega_E},
\]

with

\[
\mathcal L_p(E)
=
\frac{\log_p q_E}{\operatorname{ord}_p q_E}.
\]

This is direct evidence that a raw p-adic zero can contain a local interpolation contribution not representing Mordell--Weil rank.

The RZDP correction step is therefore mandatory, not cosmetic.

## 7. Higher and critical exceptional zeros

More general p-adic settings can contain higher or critical exceptional zeros and derived regulators.

Benois--Buyukboduk, for example, prove a p-adic BSD-type leading-term formula for a second derivative in a non-crystalline semistable setting, expressed through a cyclotomic p-adic regulator on an extended Selmer group.

Their later critical-p-adic-L-function theory develops thick Selmer complexes and leading-term formulas.

These results justify treating the exceptional/interpolation correction as a typed layer. They do not supply a universal all-elliptic-curves equality \(\eta=0\).

## 8. Main-conjecture layer remains distinct

Kato's Euler system and explicit reciprocity law connect p-adic zeta data to Selmer groups and prove a divisibility toward the Iwasawa main conjecture under stated hypotheses.

That attacks \(\rho\), not automatically \(\eta\).

Thus:

\[
\boxed{
\text{complex }L\text{-order}
\xrightarrow{\eta}
\text{corrected p-adic analytic order}
\xrightarrow{\rho}
\text{Selmer determinant order}
\xrightarrow{d_i}
\text{Selmer zero-mode count}
\xrightarrow{s_p}
\text{Mordell--Weil rank}.
}
\]

Every arrow has a separate proof obligation.

## 9. Closure criterion

After a valid local exceptional-factor normalization, the Route-S rank equality follows if

\[
\eta_{E,p}=0,
\qquad
\rho_{E,p}=0,
\qquad
d_i(E,p)=0\ \forall i,
\qquad
s_p(E)=0.
\]

The decomposition itself does not prove any of these vanishings.

## 10. A0 firewall

A0 is a support/zero-realization principle.

Multiplicity and its transfer require additional derived theorems about:

- interpolation order \(\eta\);
- determinant valuation \(\rho\);
- jet/contact spectrum \(d_i\);
- hidden arithmetic quotient \(s_p\).

No extra axiom is introduced. These remain explicit theorem gates.

## 11. Sources

- B. Mazur, J. Tate, J. Teitelbaum, *On p-adic analogues of the conjectures of Birch and Swinnerton-Dyer*, Invent. Math. 84 (1986), 1--48.
- R. Greenberg, G. Stevens, *p-adic L-functions and p-adic periods of modular forms*, Invent. Math. 111 (1993), 407--447.
- D. Benois, K. Buyukboduk, *On the exceptional zeros of p-non-ordinary p-adic L-functions and a conjecture of Perrin-Riou*, Trans. Amer. Math. Soc. 376 (2023), 231--284.
- D. Benois, K. Buyukboduk, *Arithmetic of Critical p-Adic L-Functions*, Memoirs AMS 321 (2026), no. 1635.
- K. Kato, *p-adic Hodge theory and values of zeta functions of modular forms*, Asterisque 295 (2004), 117--290.
