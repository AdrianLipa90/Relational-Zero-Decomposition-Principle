# BSD Multiplicity/Index Decomposition v0.1

Status: **EXACT REDUCTIONS / PARITY SEAM CLOSED / INTEGER LIFT OPEN**

Date: 2026-09-24

## 1. Clay target

For an elliptic curve \(E/\mathbb Q\), the Millennium Prize rank statement is

\[
r_{\mathrm{an}}(E):=\operatorname{ord}_{s=1}L(E,s)
=
\operatorname{rank}_{\mathbb Z}E(\mathbb Q)
=:r_{\mathrm{MW}}(E).
\]

Clay still lists the Birch--Swinnerton-Dyer conjecture as unsolved. The official problem description states that the Taylor expansion at \(s=1\) should begin with a nonzero coefficient in degree \(r=\operatorname{rank}E(\mathbb Q)\).

## 2. Exact analytic index triad

Set

\[
L_E(z):=L(E,1+z).
\]

Let \(r=r_{\mathrm{an}}(E)\). Since \(L_E\) is holomorphic near \(0\) and is not identically zero, there is a unit \(u(z)\) with \(u(0)\neq0\) such that

\[
L_E(z)=z^r u(z).
\]

Hence three integers coincide exactly:

\[
\boxed{
r_{\mathrm{an}}(E)
=
\operatorname{ord}_{z=0}L_E(z)
=
\operatorname{wind}_0\!\left(L_E(\varepsilon e^{i\theta})\right)
=
\operatorname{length}_{\mathbb C\{z\}}
\frac{\mathbb C\{z\}}{(L_E)}
}
\]

for sufficiently small \(\varepsilon>0\) containing no other zero.

The winding equality is the argument principle:

\[
r_{\mathrm{an}}(E)
=
\frac{1}{2\pi i}
\oint_{|z|=\varepsilon}
\frac{L_E'(z)}{L_E(z)}\,dz.
\]

The local-algebra equality follows because multiplication by the unit \(u\) does not change the principal ideal:

\[
(L_E)=(z^r),
\qquad
\mathbb C\{z\}/(L_E)
\cong
\mathbb C\{z\}/(z^r),
\]

whose complex length is \(r\).

This part is standard local complex analysis/algebra and requires no BSD assumption.

## 3. Exact arithmetic index

Define

\[
V_E:=E(\mathbb Q)\otimes_{\mathbb Z}\mathbb Q.
\]

By Mordell--Weil, \(V_E\) is finite dimensional and

\[
r_{\mathrm{MW}}(E)=\dim_{\mathbb Q}V_E.
\]

For any finite-dimensional vector space,

\[
\boxed{
\dim V_E
=
\max\{k\ge0:\Lambda^k V_E\neq0\}.
}
\]

Therefore BSD is exactly equivalent to the equality of the two independently defined integer indices

\[
\boxed{
\operatorname{length}_{\mathbb C\{z\}}
\frac{\mathbb C\{z\}}{(L_E)}
=
\max\{k:\Lambda^k(E(\mathbb Q)\otimes\mathbb Q)\neq0\}.
}
\]

This is the RZDP multiplicity/index normal form.

## 4. Closed parity seam

Let \(r_p(E)\) be the \(\mathbb Z_p\)-corank of the \(p^\infty\)-Selmer group. Dokchitser--Dokchitser prove for elliptic curves over \(\mathbb Q\) and every prime \(p\) that

\[
\boxed{
r_{\mathrm{an}}(E)\equiv r_p(E)\pmod2.
}
\]

Thus the analytic winding multiplicity and the arithmetic Selmer index are already identified modulo two.

This is a genuine theorem-level seam. It does **not** give the integer equality required by BSD.

## 5. Selmer/Sha decomposition

The standard Kummer/Selmer formalism gives an exact sequence whose rationalized form may be written schematically as

\[
0\to E(\mathbb Q)\otimes\mathbb Q_p
\to H^1_f(\mathbb Q,V_p(E))
\to V_p\Sha(E/\mathbb Q)
\to0.
\]

Accordingly,

\[
\dim_{\mathbb Q_p}H^1_f(\mathbb Q,V_p(E))
=
r_{\mathrm{MW}}(E)
+
\operatorname{corank}_{\mathbb Z_p}\Sha(E/\mathbb Q)[p^\infty].
\]

This identifies a second obstruction: a Selmer index need not equal the Mordell--Weil rank unless the Tate--Shafarevich contribution is controlled.

## 6. Integer-lift problem

The unresolved RZDP gate is therefore not “find a parity relation”. That seam is already closed.

The missing theorem must lift the known \(\mathbb Z/2\mathbb Z\) information to the full non-negative integer multiplicity while simultaneously landing on the Mordell--Weil side:

\[
\boxed{
\operatorname{wind}(L_E)
\quad\xrightarrow{\text{INTEGER LIFT}}\quad
\dim_{\mathbb Q}E(\mathbb Q)\otimes\mathbb Q.
}
\]

A non-circular proof must construct this lift from independently established arithmetic/analytic structure. Merely defining an index to equal either side is forbidden.

## 7. Candidate bridge object

A natural candidate is a Selmer-complex/determinant-line object equipped with two independent comparison theorems:

1. **analytic comparison:** its derived/determinant order is the local analytic length of the \(L\)-germ at \(s=1\);
2. **arithmetic comparison:** the same index reduces to the Mordell--Weil dimension, with the Tate--Shafarevich contribution explicitly controlled.

Modern higher-rank Euler/Kolyvagin/Stark systems, exterior-power biduals, Selmer complexes, height regulators, and derived Bockstein regulators are precisely in this structural neighborhood. They provide the correct language, but no source checked here supplies the missing all-curves comparison theorem.

## 8. Internal Fredholm seam firewall

The existing Infinities/PNCS FSI.05 theorem

\[
\operatorname{rank}(I-U^kU^{*k})=k,
\qquad
\operatorname{ind}(U^k)=-k
\]

is exact and useful as an integer-index model.

However, there is currently **no canonical map** in the project from

\[
L(E,s)\text{ germ / Selmer complex / }E(\mathbb Q)
\]

to that unilateral-shift operator preserving the relevant arithmetic data.

Therefore FSI.05 supplies an index grammar, not the BSD integer lift.

## 9. Minimal current proof obligation

The shortest non-circular target is:

> **RZDP-BSD Integer-Lift Theorem.** Construct, for every elliptic curve \(E/\mathbb Q\), a canonical arithmetic-analytic index object \(\mathcal I_E\) and prove independently that
>
> \[
> \mathcal I_E
> =
> \operatorname{length}_{\mathbb C\{z\}}
> \mathbb C\{z\}/(L(E,1+z))
> \]
>
> and
>
> \[
> \mathcal I_E
> =
> \dim_{\mathbb Q}(E(\mathbb Q)\otimes\mathbb Q).
> \]

Once both comparison theorems are closed, BSD rank equality follows immediately.

Current status: **OPEN_BRIDGE**.

## 10. Provenance / sources

Primary external anchors used for this reduction:

- Andrew Wiles, official Clay problem description, *The Birch and Swinnerton-Dyer Conjecture*.
- Tim Dokchitser and Vladimir Dokchitser, *On the Birch-Swinnerton-Dyer quotients modulo squares*, Annals of Mathematics 172 (2010), including the \(p\)-parity theorem over \(\mathbb Q\).
- Jan Nekovař, *Selmer complexes*, Astérisque 310, for the Bloch--Kato/Selmer-complex formulation and the Tate--Shafarevich correction.
- Mazur--Rubin and later higher-rank Euler/Kolyvagin/Stark-system work for exterior-power arithmetic control.

Internal source:

- PhaseNav-Natural-Coding-System, FSI.05, pinned seam from Infinities unilateral-shift Fredholm index to countable successor order; firewall preserved.
