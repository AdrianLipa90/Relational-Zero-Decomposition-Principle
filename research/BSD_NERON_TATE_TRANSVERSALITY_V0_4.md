# BSD Neron--Tate Transversality and Two-Realization Split v0.4

Status: **STANDARD HEIGHT THEOREM / CONDITIONAL CROSSING IDENTIFICATION / RANK-ONE SANITY CHECK / BSD STILL OPEN**

Date: 2026-09-24

## 1. Arithmetic zero-mode geometry

Let
\[
V_E^{\mathbb R}
:=
(E(\mathbb Q)/E(\mathbb Q)_{\rm tors})
\otimes_{\mathbb Z}\mathbb R.
\]

The Neron--Tate canonical height induces a positive-definite quadratic form
\[
\widehat h_E:V_E^{\mathbb R}\to\mathbb R_{\ge0}.
\]

Its associated symmetric bilinear pairing
\[
\langle P,Q\rangle_{\rm NT}
=
\frac12\bigl(
\widehat h_E(P+Q)-\widehat h_E(P)-\widehat h_E(Q)
\bigr)
\]
is nondegenerate. Hence
\[
H_{\rm NT}:V_E^{\mathbb R}\to(V_E^{\mathbb R})^*,
\qquad
P\mapsto\langle P,\cdot\rangle_{\rm NT}
\]
is an isomorphism.

Equivalently, for a basis \(P_1,\ldots,P_r\) of the free Mordell--Weil lattice,
\[
\boxed{
\operatorname{Reg}_{\rm NT}(E)
=
\det(\langle P_i,P_j\rangle_{\rm NT})
>0.
}
\]

This is standard arithmetic geometry and does not assume BSD.

## 2. Direct archimedean crossing criterion

Suppose one constructs a holomorphic square family
\[
A_E(z)
\]
with canonical identifications
\[
\ker A_E(0)
\cong
V_E^{\mathbb R}\otimes_{\mathbb R}\mathbb C
\]
and
\[
\operatorname{coker}A_E(0)
\cong
(V_E^{\mathbb R})^*\otimes_{\mathbb R}\mathbb C.
\]

If, independently of BSD,
\[
\boxed{
\Gamma_{A_E}
=
H_{\rm NT}\otimes_{\mathbb R}\mathbb C
}
\]
under these identifications, then \(\Gamma_{A_E}\) is automatically an isomorphism.

Therefore the Multiplicity--Index Transfer theorem gives
\[
\operatorname{ord}_0\det A_E
=
\operatorname{rank}E(\mathbb Q).
\]

If in addition
\[
\det A_E(z)=u_E(z)L(E,1+z),
\qquad
u_E(0)\neq0,
\]
then BSD rank equality follows.

Thus the direct archimedean route has three gates:
\[
\boxed{
\text{complex L-germ registration}
+
\text{Mordell--Weil kernel identification}
+
\text{crossing = Neron--Tate height}.
}
\]

The nondegeneracy itself is already standard.

## 3. This is not the Selmer/Bockstein route

The direct Neron--Tate route must not be conflated with the p-adic Selmer-complex route.

For the latter, the specialized cohomological dimension is
\[
r_p(E)
=
r_{\rm MW}(E)+s_p(E),
\]
where
\[
s_p(E)
=
\operatorname{corank}_{\mathbb Z_p}\Sha(E/\mathbb Q)[p^\infty].
\]

The cyclotomic Bockstein naturally produces p-adic height data on the Selmer side. Neron--Tate positivity on the Mordell--Weil quotient does not, by itself, prove nondegeneracy on additional divisible Sha directions.

Therefore RZDP retains two distinct strategies:

### Route A -- archimedean / Mordell--Weil direct
\[
L_E
\to
A_E
\to
\ker A_E(0)=V_E
\to
\Gamma_{A_E}=H_{\rm NT}.
\]

If every arrow is independently constructed, BSD rank follows directly.

### Route S -- p-adic / Selmer determinant
\[
L_E
\to
\text{zeta/determinant section}
\to
C_{E,p}
\to
\text{Bockstein}
\to
r_p
\to
r_{\rm MW}+s_p.
\]

After global registration this gives
\[
\delta_{\rm BSD}
=
\varepsilon_{E,p}+s_p,
\]
with both terms nonnegative.

No step in Route A is allowed to erase the explicit Sha obstruction in Route S.

## 4. Rank-one sanity check: Gross--Zagier--Kolyvagin

The archimedean derivative/height mechanism is not invented by RZDP.

In the Gross--Zagier setting, a first central derivative of an appropriate elliptic/modular L-function is, up to an explicit nonzero factor, the Neron--Tate height of a Heegner point:
\[
L'(1)\doteq\langle P,P\rangle_{\rm NT}.
\]

Consequently, nonzero first derivative forces a non-torsion arithmetic point. Kolyvagin's Euler-system results then control the Mordell--Weil rank and Tate--Shafarevich group. In particular, the BSD rank equality is known for elliptic curves over \(\mathbb Q\) of analytic rank at most one.

Thus rank one realizes the schematic chain
\[
\boxed{
\text{simple analytic zero}
\leftrightarrow
\text{nonzero height}
\leftrightarrow
\text{one arithmetic zero mode}.
}
\]

This is a strong consistency check for the RZDP archimedean route. It is not a proof for higher rank.

## 5. Smith-contact interpretation

For a local determinant family with Smith exponents
\[
a_i\ge0,
\]
simple crossing means
\[
a_i=1
\]
on every zero-mode channel.

If the direct crossing is Neron--Tate, its nondegeneracy forces precisely this simple-contact condition on the Mordell--Weil channels:
\[
d_i:=a_i-1=0.
\]

Therefore the direct height route can be read as a theorem that eliminates higher contact depth once the crossing-height identification is established.

## 6. Relational-zero interpretation

The canonical height itself is a faithful positive arithmetic defect on the real free Mordell--Weil space:
\[
D_{\rm NT}(P):=\widehat h_E(P)\ge0,
\]
with
\[
D_{\rm NT}(P)=0
\iff
P=0
\quad
\text{in }V_E^{\mathbb R}.
\]

This supplies a genuine arithmetic realization of relational zero. What remains unresolved is the global registration of the analytic zero germ with this arithmetic geometry.

## 7. Firewall

The conjectural BSD leading-coefficient formula already contains the Neron--Tate regulator. Therefore the crossing-height identity cannot be inferred merely from the fact that the same regulator appears in BSD.

The comparison map must be constructed independently.

Likewise, the p-adic Bockstein height and the archimedean Neron--Tate height are not silently identified.

## 8. Sources and project provenance

Standard sources:
- J. H. Silverman, *The Arithmetic of Elliptic Curves*, 2nd ed., Springer, 2009, for the canonical height and Neron--Tate pairing.
- B. Gross and D. Zagier, *Heegner points and derivatives of L-series*, Invent. Math. 84 (1986), 225--320.
- V. A. Kolyvagin, *Finiteness of E(Q) and Sha(E,Q) for a subclass of Weil curves*, Math. USSR-Izv. 32 (1989), 523--541.

Project search:
- No pre-existing AdrianLipa90 repository theorem was found for a Neron--Tate/canonical-height BSD bridge.
- This file is therefore a new RZDP reduction, not a relabeling of an existing project result.
