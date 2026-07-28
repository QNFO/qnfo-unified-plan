# HANDOFF.md — QNFO Unified Plan: ℚ-vs-ℝ

## Agent Handoff Record

**Date:** 2026-07-28
**Session Agent:** DeepChat (DeepSeek v4 Flash)
**Exit Status:** Phase 3 complete — all 4 sub-claims defended

## Project State

| Asset | URL/Location |
|:------|:-------------|
| GitHub | https://github.com/QNFO/qnfo-unified-plan |
| Zenodo Concept DOI | 10.5281/zenodo.21638962 |
| Zenodo Latest | 10.5281/zenodo.21648034 (v4.0) |
| R2 Artifacts | `qnfo-projects/qnfo-unified-plan/` |
| R2 Releases | `qnfo-releases/releases/2026/07/qnr-justification-memo/v4.0/` |
| D1 Living-Paper | identifier: `qnr-justification-memo` |
| Branch | `feature/phase2.1-oe-proof` (active, unpulled to main) |
| Latest Tag | `v0.4-phase3` (GitHub Release, Latest) |

## Sub-Claim Status

| Claim | Status | Evidence |
|:------|:-------|:---------|
| MF (Measurement Finitude) | [established] | Bekenstein + Holevo + thermal noise bounds |
| OE (Observational Equivalence) | [established for lattice QFT] | Wilson's lattice QFT construction |
| OTA (Ostrowski Applicability) | [established conditional] | MF∧OE→OTA deductive proof |
| CNC (Cardinality Non-Constraint) | [established] | ℚ countability + computable reals |

## Pending WBS

| Phase | Task | Status |
|:------|:-----|:-------|
| Phase 4 | GR Regge calculus ℚ-construction — the last speculative holdout for OE | [PENDING] |
| Merge | feature/phase2.1-oe-proof → feature/phase0-scaffold → main | [PENDING] |
| Buffer | Social post for v4.0 publication | [PENDING] |

## Known Issues / Anti-Patterns

1. **Unmerged branch:** `feature/phase2.1-oe-proof` diverged from `feature/phase0-scaffold`. All Phase 2-4 commits are on the oe-proof branch only. Root branch has only Phase 0-1 commits. Create PR and merge before further development.
2. **KIF-42 (Zenodo Multi-File Protocol):** Research SKILL.md updated with v2.25 banner and corrected Upload Files endpoint. The canonical `zenodo-create-upload.py` + `zenodo-metadata-publish.py` workflow now works correctly — verified live on v3.0 and v4.0.
3. **wrangler v4 removed `r2 object list`:** infra-audit baseline checks need REST API fallback.

## Continuation Prompt

```
--- CONTINUATION PROMPT (paste into new chat) ---
TASK: Complete ℚ-vs-ℝ Phase 4 (GR Regge calculus ℚ-construction) → merge branches → Buffer post → closeout.
STATE: qnfo-unified-plan repo at feature/phase2.1-oe-proof (unmerged). 4 Zenodo versions (v4.0 latest). 3/4 sub-claims at established tier. OE for GR remains [speculative] — this is the last gap.
CONTEXT-ID: qnfo-unified-plan-handoff-001
R2: qnfo-projects/qnfo-unified-plan/ + qnfo-releases/releases/2026/07/qnr-justification-memo/
WBS: Phase 4 pending (GR construction). Merge pending (oe-proof → root → main). Buffer pending.
--- END ---
```
