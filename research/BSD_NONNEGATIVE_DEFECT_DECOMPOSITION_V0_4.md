# BSD Nonnegative Defect Decomposition v0.4

Status: **LOCAL MULTIPLICITY THEOREM / CONDITIONAL BSD REGISTRATION / BSD STILL OPEN**

Date: 2026-09-24

## 1. Multiplicity lower bound

Let
\[
A(z):\mathbb C^n\to\mathbb C^n
\]
be holomorphic near \(z=0\), assume \(\det A\) is not identically zero, and put
\[
r:=\dim\ker A(0)=\dim\operatorname{coker}A(0).
\]

Choose complements as in the Multiplicity--Index Transfer Lemma and write
\[
A(z)=
\begin{pmatrix}
a(z)&b(z)\\
c(z)&d(z)
\end{pmatrix},
\]
with \(d(0)\) invertible and \(a(0)=b(0)=c(0)=0\).

The Schur complement
\[
S(z):=a(z)-b(z)d(z)^{-1}c(z)
\]
is an \(r\times r\) matrix satisfying
\[
S(z)=z\Gamma_A+O(z^2),
\]
where
\[
\Gamma_A:
\ker A(0)\to\operatorname{coker}A(0)
\]
is the crossing map induced by \(A'(0)\).

Since every entry of \(S(z)\) is divisible by \(z\),
\[
\det S(z)
\]
is divisible by \(z^r\). Therefore
\[
\boxed{
\operatorname{ord}_{z=0}\det A(z)\ge r.
}
\]

Moreover, the coefficient of \(z^r\) is
\[
\det d(0)\det\Gamma_A.
\]
Hence
\[
\boxed{
\operatorname{ord}_{z=0}\det A(z)=r
\iff
\Gamma_A\text{ is an isomorphism}.
}
\]

This strengthens the earlier transfer lemma.

## 2. Multiplicity excess

Define
\[
\varepsilon(A)
:=
\operatorname{ord}_{z=0}\det A(z)
-
\dim\ker A(0).
\]

Then
\[
\boxed{
\varepsilon(A)\in\mathbb Z_{\ge0}
}
\]
and
\[
\boxed{
\varepsilon(A)=0
\iff
\Gamma_A\text{ is an isomorphism}.
}
\]

Thus failure of first-order transversality is measured by an exact nonnegative excess multiplicity.

## 3. Perfect-complex / Bockstein form

Let
\[
R=K[[T]]
\]
and let a two-term perfect complex of Euler characteristic zero be represented by
\[
C_R:
\qquad
R^n\xrightarrow{A(T)}R^n.
\]

At augmentation,
\[
H^1(C_0)=\ker A(0),
\qquad
H^2(C_0)=\operatorname{coker}A(0).
\]

The augmentation Bockstein is
\[
\beta_C=qA'(0)|_{\ker A(0)}
\]
up to the conventional generator/sign of \((T)/(T^2)\).

Therefore
\[
\boxed{
\varepsilon(C_R)
:=
\operatorname{ord}_{T=0}\det A(T)
-
\dim_K H^1(C_0)
\ge0,
}
\]
with
\[
\boxed{
\varepsilon(C_R)=0
\iff
\beta_C\text{ is an isomorphism}.
}
\]

This is an exact local-algebra theorem.

## 4. Conditional BSD registration

Suppose a Selmer/deformation complex \(C_{E,p}\) is constructed and the still-open global registration gates establish

\[
\operatorname{ord}_{T=0}\det C_{E,p}
=
r_{\rm an}(E)
\]
and
\[
\dim H^1(C_{E,p}\otimes_R K)
=
r_p(E),
\]
where
\[
r_p(E)
=
\operatorname{corank}_{\mathbb Z_p}
\operatorname{Sel}_{p^\infty}(E/\mathbb Q).
\]

Then the exact local theorem gives
\[
\boxed{
\varepsilon_{E,p}
:=
r_{\rm an}(E)-r_p(E)
\ge0.
}
\]

By the known parity theorem,
\[
r_{\rm an}(E)-r_p(E)
\]
is even. Hence
\[
\boxed{
\varepsilon_{E,p}=2k_p(E)\in2\mathbb Z_{\ge0}.
}
\]

This nonnegativity is **conditional on the analytic/determinant and specialization registrations**. Those registrations are not yet universal theorems.

## 5. Nonnegative BSD defect decomposition

The standard Selmer/Sha exact sequence gives
\[
r_p(E)=r_{\rm MW}(E)+s_p(E),
\]
where
\[
s_p(E)
=
\operatorname{corank}_{\mathbb Z_p}
\Sha(E/\mathbb Q)[p^\infty]
\ge0.
\]

Under the registrations of Section 4,
\[
\begin{aligned}
r_{\rm an}(E)-r_{\rm MW}(E)
&=
\bigl(r_{\rm an}(E)-r_p(E)\bigr)
+
\bigl(r_p(E)-r_{\rm MW}(E)\bigr)\\
&=
\varepsilon_{E,p}+s_p(E).
\end{aligned}
\]

Thus
\[
\boxed{
\delta_{\rm BSD}(E)
=
\varepsilon_{E,p}+s_p(E),
\qquad
\varepsilon_{E,p}\ge0,
\quad
s_p(E)\ge0.
}
\]

Consequently, under the same registration hypotheses,
\[
\boxed{
\mathrm{BSD}_{\rm rank}
\iff
\varepsilon_{E,p}=0
\ \text{and}\
s_p(E)=0.
}
\]

Equivalently:
- the Bockstein/crossing must be nondegenerate;
- the divisible \(p\)-primary Tate--Shafarevich obstruction must vanish.

## 6. Determinant-line common carrier

The natural rank-one carrier is the determinant line of the relevant Selmer complex,
\[
\Delta_{E,p}:=\operatorname{Det}_R^{-1}C_{E,p},
\]
together with the standard local/archimedean factors required by the chosen formulation.

For any invertible rank-one \(R\)-module \(\Delta\) and two nonzero meromorphic sections
\[
s_1,s_2\in\Delta\otimes_R\operatorname{Frac}(R),
\]
there is a unique
\[
q\in\operatorname{Frac}(R)^\times
\]
such that
\[
s_1=q,s_2.
\]

The difference of their augmentation orders is exactly
\[
\boxed{
\operatorname{ord}_I(s_1)-\operatorname{ord}_I(s_2)
=
\operatorname{ord}_I(q).
}
\]

Thus equality of multiplicities is equivalent to the relative trivialization ratio being an \(R\)-unit.

Recent work of Macias Castillo and Sano (2026) proves, under mild hypotheses, that the determinant of a Nekovar Selmer complex is canonically isomorphic to the corresponding module of Stark systems. This confirms that the determinant line is a canonical arithmetic carrier rather than an RZDP-invented object.

What remains open for the universal BSD application is the analytic registration of the complex central \(L\)-germ/zeta element on this carrier and the global control needed to identify the specialized arithmetic zero modes with the desired rank.

## 7. Sharpened gate structure

The BSD branch is therefore reduced to the following typed chain:

- **D1 — carrier existence:** determinant/Selmer line and arithmetic Stark-system realization — standard/canonical under stated hypotheses;
- **D2 — analytic registration:** complex central \(L\)-germ to zeta/determinant section — OPEN;
- **D3 — determinant/Selmer comparison:** identify the analytic section with the Selmer determinant section up to controlled unit — OPEN in universal BSD generality;
- **D4 — Bockstein excess:** local theorem gives \(\varepsilon\ge0\); equality is exactly nondegenerate Bockstein — local theorem exact, universal nondegeneracy OPEN;
- **D5 — specialization:** identify specialized \(H^1\) with the relevant Selmer corank — hypothesis/control dependent;
- **D6 — Sha-divisible control:** prove \(s_p=0\) or otherwise close the exact total defect — OPEN.

No Q.E.D. is promoted.

## 8. Main structural consequence

Once D2, D3 and D5 register the global arithmetic object correctly, the remaining BSD defect is no longer signed or opaque:

\[
\boxed{
\delta_{\rm BSD}
=
\underbrace{\varepsilon_{\rm Bockstein}}_{\ge0}
+
\underbrace{s_p}_{\ge0}.
}
\]

This is the strongest current RZDP BSD normal form.
