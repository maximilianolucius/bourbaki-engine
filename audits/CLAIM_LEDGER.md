# Claim ledger — Bourbaki Engine v2

Every load-bearing claim in the manuscript, its support, maturity, and the
disposition taken in the reorientation. Maturity codes as in Table 1:
C conceptual · M manually exercised · P prototype · E controlled eval · X external.

| # | Claim (paraphrase) | §  | Support | Maturity | Decision | Verification owed |
|---|---|---|---|---|---|---|
| 1 | Reliable autonomous math needs separated Discovery and Trust planes | 1,4 | design argument; pilot failure pattern | C | new, keep central | measure FTPR with/without separation |
| 2 | Unit of progress = claim surviving governed promotion | 1,4 | v1 contribution; pilot | M | preserve | — |
| 3 | Reduction/transformation edges carry their own soundness obligation | 2,6 | pilot's costliest defect lived on an edge | M | preserve, strengthen | node-vs-edge error share (Track A/B) |
| 4 | Object type is orthogonal to epistemic state | 6, App.B | MIRADOR design + case study | P | new, keep | — (implemented in MIRADOR) |
| 5 | MIRADOR provides the representational contract | 6 | `zenodo.21324524`; 28 tests, 13-cell study | P | integrate as contract | scale beyond case study |
| 6 | ProofContext returns verifiable Evidence Bundles, not similar text | 7 | `zenodo.21325288`; MathScopeBench | E | integrate as contract | scale/held-out beyond MathScopeBench |
| 7 | ProofContext serves 0% incompatible near-matches vs 44–75% | 7 | measured on MathScopeBench (dev/test) | E | state as measured, prototype-scale | replicate on larger corpus |
| 8 | Discovery Plane operators generate candidates (not novelty) | 8 | specification only | C | label conceptual | implement; measure yield/diversity |
| 9 | A kernel check is not a correspondence proof | 9 | formal-methods argument | C | new principle, keep | build correspondence-audit lens |
| 10 | search ≠ evidence ≠ certificate ≠ checker; discard the discoverer | 9 | Flyspeck lineage + pilot certificate | M (one instance) | preserve | more certified instances |
| 11 | 812,651-leaf certificate + independent one-page checker | 9,13 | pilot artifact | M | keep as single instance | arXiv/Zenodo the artifact |
| 12 | Epistemic separation of powers (4 clauses) | 10 | v1 contribution; QED independently adopts context separation | M | preserve | — |
| 13 | Fresh-context independence raises defect detection | 10 | pilot n=1 (6 internal passes missed what 1 external caught) | M (n=1) | keep as **hypothesis** | vary reviewer independence (Track B) |
| 14 | Invalidation demotes dependents to SUSPECT automatically | 12 | MIRADOR implements deterministic propagation | P | preserve | — |
| 15 | Log is the single source of truth; all else derived/rebuildable | 12 | event-sourcing + MIRADOR hash-chained log | P | preserve | — |
| 16 | No prior system carries live epistemic state + hard-filter retrieval | 3 | related-work audit (see matrix) | — | keep as delta, **audit-backed** | `RELATED_WORK_MATRIX.md` |
| 17 | FTPR is the primary trust metric; never collapsed into one score | 2,14 | design | C | preserve | compute across campaigns |
| 18 | Engine cannot self-declare R9 (community validation) | 14,15 | constitution (solution defined externally) | C | keep as guardrail | — |
| 19 | No Millennium-solution promise | title, 15 | explicit scope | C | enforce everywhere | — |

## Firstness / novelty claims (guarded)

- The manuscript makes **no unqualified "first" claim**. The delta over prior
  work (row 16) is stated as a *composition* — governed promotion over a
  representation and retrieval layer that carry epistemic state and invalidate on
  it — and is backed by the primary-source matrix, not asserted from abstracts.
- Parametric continuation of branch-and-bound certificates is described as
  "apparently without precedent" only where the pilot manuscript already does so;
  it is a research direction, not a contribution of this paper.
