# BSD Integer-Lift Obstruction Decomposition v0.2

Status: **EXACT DECOMPOSITION / TWO-TARGET REDUCTION / BSD STILL OPEN**

Date: 2026-09-24

## 1. Three ranks

For an elliptic curve \(E/\mathbb Q\) and a prime \(p\), define

\[
r_{\rm an}(E):=\operatorname{ord}_{s=1}L(E,s),
\]

\[
r_p(E):=\operatorname{corank}_{\mathbb Z_p}
\operatorname{Sel}_{p^\infty}(E/\mathbb Q),
\]

and

\[
r_{\rm MW}(E):=\operatorname{rank}_{\mathbb Z}E(\mathbb Q).
\]

Also define

\[
s_p(E):=
\operatorname{corank}_{\mathbb Z_p}
\Sha(E/\mathbb Q)[p^\infty].
\]

## 2. Exact arithmetic decomposition

The standard Kummer/Selmer exact sequence

\[
0\to E(\mathbb Q)\otimes \mathbb Q_p/\mathbb Z_p
\to \operatorname{Sel}_{p^\infty}(E/\mathbb Q)
\to \Sha(E/\mathbb Q)[p^\infty]
\to0
\]

gives, after taking \(\mathbb Z_p\)-coranks,

\[
\boxed{
r_p(E)=r_{\rm MW}(E)+s_p(E).
}
\]

Hence the Selmer-to-Mordell--Weil defect is not hidden:

\[
\boxed{
r_p-r_{\rm MW}=s_p\ge0.
}
\]

## 3. Exact parity input

The Dokchitser--Dokchitser \(p\)-parity theorem over \(\mathbb Q\) gives

\[
r_{\rm an}(E)\equiv r_p(E)\pmod2.
\]

Therefore there exists an integer

\[
k_p(E):=
\frac{r_{\rm an}(E)-r_p(E)}{2}
\in\mathbb Z.
\]

No sign is asserted for \(k_p\).

## 4. BSD defect identity

Define the BSD rank defect

\[
\delta_{\rm BSD}(E)
:=
r_{\rm an}(E)-r_{\rm MW}(E).
\]

Substituting the exact Selmer decomposition yields

\[
\begin{aligned}
\delta_{\rm BSD}
&=
(r_{\rm an}-r_p)
+
(r_p-r_{\rm MW})\\
&=
2k_p+s_p.
\end{aligned}
\]

Thus

\[
\boxed{
\delta_{\rm BSD}(E)=2k_p(E)+s_p(E).
}
\]

This identity is exact for every prime \(p\).

Consequently,

\[
\boxed{
\mathrm{BSD}_{\rm rank}
\iff
2k_p(E)+s_p(E)=0.
}
\]

The decomposition must not be over-read: because \(k_p\) need not be non-negative, BSD does not by this identity alone force \(k_p=s_p=0\) separately.

## 5. Two independent proof targets

The formerly single “integer-lift” bridge therefore splits into two typed targets.

### Target A — analytic-to-Selmer integer lift

Upgrade the known parity relation

\[
r_{\rm an}\equiv r_p\pmod2
\]

to an exact comparison strong enough to determine

\[
k_p=\frac{r_{\rm an}-r_p}{2}.
\]

The strongest simple closure would be

\[
r_{\rm an}=r_p,
\]

but this is not assumed.

### Target B — Sha-corank control

Control

\[
s_p=
\operatorname{corank}_{\mathbb Z_p}\Sha[p^\infty].
\]

In particular, finiteness of \(\Sha[p^\infty]\) implies

\[
s_p=0,
\]

and then the BSD rank statement reduces to

\[
r_{\rm an}=r_p.
\]

This is a sufficient route, not a claim that such finiteness has been proved for every elliptic curve.

## 6. RZDP interpretation

BSD is not merely a “multiplicity equals rank” statement. In RZDP it factors as

\[
\boxed{
\text{analytic local multiplicity}
\to
\text{Selmer cohomological index}
\to
\text{Mordell--Weil dimension},
}
\]

with the second arrow carrying the explicit \(\Sha\)-corank obstruction.

Equivalently,

\[
\boxed{
\text{BSD defect}
=
\text{even analytic/Selmer defect}
+
\text{Sha-corank defect}.
}
\]

This is a sharper proof-obligation decomposition than the raw BSD equality.

## 7. Relation to current literature

The parity component is already a theorem over \(\mathbb Q\) for every prime \(p\) (Dokchitser--Dokchitser).

Iwasawa-main-conjecture machinery and modern Euler/Kolyvagin/Selmer-complex methods provide exact comparison theorems in substantial families and low-rank regimes, but the currently checked 2026 literature does not furnish a universal all-elliptic-curves theorem closing both Target A and Target B. Recent 2026 main-conjecture results continue to state applications to the \(p\)-part of BSD in rank at most one.

Therefore no Q.E.D. is promoted.

## 8. Minimal next theorem

The shortest useful next target is no longer the vague full BSD bridge but one of the following:

\[
\boxed{
r_{\rm an}(E)=r_p(E)
}
\]

for a sufficiently general canonical choice of \(p\), together with \(s_p(E)=0\); or a stronger single comparison theorem that proves directly

\[
2k_p(E)+s_p(E)=0.
\]

Any proposed relational/Fredholm/determinant construction must be tested against this exact decomposition.
