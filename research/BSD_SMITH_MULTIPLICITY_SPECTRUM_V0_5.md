# BSD Smith-Normal Multiplicity Spectrum v0.5

Status: **THEOREM / CONDITIONAL BSD REGISTRATION / NO BSD PROMOTION**

Date: 2026-09-24

## 1. Local DVR setup

Let
\[
R=K[[T]]
\]
with \(K\) a characteristic-zero field, and let
\[
A(T)\in M_n(R)
\]
satisfy
\[
\det A(T)\neq0.
\]

Because \(R\) is a discrete valuation ring, there exist
\[
U(T),V(T)\in GL_n(R)
\]
and integers
\[
a_1,\ldots,a_r\ge1
\]
such that
\[
U(T)A(T)V(T)
=
\operatorname{diag}
\bigl(
T^{a_1},\ldots,T^{a_r},1,\ldots,1
\bigr).
\]

The multiset
\[
\{a_1,\ldots,a_r\}
\]
is the local multiplicity spectrum of the zero modes.

## 2. Exact multiplicity decomposition

At \(T=0\), precisely the first \(r\) invariant factors vanish. Hence
\[
\boxed{
\dim_K\ker A(0)=r.
}
\]

On the other hand,
\[
\det A(T)
=
u(T)T^{a_1+\cdots+a_r},
\qquad
u(0)\neq0,
\]
so
\[
\boxed{
\operatorname{ord}_{T=0}\det A(T)
=
\sum_{i=1}^r a_i.
}
\]

Therefore the multiplicity excess is exactly
\[
\boxed{
\varepsilon(A)
=
\operatorname{ord}_{T=0}\det A(T)-\dim\ker A(0)
=
\sum_{i=1}^r(a_i-1).
}
\]

Every summand is nonnegative.

## 3. Transversality criterion

The first crossing/Bockstein is invertible exactly when every zero-mode invariant factor is simple:
\[
a_1=\cdots=a_r=1.
\]

Equivalently,
\[
\boxed{
\varepsilon(A)=0
\iff
a_i=1\ \forall i
\iff
\Gamma_A\text{ is an isomorphism}.
}
\]

Thus the excess multiplicity is not an opaque scalar. It is the total higher-contact depth of the zero modes.

Define
\[
d_i:=a_i-1\in\mathbb Z_{\ge0}.
\]

Then
\[
\boxed{
\varepsilon(A)=\sum_i d_i.
}
\]

The numbers \(d_i\) measure how many orders beyond a simple transverse crossing each zero mode persists.

## 4. Perfect-complex interpretation

For a two-term perfect complex
\[
C_R:
R^n\xrightarrow{A(T)}R^n,
\]
the same invariant factors give
\[
\dim H^1(C_0)=r
\]
and
\[
\operatorname{ord}_{T=0}\det C_R
=
\sum_i a_i.
\]

Hence
\[
\boxed{
\operatorname{ord}_{T=0}\det C_R
=
\dim H^1(C_0)
+
\sum_i d_i.
}
\]

This is the exact local multiplicity decomposition.

## 5. Conditional BSD registration

Assume the global BSD registration gates identify
\[
\operatorname{ord}_{T=0}\det C_{E,p}
=
r_{\rm an}(E)
\]
and
\[
\dim H^1(C_{E,p}\otimes_RK)
=
r_p(E).
\]

Then the Smith spectrum of the registered Selmer complex gives
\[
\boxed{
r_{\rm an}(E)
=
r_p(E)
+
\sum_{i=1}^{r_p(E)}d_i(E,p).
}
\]

Therefore
\[
\boxed{
r_{\rm an}(E)-r_p(E)
=
\sum_i d_i(E,p)
\ge0.
}
\]

By the known parity theorem,
\[
\boxed{
\sum_i d_i(E,p)\in2\mathbb Z_{\ge0}.
}
\]

## 6. Full BSD defect spectrum

The Selmer/Sha decomposition is
\[
r_p(E)
=
r_{\rm MW}(E)+s_p(E),
\]
with
\[
s_p(E)
=
\operatorname{corank}_{\mathbb Z_p}
\Sha(E/\mathbb Q)[p^\infty].
\]

Combining the two exact decompositions gives
\[
\boxed{
r_{\rm an}(E)-r_{\rm MW}(E)
=
\sum_{i=1}^{r_p(E)}d_i(E,p)
+
s_p(E).
}
\]

Under the registration hypotheses, every term on the right is nonnegative.

Hence
\[
\boxed{
\mathrm{BSD}_{\rm rank}
\iff
d_i(E,p)=0\ \forall i
\quad\text{and}\quad
s_p(E)=0.
}
\]

Equivalently, BSD rank equality means:

1. every registered Selmer zero mode crosses transversely at first order;
2. there is no divisible \(p\)-primary Tate--Shafarevich corank.

## 7. Relational-zero interpretation

This is a literal decomposition of zero multiplicity:

\[
\boxed{
\text{analytic multiplicity}
=
\text{number of arithmetic zero modes}
+
\text{higher contact depth}.
}
\]

After the Selmer-to-Mordell--Weil split,

\[
\boxed{
\text{analytic multiplicity}
=
\text{Mordell--Weil modes}
+
\text{Sha modes}
+
\text{higher contact depth}.
}
\]

The two obstruction classes are structurally distinct:

- \(s_p\) counts arithmetic zero modes present in Selmer but not in Mordell--Weil;
- \(d_i\) measures excess analytic multiplicity carried by higher-order contact of already registered zero modes.

## 8. Firewall

The Smith-normal theorem is exact local algebra.

The BSD formula above is conditional on the global registrations
\[
\operatorname{ord}\det C_{E,p}=r_{\rm an}(E)
\]
and
\[
\dim H^1(C_{E,p}\otimes K)=r_p(E).
\]

Those global comparisons remain the unresolved arithmetic-analytic content.

No Q.E.D. is promoted.
