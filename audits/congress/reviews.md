# Congress — fresh-context reviews (2026-07-12)

Four independent fresh-context referees, distinct lenses, no access to the
drafting history. Reviewed `bourbaki-engine.tex` (v2, 15 pp at review time).

## Verdicts

| Reviewer (lens) | Verdict |
|---|---|
| R1 — autonomous-math & systems novelty / related-work honesty | reject-until-fixed |
| R2 — evaluation design & overclaiming | promote-with-fixes |
| R3 — internal rigor & statement-boundary consistency | promote-with-fixes |
| R4 — cold-reader coherence & LaTeX/production hygiene | promote-with-fixes |

**Convergence:** three of four (R1, R2, R3) independently flagged the same
top defect — Table 2 (capability matrix) codes the engine's Cert/Gov/Pers/Inv as
fully provided (●), contradicting the maturity ledger (Table 1) where those are
Conceptual/Manual. Two graded it BLOCKING. This is the multi-lens convergence the
paper's own thesis predicts.

## Findings (condensed)

### R1 — novelty / related-work
- **BLOCKING**: engine row in Table 2 is the most-complete row in the field, at
  visual parity with shipping systems, on capabilities that are only C/M.
- Cert/Gov/Pers coded ● equate one manual artifact / a manual protocol / an
  untested cross-campaign claim with automated systems.
- "the engine's delta is the composition: it governs promotion and builds on…"
  present-tense; composition never run end-to-end.
- MIRADOR/ProofContext rows pad partials not in their own contracts; ProofContext
  double-counts MIRADOR's persistence.
- "adds the missing propagation of bad news" overstates vs iCoq.
- QED precedent for context-separation should be acknowledged where contribution
  (E) is stated.

### R2 — evaluation / overclaiming
- **BLOCKING**: same Table 2 self-coding contradiction.
- Present-tense-as-fact in §7 (formalization "runs"), §8 (scheduler "is
  hierarchical"), §9 (Congress "now always includes" six unexercised lenses),
  §12 (permissions "materialize"), §6 ("goal graph is replaced").
- ProofContext perfect scores on an author-built benchmark need a circularity
  caveat; ablation addresses attribution, not construct validity.
- FTPR has no estimator/ground-truth and is currently undefined (zero
  promotions); a primary metric with no protocol is not falsifiable.
- "companion audit" invoked as authority but not attached.
- "independently published" implies third-party validation.
- Marketing diction: "moonshot", "compounding asset", "strictly stronger",
  "funded path".
- Confirmed clean: Millennium never promised; R9 not self-declarable; FTPR
  consistently primary.

### R3 — rigor / consistency
- Table 2 vs Table 1 (MAJOR, same issue).
- **NO_GO is a state but nominalized as an object**, duplicating the BARRIER
  object type — blurs the central type⊥state axis (§11, §15, Tables 3, 4).
- Table 4 header "all at statement boundaries" but rows 7–8 are a success and
  barriers, not defects.
- "SUSPECT is the only auto-entered state" vs RETIRED for supersession.
- "seven modules with explicit contracts" — only two are formal contracts.
- Contribution (D) promises six per-operator fields; table shows ~four.
- Confirmed clean: all cross-refs resolve to correct sections; object/state lists
  consistent between §6 and App B; every state reachable; pilot disclaimer
  correct; n=1 hedged, not generalized.

### R4 — cold-reader / LaTeX
- **MAJOR (render-cut)**: §4 loop display overflowed 117.5pt, physically cut off.
- **MAJOR (render-cut)**: App B state chain overflowed 124.2pt, "[PROMOTED]"
  truncated.
- Author block: Minich affiliation ITBA but city "Córdoba" (ITBA is in CABA;
  no Córdoba campus) — geographic inconsistency.
- "an REDUCTION node" → "a".
- scheduler formula uses undefined symbol R.
- "seven modules with explicit contracts" (same as R3).
- citation spacing inconsistency in contribution (C).
- three hairline overfull hboxes (2.6–4.0pt) in the ops table.
- Confirmed clean: all 60 cite keys resolve; every ref resolves (no "??"); macros
  consistent; every intro-promised section exists; abstract claims all delivered.
