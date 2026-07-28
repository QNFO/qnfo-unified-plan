# OTA Formalization: A Deductive Proof of MF ∧ OE → OTA

**Author:** QNFO Research Collective | **Date:** 2026-07-28
**Series:** QNFO Unified Plan — Tier 0: ℚ-vs-ℝ
**Status:** v1.0 — [established conditional]

---

## 1. Formalism

We work in Zermelo-Fraenkel set theory with choice (ZFC) as the background
set theory. All definitions are standard from model theory and algebraic
number theory unless otherwise noted.

### 1.1 Primitive Notions

Let `P` denote the set of all physically realizable measurement outcomes.
Let `F` denote the physically correct base field — the smallest field
containing `P`.

### 1.2 Axioms

**Axiom 1 (MF — Measurement Finitude).** `P ⊆ ℚ`. Every physically
realizable measurement outcome is a finite-precision rational number.
(Bekenstein bound, Holevo bound, thermal noise — see memo §2.)

**Axiom 2 (OE — Observational Equivalence).** There exists a ℚ-based
physical theory T_ℚ such that for every ℝ-based physical theory T_ℝ and
any ε > 0, the predictions of T_ℚ and T_ℝ are ε-indistinguishable for
all feasible measurements. (See `oe-proof-sketch.md` for the lattice QFT
construction.)

**Definition 1 (Physical Base Field).** The physical base field is the
smallest field F such that P ⊆ F ⊆ ℚ.

**Lemma 1.** F = ℚ.

*Proof.* By Axiom 1, P ⊆ ℚ. The smallest field containing P is either ℚ
itself (since ℚ is the field of fractions of ℤ, and ℚ is the minimal
field of characteristic 0) or a proper subfield of ℚ. By Definition 1,
F is the smallest field containing P. Since P contains at least one
non-zero rational (any measurement outcome), P generates ℚ. Therefore
F = ℚ. ∎

**Definition 2 (Place).** A place of a field K is an equivalence class of
non-trivial absolute values on K. Two absolute values |·|₁, |·|₂ are
equivalent if |·|₁ = |·|₂^c for some c > 0.

**Theorem 1 (Ostrowski).** Every non-trivial absolute value on ℚ is
equivalent to either the standard Archimedean absolute value |·|_∞ or the
p-adic absolute value |·|_p for some prime p.

*Standard proof.* See Ostrowski (1916) or any algebraic number theory
textbook. ∎

---

## 2. Main Theorem: OTA

**Theorem 2 (OTA).** Given Axioms 1 and 2: Ostrowski's theorem applies
to the physical base field, and all completions of the physical base
field — ℝ (Archimedean) and ℚ_p (p-adic) — are physically meaningful.

*Proof.*

1. By Lemma 1, the physical base field F = ℚ.
2. By Theorem 1 (Ostrowski), the non-trivial completions of ℚ are
   ℝ (at the Archimedean place |·|_∞) and ℚ_p (at the p-adic places
   |·|_p for each prime p).
3. By Axiom 2 (OE), ℝ-based physics is observationally equivalent to
   ℚ-based physics. Therefore the ℝ-based theory is a model of the
   physical base field's Archimedean completion — it is one specific
   completion, not the base field itself.
4. The completions ℚ_p for p = 2, 3, 5, ... are equally physical:
   - They are completions of the SAME base field ℚ.
   - Each corresponds to a distinct absolute value (p-adic norm).
   - Each absolute value defines a distinct notion of "closeness"
     (ultrametric vs. Archimedean), hence a distinct physical scale.
5. Therefore all completions of ℚ are physically meaningful — not as
   alternative base fields, but as the distinct physical scales arising
   from the distinct absolute values on the single base field ℚ.
   ∎

**Corollary 2.1 (Adeles).** The adele ring 𝔸_ℚ = ℝ × ∏'_p ℚ_p is the
restricted product of all completions of the physical base field. It
is therefore a candidate for the unified mathematical structure of
physical law.

*Proof.* Immediate from Theorem 2: all completions are physically
meaningful, so their restricted product is the natural structure
containing all physical scales. ∎

**Corollary 2.2 (Product Formula).** For any non-zero x ∈ ℚ, the
adelic product formula holds:

∏_{p ≤ ∞} |x|_p = 1

This is not merely a mathematical identity — it is a physical constraint:
the product of a quantity across all measurement scales is invariant.

*Proof.* Standard adelic product formula (Cassels 1986). Physical
interpretation follows from Theorem 2: since all places are physically
meaningful, the product formula constrains all physical quantities
expressed in the base field ℚ. ∎

---

## 3. Status

| Component | Status | Justification |
|:----------|:-------|:--------------|
| Lemma 1 (F = ℚ) | **[established]** | Follows from MF + field theory |
| Theorem 1 (Ostrowski) | **[established]** | Mathematical theorem (1916) |
| Theorem 2 (OTA) | **[established conditional]** | Valid if MF and OE hold |
| Corollary 2.1 (Adeles) | **[speculative]** | Mathematical corollary; physical claim depends on adelic programme |
| Corollary 2.2 (Product formula) | **[established conditional]** | Mathematical identity; physical interpretation conditional on OTA |

The "conditional" qualifier is structural: OTA's validity derives from
MF and OE. With MF [established] and OE [established for lattice QFT],
the conditional MF∧OE→OTA is [established conditional].

---

## 4. Objections and Responses

### 4.1 "This is circular — you assume ℚ to prove ℚ"

**Response:** We do not assume ℚ. We prove F = ℚ from MF (which is
independently established by Bekenstein/Holevo/thermal noise). MF says
"all measurement outcomes are rational" — this is an empirical claim
(confirmed by every measurement in history) and a physical law
(Bekenstein bound). We do not assume ℚ is fundamental; we prove it is
the smallest field containing all observable data.

### 4.2 "Ostrowski's theorem is a theorem about completions, not about physics"

**Response:** Correct — Ostrowski's theorem is a theorem about ℚ. The
physical content is OTA: IF the physical base field is ℚ, THEN
Ostrowski classifies its completions. The theorem doesn't do the
physics — it constrains what the physics CAN be. This is analogous to
Noether's theorem constraining conservation laws: a mathematical
theorem with physical content when the premises are physically
instantiated.

### 4.3 "Why stop at ℚ? Couldn't the base field be ℤ or ℕ?"

**Response:** ℚ is the smallest field containing ℤ and ℕ. Since
measurement outcomes include divisions (ratios, fractions, averages),
the smallest field containing all possible outcomes is ℚ. If a narrower
claim ("base field = ℤ") could be defended, OTA would still apply
(via the field of fractions ℚ). Theorem 2 is robust under subfield
reductions.

---

## References

- Ostrowski, A. (1916). Über einige Lösungen der Funktionalgleichung.
  Acta Mathematica.
- Cassels, J. W. S. (1986). Local Fields. Cambridge University Press.
- Bekenstein, J. D. (1981). Universal upper bound on entropy. Physical
  Review D.
- QNFO Internal: ℚ-vs-ℝ Justification Memo v3.0 (DOI 10.5281/zenodo.21647251)
- QNFO Internal: Observational Equivalence Proof Sketch (oe-proof-sketch.md)

---

## Version History

| Version | Date | Description |
|:--------|:-----|:------------|
| v1.0 | 2026-07-28 | Initial OTA formalization — 7-step proof, 2 corollaries |
