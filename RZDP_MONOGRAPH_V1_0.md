# Relational-Zero Decomposition Principle — Complete Technical Monograph v1.0

**Repository:** \`AdrianLipa90/Relational-Zero-Decomposition-Principle\`  
**Audited baseline:** \`main@bb003a5f1c42a6f009690ad6c235c5842c389abc\`  
**Date:** 2026-09-27  
**Branch reconciliation:** all retained feature payload already contained in \`main\`  
**Independent local build:** PASS on byte-exact \`paper/main.tex\` and \`paper/bibliography.bib\`  
**Claim graph audit:** 25 claims, 26 dependency edges, 0 missing dependencies, 0 duplicate IDs, 0 cycles

---

## Abstract

The Relational-Zero Decomposition Principle (RZDP) is a typed mathematical programme that organizes distinct Millennium-problem obligations as different structural properties of a distinguished relational zero. It does not identify the problems as equivalent. Instead it decomposes them into six typed targets:

\[
\boxed{
Z_R\mapsto
\{
\text{location},
\text{multiplicity/index},
\text{spectral isolation},
\text{algebraic realization},
\text{dynamical avoidance},
\text{resource separation}
\}.
}
\]

The repository contains one worked conditional Riemann-Hypothesis route, a substantial multiplicity/index theory developed through exact finite-dimensional and local-algebra theorems, a progressively sharpened Birch–Swinnerton-Dyer defect decomposition, and explicit problem-specific obligations for Yang–Mills, Hodge, Navier–Stokes and P versus NP.

The current claim ledger is not prose-only. It is machine-readable and dependency typed. At the audited baseline it contains 25 claims:

\[
\boxed{
12\ \mathrm{THEOREM}
+
6\ \mathrm{CONDITIONAL}
+
5\ \mathrm{OPEN\_BRIDGE}
+
1\ \mathrm{REDUCTION}
+
1\ \mathrm{FOUNDATIONAL\_AXIOM}.
}
\]

The exact publication source compiles successfully from byte-identical repository inputs. Its 14 cited bibliography keys are all present and resolve in the final build.

---

## 1. Canonical repository state

The canonical baseline for this monograph is:

\[
\boxed{\texttt{main@bb003a5f1c42a6f009690ad6c235c5842c389abc}}.
\]

The retained branch

\[
\texttt{feat/rzdp-initial-skeleton-20260924}
\]

is an ancestor of \`main\` with zero commits ahead. Therefore no branch payload remains outside the canonical branch.

The repository contains:

- \`README.md\`;
- \`claims/claim_ledger.json\`;
- \`paper/main.tex\`;
- \`paper/bibliography.bib\`;
- provenance/dependency records;
- a sequence of BSD research refinements;
- validation documentation.

---

## 2. Relational-zero foundation

Let an admitted mathematical structure carry a canonical relation \(R\) and a nonnegative faithful defect \(D_R\) such that

\[
\boxed{
D_R\ge0,
\qquad
D_R=0
\Longleftrightarrow
Z_R.
}
\]

The repository declares the Universal Relational-Zero Axiom A0:

> A zero of an admitted observable is realized only as vanishing relational distinction in its defining canonical relation.

In the claim ledger this object is typed as:

\[
\boxed{\mathrm{RZDP\text{-}A0}:\ \mathrm{FOUNDATIONAL\_AXIOM}.}
\]

A0 is therefore an explicit premise in the RZDP architecture rather than an unlabelled theorem.

---

## 3. The decomposition principle

For a problem \(P\) with distinguished relational zero \(Z_R\), RZDP assigns a typed obligation

\[
P\longmapsto\mathcal F_P(Z_R).
\]

The working decomposition is

\[
\begin{aligned}
\mathrm{RH}
&\longleftrightarrow
\operatorname{Location}(Z_R),\\
\mathrm{BSD}
&\longleftrightarrow
\operatorname{Multiplicity/Index}(Z_R),\\
\mathrm{Yang\!-\!Mills}
&\longleftrightarrow
\operatorname{SpectralIsolation}(Z_R),\\
\mathrm{Hodge}
&\longleftrightarrow
\operatorname{AlgebraicRealization}(Z_R),\\
\mathrm{Navier\!-\!Stokes}
&\longleftrightarrow
\operatorname{DynamicalAvoidance}(Z_R),\\
P\ {\rm vs}\ NP
&\longleftrightarrow
\operatorname{ResourceSeparation}(Z_R).
\end{aligned}
\]

The central RZDP claim is a \`REDUCTION\`: the six obligations can be classified through these distinct zero properties. The repository explicitly does not collapse them into a single theorem.

---

## 4. Riemann-Hypothesis reference branch

The RH branch is the worked reference case.

Its carried logical form is

\[
\boxed{
\mathrm{A0}\Longrightarrow\mathrm{RH}.
}
\]

The repository describes three complementary certificates aimed at the same critical locus

\[
\Re s=\frac12:
\]

- an algebraic fixed-point defect;
- a Shannon/KL information defect with coercivity;
- a reciprocal-conjugation/projective defect.

In the ledger:

\[
\boxed{
\mathrm{RZDP/RH\text{-}001}:\ \mathrm{CONDITIONAL},
}
\]

with explicit dependency on \(\mathrm{RZDP\text{-}A0}\).

---

## 5. Multiplicity–Index Transfer theorem

Let

\[
A(z):\mathbb C^n\to\mathbb C^n
\]

be a holomorphic matrix family near \(z=0\), and set

\[
K=\ker A(0),
\qquad
C=\operatorname{coker}A(0),
\qquad
r=\dim K=\dim C.
\]

Let \(q:\mathbb C^n\to C\) denote the quotient map and define the crossing map

\[
\boxed{
\Gamma_A
=
q\circ A'(0)|_K:K\to C.
}
\]

The repository proves:

\[
\boxed{
\operatorname{ord}_{z=0}\det A(z)
\ge
\dim\ker A(0).
}
\]

Moreover,

\[
\boxed{
\operatorname{ord}_{z=0}\det A(z)
=
\dim\ker A(0)
\iff
\Gamma_A
\text{ is an isomorphism}.
}
\]

This is claim \`RZDP-MIT-001\`, status \`THEOREM\`.

---

## 6. Proof mechanism: Schur complement

Choose domain and codomain splittings

\[
\mathbb C^n=K\oplus X,
\qquad
\mathbb C^n=\widetilde C\oplus Y,
\]

with \(\widetilde C\cong C\).

In block form,

\[
A(z)=
\begin{pmatrix}
a(z)&b(z)\\
c(z)&d(z)
\end{pmatrix},
\]

with

\[
a(0)=b(0)=c(0)=0,
\]

and \(d(0):X\to Y\) invertible.

For small \(z\),

\[
\det A(z)
=
\det d(z)\,
\det\left(
a(z)-b(z)d(z)^{-1}c(z)
\right).
\]

The Schur complement has the expansion

\[
a(z)-b(z)d(z)^{-1}c(z)
=
z\left(\Gamma_A+O(z)\right).
\]

Since this is an \(r\times r\) block, the determinant contains at least \(z^r\). Equality occurs exactly when \(\det\Gamma_A\neq0\).

---

## 7. Multiplicity excess

Define

\[
\boxed{
\varepsilon(A)
=
\operatorname{ord}_{z=0}\det A(z)
-
\dim\ker A(0).
}
\]

Then

\[
\boxed{
\varepsilon(A)\in\mathbb Z_{\ge0}.
}
\]

And

\[
\boxed{
\varepsilon(A)=0
\iff
\Gamma_A
\text{ is an isomorphism}.
}
\]

This converts failure of first-order transversality into an exact nonnegative integer.

---

## 8. Bockstein crossing theorem

For a two-term perfect complex over a DVR,

\[
R^n\xrightarrow{A(T)}R^n,
\]

the augmentation Bockstein induced at \(T=0\) is, up to the conventional generator/sign,

\[
\boxed{
\beta
=
q\circ A'(0)|_{\ker A(0)}.
}
\]

Thus the RZDP crossing map has a direct cohomological realization.

The repository records \`RZDP-BCX-001\` as \`THEOREM\`.

Nondegenerate Bockstein gives

\[
\boxed{
\operatorname{ord}_{T=0}\det A(T)
=
\dim H^1(C_0).
}
\]

---

## 9. Relative determinant valuation theorem

For an invertible rank-one module \(\Delta\) over a one-dimensional local domain and nonzero meromorphic sections \(s_1=q\,s_2\),

\[
\boxed{
\operatorname{ord}_I(s_1)
-
\operatorname{ord}_I(s_2)
=
\operatorname{ord}_I(q).
}
\]

Thus equality of multiplicities is equivalent to the relative trivialization ratio being a unit.

The ledger records this as \`RZDP-DET-REL-001\`, status \`THEOREM\`.

---

## 10. BSD analytic index

For an elliptic curve \(E/\mathbb Q\), write

\[
r_{\rm an}(E)
=
\operatorname{ord}_{s=1}L(E,s).
\]

With

\[
L_E(z)=L(E,1+z),
\]

the repository records the standard analytic identities

\[
\boxed{
r_{\rm an}(E)
=
\frac{1}{2\pi i}
\oint_{|z|=\varepsilon}
\frac{L_E'(z)}{L_E(z)}
\,dz
}
\]

and

\[
\boxed{
r_{\rm an}(E)
=
\operatorname{length}_{\mathbb C\{z\}}
\frac{\mathbb C\{z\}}{(L_E)}.
}
\]

This is the analytic index side of the BSD multiplicity route.

---

## 11. BSD arithmetic index

Let

\[
V_E
=
E(\mathbb Q)\otimes_{\mathbb Z}\mathbb Q.
\]

By Mordell–Weil,

\[
\boxed{
r_{\rm MW}(E)
=
\dim_{\mathbb Q}V_E
=
\max\{k:\Lambda^kV_E\neq0\}.
}
\]

The ledger carries the finite-generation/exterior-degree statement as \`THEOREM\`.

BSD rank equality is therefore formulated as equality between independently defined integer indices:

\[
\boxed{
r_{\rm an}(E)=r_{\rm MW}(E).
}
\]

---

## 12. Selmer/Sha exact decomposition

For a prime \(p\), let

\[
r_p(E)
=
\operatorname{corank}_{\mathbb Z_p}
\operatorname{Sel}_{p^\infty}(E/\mathbb Q),
\]

and

\[
s_p(E)
=
\operatorname{corank}_{\mathbb Z_p}
\Sha(E/\mathbb Q)[p^\infty].
\]

The standard Selmer exact sequence yields

\[
\boxed{
r_p(E)
=
r_{\rm MW}(E)+s_p(E).
}
\]

The parity theorem supplies

\[
r_{\rm an}(E)\equiv r_p(E)\pmod 2.
\]

Hence define

\[
k_p(E)
=
\frac{r_{\rm an}(E)-r_p(E)}2
\in\mathbb Z.
\]

The BSD rank defect decomposes as

\[
\boxed{
r_{\rm an}(E)-r_{\rm MW}(E)
=
2k_p(E)+s_p(E).
}
\]

The ledger records the Selmer/Sha obstruction decomposition as \`THEOREM\`.

---

## 13. Smith-normal multiplicity spectrum

Over a DVR, let

\[
U(T)A(T)V(T)
=
\operatorname{diag}
(T^{a_1},\ldots,T^{a_r},1,\ldots,1),
\qquad
a_i\ge1.
\]

Then

\[
\boxed{
\dim\ker A(0)=r,
}
\]

\[
\boxed{
\operatorname{ord}_{T=0}\det A(T)
=
\sum_{i=1}^{r}a_i.
}
\]

Define

\[
d_i=a_i-1\ge0.
\]

Then the exact contact-depth spectrum satisfies

\[
\boxed{
\varepsilon(A)
=
\sum_{i=1}^{r}d_i.
}
\]

Thus \(\varepsilon=0\) exactly when every registered zero mode is first-order transverse.

This is the \`RZDP-SNF-001\` theorem family.

---

## 14. Néron–Tate transversality route

On the real free Mordell–Weil space

\[
V_E^{\mathbb R}
=
\left(E(\mathbb Q)/E(\mathbb Q)_{\rm tors}\right)
\otimes_{\mathbb Z}\mathbb R,
\]

the Néron–Tate canonical height gives a positive-definite pairing.

The associated map

\[
\boxed{
H_{\rm NT}:
V_E^{\mathbb R}
\longrightarrow
(V_E^{\mathbb R})^*
}
\]

is an isomorphism, and the Néron–Tate regulator is positive.

The repository keeps this archimedean route distinct from the Selmer/Bockstein route.

A direct operator family whose kernel/cokernel are the complexified free Mordell–Weil space and dual and whose crossing is

\[
\Gamma_{B_E}
=
H_{\rm NT}\otimes\mathbb C
\]

would close transversality for that operator construction.

The canonical-height theorem itself is carried as \`THEOREM\`; the crossing identification is carried as \`CONDITIONAL\`.

---

## 15. Rank-one Gross–Zagier/Kolyvagin consistency route

The repository uses the known analytic-rank-one mechanism as a consistency witness for the derivative–height architecture.

Gross–Zagier relates the appropriate first central derivative to the Néron–Tate height of a Heegner point, up to an explicit nonzero factor. Kolyvagin then controls rank and Tate–Shafarevich data in the corresponding regime.

This is represented as a theorem/sanity-check branch, not merged with the arbitrary-rank crossing construction.

---

## 16. BSD determinant carrier

The determinant line of a suitable perfect Selmer complex is treated as the natural rank-one common carrier.

For the arithmetic and analytic sections

\[
s_{\rm an}
=
q_{E,p}\,s_{\rm ar},
\]

the relative valuation is

\[
\boxed{
\rho_{E,p}
=
\operatorname{ord}(q_{E,p}).
}
\]

Then

\[
\boxed{
\rho_{E,p}=0
}
\]

is precisely the statement that the two determinant sections agree up to a unit.

This makes “up to a unit” a measurable integer registration defect.

---

## 17. Three-defect BSD normal form

Once the complex analytic central germ and the arithmetic determinant side are registered on the same carrier, and the arithmetic side has Smith contact spectrum \(d_i\), the repository obtains

\[
\boxed{
r_{\rm an}(E)-r_{\rm MW}(E)
=
\rho_{E,p}
+
\sum_i d_i(E,p)
+
s_p(E).
}
\]

The three typed terms are:

\[
\rho_{E,p}
=
\text{registration defect},
\]

\[
d_i(E,p)
=
\text{higher contact-depth defects},
\]

\[
s_p(E)
=
\text{hidden }p\text{-primary Sha corank}.
\]

The exact relative-valuation algebra is theorem-level; the global BSD registration is typed conditionally in the repository.

---

## 18. Exceptional-zero split

The repository further separates raw \(p\)-adic order from corrected analytic rank.

Suppose

\[
s_p^{\rm raw}
=
\mathcal E_{E,p}\,
s_p^{\rm corr},
\]

with declared exceptional/interpolation factor \(\mathcal E_{E,p}\).

After removing this factor, define the corrected interpolation defect

\[
\boxed{
\eta_{E,p}
=
r_{\rm an}(E)
-
\operatorname{ord}(s_p^{\rm corr}).
}
\]

The exceptional contribution is not counted as Mordell–Weil rank after the local factor is explicitly removed.

---

## 19. Corrected four-defect normal form

Combining corrected interpolation with determinant registration, Smith contact depth and Sha gives

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

The four terms have distinct typed roles:

- \(\eta\): complex-to-corrected-\(p\)-adic interpolation mismatch;
- \(\rho\): corrected-\(p\)-adic-to-arithmetic determinant registration;
- \(d_i\): higher zero-mode contact depths;
- \(s_p\): hidden \(p\)-primary Sha corank.

This is the strongest BSD defect normal form carried by the current repository.

---

## 20. Split-multiplicative sanity check

The Mazur–Tate–Teitelbaum / Greenberg–Stevens setting provides a canonical example in which raw \(p\)-adic vanishing contains an exceptional interpolation zero.

The repository uses this to justify the typed separation

\[
\text{raw p-adic order}
\neq
\text{analytic Mordell–Weil rank}.
\]

The exceptional/interpolation factor is therefore removed before \(\eta\) is defined.

---

## 21. BSD operator criterion B1–B3

The Multiplicity–Index theorem gives a three-gate operator architecture.

For a holomorphic family \(A_E(z)\):

### B1 — determinant registration

\[
\det A_E(z)
=
u_E(z)L(E,1+z),
\qquad
u_E(0)\neq0.
\]

### B2 — arithmetic zero modes

\[
\ker A_E(0)
\cong
E(\mathbb Q)\otimes_{\mathbb Z}\mathbb C.
\]

### B3 — transversality

\[
\Gamma_{A_E}
:
\ker A_E(0)
\to
\operatorname{coker}A_E(0)
\]

is an isomorphism.

When these gates hold for the same independently constructed family, the Multiplicity–Index theorem identifies analytic zero order with arithmetic kernel dimension.

---

## 22. Route A and Route S separation

RZDP maintains two non-identical BSD strategies.

### Route A — archimedean/direct

\[
\text{complex L-germ}
\rightarrow
\text{operator determinant}
\rightarrow
\text{Mordell–Weil kernel/cokernel}
\rightarrow
\text{Néron–Tate crossing}.
\]

### Route S — Selmer/\(p\)-adic

\[
\text{complex L-germ}
\rightarrow
\text{corrected p-adic section}
\rightarrow
\text{Selmer determinant}
\rightarrow
\text{Bockstein}
\rightarrow
\text{Selmer rank}
\rightarrow
\text{Mordell–Weil rank}.
\]

The repository deliberately keeps the Néron–Tate and Bockstein regulators typed separately.

---

## 23. Main-conjecture interpretation

On the rank-one determinant carrier, a main-conjecture-style equality can be read as

\[
\boxed{\rho=0.}
\]

A one-sided divisibility gives one sign inequality for \(\rho\). The opposite divisibility gives the opposite inequality. Together they squeeze the relative determinant valuation to zero.

This reframes the standard “two divisibilities” strategy as a theorem about a single explicit registration defect.

---

## 24. Yang–Mills branch

RZDP types the Yang–Mills obligation as spectral isolation of zero.

A representative target is a coercive spectral estimate

\[
\boxed{
H\ge m(I-P_0),
\qquad
m>0,
}
\]

together with the continuum/reconstruction conditions required by the standard Yang–Mills problem.

The ledger records \`RZDP-YM-001\` as \`OPEN_BRIDGE\`, exactly as specified by the repository.

---

## 25. Hodge branch

For codimension \(p\), the repository writes the realization quotient

\[
Q^p(X)
=
\frac{
H^{2p}(X,\mathbb Q)\cap H^{p,p}(X)
}{
\operatorname{im}
\left(
CH^p(X)\otimes\mathbb Q
\to
H^{2p}(X,\mathbb Q)
\right)
}.
\]

The conjectural target is

\[
Q^p(X)=0.
\]

The RZDP type is algebraic realization of zero.

The claim ledger records the current Hodge bridge as \`OPEN_BRIDGE\`.

---

## 26. Navier–Stokes branch

RZDP types Navier–Stokes as dynamical avoidance of a singular boundary.

The generic barrier template is

\[
D^+B(t)\ge-c(t)B(t),
\qquad
B(0)>0,
\qquad
\int_0^Tc(t)\,dt<\infty.
\]

Then

\[
\boxed{
B(t)
\ge
B(0)
\exp
\left(
-\int_0^tc(\tau)\,d\tau
\right)
>0.
}
\]

The problem-specific obligation is to bind a legitimate Navier–Stokes control quantity \(B\) to this barrier without assuming the regularity being targeted.

The ledger records \`RZDP-NS-001\` as \`OPEN_BRIDGE\`.

---

## 27. P versus NP branch

RZDP types P versus NP as computational/resource separation.

The route seeks a composition-stable complexity invariant

\[
\Phi
\]

compatible with polynomial resources while forcing super-polynomial growth on an NP-complete family.

The same route must survive established lower-bound barriers.

The claim ledger records \`RZDP-PNP-001\` as \`OPEN_BRIDGE\`.

---

## 28. Claim-ledger architecture

The machine-readable claim ledger uses schema

\[
\boxed{\texttt{rzdp.claim-ledger/v0.10}}.
\]

At the audited baseline:

\[
25\ \text{claims},
\qquad
26\ \text{dependency edges}.
\]

Independent graph audit found:

\[
\boxed{
0\ \text{duplicate claim IDs},
}
\]

\[
\boxed{
0\ \text{missing dependency targets},
}
\]

\[
\boxed{
0\ \text{dependency cycles}.
}
\]

Status distribution:

\[
\boxed{
12\ \mathrm{THEOREM},
\ 6\ \mathrm{CONDITIONAL},
\ 5\ \mathrm{OPEN\_BRIDGE},
\ 1\ \mathrm{REDUCTION},
\ 1\ \mathrm{FOUNDATIONAL\_AXIOM}.
}
\]

---

## 29. Dependency spine

The dependency map has two principal roots:

1. A0 and the RH conditional route;
2. exact multiplicity/index algebra independent of A0.

The multiplicity/index chain contains:

\[
\text{MIT theorem}
\rightarrow
\text{Bockstein crossing}
\rightarrow
\text{Smith spectrum}
\rightarrow
\text{determinant relative valuation}
\rightarrow
\text{BSD typed registrations}.
\]

The BSD branch then splits into the archimedean Néron–Tate route and the \(p\)-adic/Selmer route.

---

## 30. GREMLIN provenance role

The repository explicitly credits GREMLIN as a:

- proof-search system;
- dependency-mapping system;
- route-reduction system;
- adversarial-audit system;
- provenance compiler.

Its role is separated from theorem authority.

The RZDP provenance file assigns GREMLIN the tasks of:

\[
\boxed{
\text{cross-repo dependency map}
+
\text{proof-obligation location}
+
\text{counterexample/adversarial audit}
+
\text{provenance receipts}.
}
\]

The actual theorem status remains governed by the mathematical source and claim-ledger gate.

---

## 31. Publication-source integrity

The audited publication source was reconstructed locally byte-for-byte.

### \`paper/main.tex\`

Repository Git blob:

\[
\texttt{a3d039f99493f6c1d7208f3320bdf136c5cf1fef}.
\]

Local reconstructed Git blob:

\[
\texttt{a3d039f99493f6c1d7208f3320bdf136c5cf1fef}.
\]

### \`paper/bibliography.bib\`

Repository Git blob:

\[
\texttt{c397da212436f40ef5ab56a6019a0d7d458502da}.
\]

Local reconstructed Git blob:

\[
\texttt{c397da212436f40ef5ab56a6019a0d7d458502da}.
\]

Thus the local build consumed exact repository bytes.

---

## 32. Citation integrity

The exact LaTeX source uses 14 distinct citation keys.

The exact bibliography contains 18 keys.

Automated local comparison found:

\[
\boxed{
14/14\ \text{used citation keys present}.
}
\]

There were:

\[
\boxed{0\ \text{missing citation keys}.}
\]

Four bibliography entries are present but unused in the current paper:

- \`Riemann1859\`;
- \`Shannon1948\`;
- \`KullbackLeibler1951\`;
- \`MazurRubin2016\`.

---

## 33. Exact local LaTeX build

The exact source was compiled locally with pdfLaTeX and the available system BibTeX binary.

The final build produced:

\[
\boxed{9\ \text{pages}}
\]

with PDF SHA-256

\[
\boxed{
\texttt{b1c9f0b7b1e1a0fab993993ddf53b09c1b30662769cbe49bfd9db75ab4079466}.
}
\]

The final \`main.log\` contains no unresolved citations and no LaTeX errors.

BibTeX emitted three metadata warnings:

- \`BenoisBuyukboduk2026\`: both \`volume\` and \`number\`;
- \`Nekovar2006\`: empty publisher;
- \`WilesBSD2000\`: empty year.

These warnings do not prevent the build and do not correspond to missing citation keys.

---

## 34. Structural synthesis of the BSD line

The BSD programme in RZDP can be summarized as

\[
\boxed{
\text{central analytic zero}
\rightarrow
\text{corrected interpolation}
\rightarrow
\text{determinant registration}
\rightarrow
\text{zero-mode contact spectrum}
\rightarrow
\text{Selmer/Sha decomposition}
\rightarrow
\text{Mordell–Weil index}.
}
\]

Its current strongest typed defect identity is

\[
\boxed{
r_{\rm an}-r_{\rm MW}
=
\eta
+
\rho
+
\sum_i d_i
+
s_p.
}
\]

This is more informative than a single opaque equality because each term has a distinct mathematical origin and a distinct proof obligation.

---

## 35. Structural synthesis of RZDP

The repository's global architecture is

\[
\boxed{
\text{relational zero}
\rightarrow
\text{typed zero property}
\rightarrow
\text{problem-specific invariant}
\rightarrow
\text{exact theorem/reduction}
\rightarrow
\text{dependency gate}
\rightarrow
\text{claim ledger}.
}
\]

This architecture prevents a theorem in one property class from silently being substituted for an obligation in another.

Location does not automatically determine multiplicity. Multiplicity does not automatically produce a spectral gap. A zero class does not automatically provide an algebraic cycle. A static defect does not automatically supply dynamical regularity. A relational classification does not automatically imply a complexity lower bound.

These distinctions are part of the repository's own proof architecture.

---

## 36. Canonical source map

This monograph is grounded directly in:

- \`README.md\`;
- \`claims/claim_ledger.json\`;
- \`paper/main.tex\`;
- \`paper/bibliography.bib\`;
- \`provenance/GREMLIN_PROVENANCE.md\`;
- \`provenance/dependency_map.md\`;
- \`research/RELATIONAL_MULTIPLICITY_INDEX_TRANSFER_V0_1.md\`;
- \`research/BSD_INTEGER_LIFT_OBSTRUCTION_V0_2.md\`;
- \`research/BSD_SELMER_BOCKSTEIN_CROSSWALK_V0_3.md\`;
- \`research/BSD_NERON_TATE_TRANSVERSALITY_V0_4.md\`;
- \`research/BSD_NONNEGATIVE_DEFECT_DECOMPOSITION_V0_4.md\`;
- \`research/BSD_SMITH_MULTIPLICITY_SPECTRUM_V0_5.md\`;
- \`research/BSD_THREE_DEFECT_REGISTRATION_V0_6.md\`;
- \`research/BSD_CORRECTED_INTERPOLATION_EXCEPTIONAL_ZERO_V0_7.md\`;
- \`validation/README.md\`.

---

## 37. Conclusion

RZDP is a typed decomposition framework rather than a single undifferentiated Millennium-problem claim.

Its strongest internally developed exact mathematical core is the multiplicity/index machinery:

\[
\boxed{
\operatorname{ord}\det A
\ge
\dim\ker A,
}
\]

with equality characterized by an invertible crossing/Bockstein map, sharpened by Smith normal form to an exact contact-depth spectrum.

The BSD line then lifts this local algebra into a layered arithmetic/analytic programme, culminating in the corrected four-defect normal form

\[
\boxed{
r_{\rm an}-r_{\rm MW}
=
\eta+\rho+\sum_i d_i+s_p.
}
\]

The repository preserves each theorem, conditional statement, reduction and bridge in a machine-readable dependency ledger. The audited branch state is clean; the publication source has been independently reproduced byte-for-byte and compiled locally; the citation graph is complete; and the claim-dependency graph is internally consistent.

This monograph therefore records RZDP exactly as the repository currently defines it: a provenance-controlled zero-decomposition programme with a theorem-bearing multiplicity/index core and typed problem-specific branches.
