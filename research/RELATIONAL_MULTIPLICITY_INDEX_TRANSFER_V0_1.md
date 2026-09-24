# Relational Multiplicity-Index Transfer Lemma v0.1

Status: **THEOREM / BSD OPERATOR CRITERION CONDITIONAL / NO BSD PROMOTION**

Date: 2026-09-24

## 1. Setup

Let

\[
A(z):\mathbb C^n\to\mathbb C^n
\]

be holomorphic near \(z=0\). Put

\[
A_0=A(0),\qquad A_1=A'(0),
\]

\[
K=\ker A_0,\qquad
C=\operatorname{coker}A_0.
\]

Since domain and codomain have equal finite dimension,

\[
\dim K=\dim C=:r.
\]

Let \(q:\mathbb C^n\to C\) be the quotient map and define the crossing map

\[
\Gamma_A=q\circ A_1|_K:K\to C.
\]

## 2. Multiplicity-Index Transfer Lemma

**Theorem.** If \(\Gamma_A\) is an isomorphism, then

\[
\boxed{
\operatorname{ord}_{z=0}\det A(z)
=
r
=
\dim\ker A(0).
}
\]

Thus a transverse zero-mode crossing forces determinant multiplicity to equal the dimension of the zero-mode space.

## 3. Proof

Choose a domain complement \(X\) and a codomain complement \(\widetilde C\):

\[
\mathbb C^n=K\oplus X,
\qquad
\mathbb C^n=\widetilde C\oplus Y,
\qquad
Y=\operatorname{im}A_0,
\]

where the quotient map identifies \(\widetilde C\cong C=\operatorname{coker}A_0\).

In these decompositions write

\[
A(z)=
\begin{pmatrix}
a(z)&b(z)\\
c(z)&d(z)
\end{pmatrix}.
\]

At \(z=0\),

\[
a(0)=b(0)=c(0)=0,
\]

and

\[
d(0):X\to Y
\]

is an isomorphism. Hence \(d(z)\) is invertible for sufficiently small \(z\).

By the Schur-complement formula,

\[
\det A(z)
=
\det d(z)\,
\det\!\left(
a(z)-b(z)d(z)^{-1}c(z)
\right).
\]

Because \(b(0)=c(0)=0\),

\[
b(z)d(z)^{-1}c(z)=O(z^2),
\]

while

\[
a(z)=z\,a'(0)+O(z^2).
\]

Under the chosen identifications \(a'(0)=\Gamma_A\). Therefore

\[
a(z)-b(z)d(z)^{-1}c(z)
=
z\bigl(\Gamma_A+O(z)\bigr).
\]

If \(\Gamma_A\) is invertible, then

\[
\det A(z)
=
z^r u(z),
\qquad
u(0)\neq0.
\]

Hence

\[
\operatorname{ord}_0\det A=r.
\]

Q.E.D.

## 4. BSD operator criterion

Set

\[
L_E(z)=L(E,1+z).
\]

Suppose that for every elliptic curve \(E/\mathbb Q\) one constructs a holomorphic matrix family \(A_E(z)\) satisfying independently:

### B1 — analytic determinant comparison

There is a holomorphic unit \(u_E(0)\neq0\) such that

\[
\boxed{
\det A_E(z)=u_E(z)L_E(z).
}
\]

### B2 — arithmetic zero-mode identification

There is a canonical isomorphism

\[
\boxed{
\ker A_E(0)
\cong
E(\mathbb Q)\otimes_{\mathbb Z}\mathbb C.
}
\]

### B3 — relational transversality

The crossing map

\[
\Gamma_{A_E}:
\ker A_E(0)\to\operatorname{coker}A_E(0)
\]

is an isomorphism.

Then

\[
\operatorname{ord}_{s=1}L(E,s)
=
\dim\ker A_E(0)
=
\operatorname{rank}E(\mathbb Q),
\]

so

\[
\boxed{
(B1)+(B2)+(B3)
\Longrightarrow
\mathrm{BSD}_{\rm rank}.
}
\]

This implication is exact. It is not a proof of BSD until \(A_E\) is constructed non-circularly.

## 5. Determinant-line relation

The Bloch-Kato / Fontaine-Perrin-Riou / Tamagawa-number framework already uses determinants of perfect Galois-cohomology/Selmer complexes to connect analytic L-data with arithmetic cohomology.

That makes determinant/Selmer complexes the canonical standard candidate class for \(A_E\)-type data, but it is not a shortcut: the universal comparison required to close B1-B3 is part of the still-open BSD/Bloch-Kato/Tamagawa-number picture.

## 6. Project firewall

The existing Infinities/PNCS unilateral-shift Fredholm theorem supplies an exact integer-index grammar. There is currently no canonical elliptic-curve map

\[
E\mapsto A_E
\]

to that shift model preserving both the L-germ and Mordell-Weil data. Therefore the shift theorem cannot be used as B1 or B2.

## 7. Current frontier

The vague integer-lift problem is now replaced by three typed obligations:

\[
\boxed{
\mathrm{B1}:\text{ determinant carries the L-germ},
}
\]

\[
\boxed{
\mathrm{B2}:\text{ zero modes carry Mordell-Weil},
}
\]

\[
\boxed{
\mathrm{B3}:\text{ crossing is nondegenerate}.
}
\]

The next audit should search determinant-line/Selmer-complex constructions for B1 and B2 separately; B3 is then a concrete transversality theorem.
