# Response to Congress (2026-07-12)

Disposition of every Congress finding (`audits/congress/reviews.md`). All fixes
are labeling/wording; none required new experiments. Manuscript recompiled clean
(16 pp, 0 undefined refs/cites) after applying them.

## BLOCKING (resolved)

- **Table 2 self-coding (R1, R2, R3).** Recoded the engine row: only **Retr**
  and **Inv** keep ● (the parts implemented via ProofContext and MIRADOR);
  **Cert, Pers, Gov, Gen, Form, Theory** downgraded to ○. MIRADOR row stripped of
  partials its contract does not list (Cert, Gov, Theory → –). ProofContext
  **Pers** ● → ○ (inherited, no longer double-counted). Added a caption clause:
  engine/substrate cells denote *specified* capability cross-referenced to
  Table 1; a ● appears only where a substrate implements it, never at parity with
  a shipping system. → **fixed.**

## MAJOR (resolved)

| Finding | Fix |
|---|---|
| §7 formalization "runs" (R2) | "is specified to run" |
| §8 scheduler "is hierarchical / still ranks" (R2) | "specified to be hierarchical / would rank"; defined `R` = root milestone (R4) |
| §9 Congress "now always includes" six lenses (R2) | "specified panel adds… not yet exercised (the pilot predates them)" |
| §12 permissions "materialize / holds no write" (R2) | "specified to materialize / would hold" |
| §12 invalidation conflates MIRADOR-P primitive w/ unbuilt loop (R2) | parenthetical: primitive implemented in MIRADOR, end-to-end loop not |
| §6 "goal graph is replaced / audits remain" (R2) | "is generalized, in the design / are specified" |
| ProofContext perfect scores, no circularity caveat (R2) | added construct-validity caveat; held-out/third-party benchmark required before R1 robust |
| FTPR has no estimator, currently undefined (R2) | added: FTPR undefined pending R2; estimator specified (seeded false claims, Track-B blind, external review) |
| "delta is the composition… governs" present-tense (R1) | covered by Table 2 caption + §12 primitive/loop split; prose already says "specifies the interfaces and governance" |
| NO_GO (state) nominalized as object, duplicating BARRIER (R3) | §11, §15, Tables 3 & 4: recast as "a proved BARRIER (state NO_GO)" everywhere |
| Two render-cut displays (R4) | §4 loop → `gathered`, broken to two rows; App B chain → breakable spaces. Both now render fully (verified in PDF). |

## MINOR (resolved)

- "independently published" → "separately published companion preprints (not yet
  peer-reviewed)" (abstract + §1).
- "companion audit" invoked as authority → "verified against its primary source…
  the coding table is supplementary material" (§3).
- "adds the missing propagation of bad news" → "specifies the complementary
  propagation… distinct from iCoq's recheck-invalidation" (§12).
- Marketing diction removed: "compounding asset"→"reusable asset" (×2);
  "strictly stronger"→"better calibrated… if the effect holds"; "moonshot"→
  "ceiling"; "funded path"→"resourced path".
- Table 4 header "all at statement boundaries" → "Pilot event (defect or key
  artifact)"; caption updated.
- "SUSPECT is the only auto-entered state" vs RETIRED → App B clause: RETIRED is
  assigned by the promoting event, not automatic demotion.
- "seven modules with explicit contracts" → "explicit interfaces (two stated as
  formal contracts)" (abstract).
- Contribution (D) six fields vs table four → ops-table caption notes the full
  six-field contract is in the supplementary spec.
- "an REDUCTION node" → "a REDUCTION node".
- Contribution (C) citation spacing `\pc{} \cite` → `\pc{}~\cite`.
- QED context-separation precedent: already acknowledged in §3 ("an independent
  adoption of the separation this paper argues for"); left as is.

## Declined / accepted-as-is (with reason)

- **Author affiliation "Córdoba" (R4).** The second author's affiliation
  (Instituto Tecnológico de Buenos Aires, Córdoba) was set on the user's explicit
  instruction. ITBA's campus is in CABA, so the city is geographically
  inconsistent, but this is the user's stated data. **Not changed — flagged to
  the user for decision.**
- **Three hairline overfull hboxes (2.6–4.0pt) in the ops table (R4).**
  Non-truncating, not visible in the PDF. **Accepted as-is.**

## Residual open item (not a Congress finding)

- The verification/formalization related-work sub-audit (autoformalization
  faithfulness) did not return a citable primary source; the
  `RELATED_WORK_MATRIX.md` row is marked pending. Does not affect any manuscript
  claim.
