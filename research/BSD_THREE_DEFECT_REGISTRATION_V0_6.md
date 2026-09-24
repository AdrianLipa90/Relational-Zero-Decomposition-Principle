# BSD Three-Defect Registration Normal Form v0.6

Status: **EXACT RELATIVE-VALUATION ALGEBRA / CONDITIONAL BSD REGISTRATION / NO BSD PROMOTION**

Date: 2026-09-24

## 1. Purpose

The current two-obstruction form
\[
\delta_{\rm BSD}
=
\sum_i d_i+s_p
\]
already assumes that the analytic section and the Selmer determinant section have been identified up to a unit.

This file removes that hidden assumption and makes the registration mismatch itself an explicit third defect.

## 2. Common determinant line

Let \(R\) be a one-dimensional local domain or DVR with fraction field \(Q(R)\), and let
\[
\Delta
\]
be an invertible rank-one \(R\)-module.

Suppose two nonzero meromorphic sections
\[
s_{\rm an},s_{\rm ar}
\in
\Delta\otimes_RQ(R)
\]
represent the analytic and arithmetic determinant data on the same carrier.

There is a unique
\[
q\in Q(R)^\times
\]
such that
\[
s_{\rm an}=q\,s_{\rm ar}.
\]

Define the registration valuation
\[
\boxed{
\rho:=\operatorname{ord}(q)
=
\operatorname{ord}(s_{\rm an})
-
\operatorname{ord}(s_{\rm ar}).
}
\]

Then
\[
\boxed{
\rho=0
\iff
q\in R^\times.
}
\]

Thus “identified up to a unit” is exactly the vanishing of a measurable integer defect.

## 3. Arithmetic determinant multiplicity

For a registered two-term Selmer complex with Smith exponents
\[
a_i=1+d_i,
\qquad
d_i\ge0,
\]
one has
\[
\operatorname{ord}(s_{\rm ar})
=
r_p(E)+\sum_i d_i(E,p).
\]

The Selmer/Sha exact sequence gives
\[
r_p(E)=r_{\rm MW}(E)+s_p(E).
\]

Hence
\[
\operatorname{ord}(s_{\rm ar})
=
r_{\rm MW}(E)
+
s_p(E)
+
\sum_i d_i(E,p).
\]

## 4. Analytic registration

Assume only that the analytic section is normalized so that
\[
\operatorname{ord}(s_{\rm an})
=
r_{\rm an}(E).
\]

No equality with the arithmetic section is assumed.

By the definition of \(\rho\),
\[
r_{\rm an}
=
\rho
+
r_{\rm MW}
+
s_p
+
\sum_i d_i.
\]

Therefore
\[
\boxed{
\delta_{\rm BSD}(E)
:=
r_{\rm an}(E)-r_{\rm MW}(E)
=
\rho_{E,p}
+
\sum_i d_i(E,p)
+
s_p(E).
}
\]

This is the **three-defect registration normal form**.

## 5. Meaning of the three defects

### Registration defect
\[
\rho_{E,p}
=
\operatorname{ord}(s_{\rm an}/s_{\rm ar}).
\]

It measures mismatch between analytic and arithmetic trivializations of the common determinant line.

It can have either sign until an integrality/divisibility theorem is proved.

### Contact-depth defect
\[
d_i(E,p)=a_i-1\ge0.
\]

It measures higher-order persistence beyond a simple transverse zero mode.

### Hidden-arithmetic defect
\[
s_p(E)
=
\operatorname{corank}_{\mathbb Z_p}\Sha(E/\mathbb Q)[p^\infty]
\ge0.
\]

It counts divisible Selmer directions not represented by free Mordell--Weil points.

## 6. Main-conjecture interpretation

The equality form of an Iwasawa main conjecture identifies the analytic and arithmetic characteristic ideals.

In the rank-one determinant-line language this is exactly
\[
q\in R^\times,
\]
hence
\[
\boxed{\rho=0.}
\]

A one-sided divisibility gives a sign condition on \(\rho\), with the sign depending on the orientation chosen for \(q=s_{\rm an}/s_{\rm ar}\).

For the conventional orientation above, an ideal inclusion
\[
(s_{\rm an})\subseteq(s_{\rm ar})
\]
implies
\[
\rho\ge0.
\]

Kato's Euler-system work proves such divisibility statements toward the Iwasawa main conjecture under its stated hypotheses. Opposite-divisibility results in complementary settings close the valuation to zero.

Thus RZDP interprets the traditional “two divisibilities” strategy as two inequalities squeezing a single registration defect:
\[
\rho\ge0,
\qquad
\rho\le0
\quad\Longrightarrow\quad
\rho=0.
\]

## 7. BSD closure criterion

Once all three defects are known to be nonnegative, one has
\[
\delta_{\rm BSD}
=
\rho
+
\sum_i d_i
+
s_p
\ge0.
\]

If, moreover,
\[
\rho=0,
\qquad
d_i=0\ \forall i,
\qquad
s_p=0,
\]
then
\[
\delta_{\rm BSD}=0
\]
and the BSD rank equality follows.

Without a sign theorem for \(\rho\), cancellation between \(\rho\) and the two nonnegative defects is algebraically possible, so no Q.E.D. may be claimed from the decomposition alone.

## 8. Relation to the archimedean route

The three-defect form belongs to the p-adic/Selmer route.

The direct Neron--Tate route bypasses the Selmer/Sha split if one independently constructs a complex analytic determinant family whose kernel is the free Mordell--Weil space and whose crossing is the Neron--Tate height map.

The two routes are complementary but not identified.

## 9. Relational-zero interpretation

The BSD multiplicity problem is now decomposed into three distinct failures of exact relational registration:

\[
\boxed{
\text{analytic excess}
=
\text{registration mismatch}
+
\text{higher contact}
+
\text{hidden arithmetic modes}.
}
\]

This is finer than the raw equality
\[
r_{\rm an}=r_{\rm MW}.
\]

It also shows a structural limit of A0: a zero-locus principle can determine where a relational zero is supported, but it does not by itself determine the valuation of a relative determinant section, the jet/contact order of each zero mode, or the size of a hidden Selmer quotient.

No additional axiom is introduced here; these are explicit theorem obligations.

## 10. Sources

- K. Kato, *p-adic Hodge theory and values of zeta functions of modular forms*, Asterisque 295 (2004), 117--290: Euler-system bounds, explicit reciprocity, and a divisibility toward the Iwasawa main conjecture.
- Standard Iwasawa main-conjecture formulations identify a p-adic L-function principal ideal with a Selmer characteristic ideal; equality is the unit-ratio condition in the determinant-line language.
