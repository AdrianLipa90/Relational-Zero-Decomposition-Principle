# BSD Selmer-Complex / Bockstein Crossing Crosswalk v0.3

Status: **EXACT LOCAL-ALGEBRA CROSSWALK / STANDARD SELMER-COMPLEX INTERPRETATION WITH HYPOTHESES / BSD STILL OPEN**

Date: 2026-09-24

## 1. Two-term perfect-complex model

Let
\[
R=K[[T]]
\]
for a characteristic-zero field \(K\), and let a perfect complex of amplitude \([1,2]\) and Euler characteristic zero be represented locally by

\[
C_R:\qquad
R^n\xrightarrow{A(T)}R^n.
\]

After specialization at the augmentation \(T=0\),

\[
C_0=C_R\otimes_R K
\]

has

\[
H^1(C_0)=\ker A(0),
\qquad
H^2(C_0)=\operatorname{coker}A(0).
\]

The determinant/characteristic element of this presentation is represented by

\[
\det A(T).
\]

## 2. Bockstein equals the derivative crossing

The short exact sequence

\[
0\to R\xrightarrow{\,T\,}R\to K\to0
\]

induces the Bockstein connecting morphism

\[
\beta_C:
H^1(C_0)
\longrightarrow
H^2(C_0)\otimes_K (T)/(T^2).
\]

For the two-term presentation above, identify \((T)/(T^2)\cong K\,dT\). Then

\[
\boxed{
\beta_C
=
q\circ A'(0)|_{\ker A(0)}
}
\]

up to the conventional choice of generator/sign for \((T)/(T^2)\).

Thus the Bockstein differential is the cohomological version of the crossing map in the Relational Multiplicity-Index Transfer Lemma.

## 3. Bockstein Multiplicity Theorem

If

\[
\beta_C:
H^1(C_0)\to H^2(C_0)
\]

is an isomorphism, then the transfer lemma gives

\[
\boxed{
\operatorname{ord}_{T=0}\det A(T)
=
\dim_K H^1(C_0)
=
\dim_K H^2(C_0).
}
\]

This is an exact local-algebra statement.

Equivalently, a nondegenerate first Bockstein converts the order of the determinant zero into the dimension of the specialized cohomological zero-mode space.

## 4. Arithmetic interpretation

In Nekovar-style self-dual Selmer-complex formalisms, the Bockstein map associated to an infinitesimal cyclotomic deformation is the input from which the p-adic height pairing is constructed. Modern treatments explicitly use these Bockstein maps to obtain regulator and leading-term formulas.

Therefore, under the hypotheses needed for the relevant Selmer complex and self-duality identifications, RZDP gate B3 has the arithmetic interpretation

\[
\boxed{
\text{B3 transversality}
\longleftrightarrow
\text{nondegenerate Bockstein / p-adic height regulator}.
}
\]

This is a structural crosswalk, not a universal nondegeneracy theorem.

## 5. Refined BSD chain

The determinant/Selmer route should therefore be audited as a chain of separate gates:

\[
\text{complex }L\text{-germ}
\longrightarrow
\text{p-adic / zeta determinant element}
\longrightarrow
\det C_R
\longrightarrow
\text{Bockstein regulator}
\longrightarrow
\text{Selmer rank}
\longrightarrow
\text{Mordell-Weil rank}.
\]

Typed obligations:

- **C1 — analytic registration:** relate the relevant determinant/zeta element to the complex central L-germ, with exceptional-zero issues made explicit;
- **C2 — determinant/main-conjecture registration:** identify the analytic p-adic/zeta element with the determinant/characteristic element of the Selmer complex;
- **C3 — Bockstein nondegeneracy:** prove the first nonzero derived regulator is nondegenerate;
- **C4 — specialization/control:** identify specialized Selmer cohomology and control finite kernel/cokernel terms;
- **C5 — Sha-divisible control:** remove the residual \(V_p\Sha\) / \(p^\infty\)-divisible obstruction needed to land on Mordell-Weil rank.

No one of C1--C5 may be replaced by a definition that already encodes BSD.

## 6. Relation to recent literature

The determinant/Bockstein direction is an active standard research direction, not a blank area.

Benois--Buyukboduk develop thick Selmer complexes, Bockstein morphisms, fundamental lines, and leading-term formulas for critical p-adic L-functions.

Burns--Kurihara--Sano develop Bockstein regulators, determinantal zeta elements, and algebraic BSD elements in refined settings.

A May 2026 preprint titled *Bockstein Determinants and Birch--Swinnerton-Dyer* also pursues determinant-line/Bockstein criteria and explicitly leaves the uniform construction/reciprocity/specialization problem as the principal burden. It is treated here as related preprint evidence, not theorem authority.

This literature audit means that novelty cannot be claimed merely for using determinant lines or Bockstein derivatives. Any RZDP novelty must lie in a new independently proved comparison or closure theorem.

## 7. Consequence for RZDP

The useful new compression is:

\[
\boxed{
\text{multiplicity}
=
\text{zero-mode dimension}
}
\]

whenever the Bockstein/crossing is nondegenerate.

For BSD, the unresolved content has now been isolated away from this local mechanism and into the global arithmetic-analytic registration and Sha/control gates.
