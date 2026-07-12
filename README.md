# The Bourbaki Engine

**A Governed Discovery Architecture for Long-Horizon Autonomous Mathematics.**

An architecture and research-program paper: how autonomous systems can generate,
retrieve, test, formalize, adversarially review, and cumulatively promote
mathematical progress over long-horizon research programs *without allowing
errors to become load-bearing knowledge*.

Its organizing thesis is dual: reliable autonomous mathematics requires two
coupled but institutionally separated systems — a **Discovery Plane** that
expands the space of mathematical possibilities (and may be exploratory,
redundant, speculative, internally contradictory) and a **Trust Plane** that
governs which outputs may become reusable knowledge (conservative, auditable,
controlled by a small explicit trusted computing base). The unit of progress is
not a generated proof but a claim that survives a governed promotion process.

This paper builds on two implemented, separately published substrates:

- **[MIRADOR](https://github.com/maximilianolucius/mirador)** — typed, versioned
  representational substrate (DOI [10.5281/zenodo.21324524](https://doi.org/10.5281/zenodo.21324524)).
- **[ProofContext](https://github.com/maximilianolucius/proofcontext)** —
  dependency-aware retrieval substrate (DOI [10.5281/zenodo.21325288](https://doi.org/10.5281/zenodo.21325288)).

## Build

```bash
latexmk -pdf bourbaki-engine.tex   # 16 pp; TeX Live 2022+, self-contained, no external assets
```

## Contents

| Path | What it is |
|---|---|
| `bourbaki-engine.tex` / `.pdf` | the manuscript |
| `bourbaki-engine-arxiv.tar.gz` | arXiv-ready source archive |
| `SECTION_MAP_AND_CHANGELOG.md` | how this revision maps to the prior claim-promotion paper |
| `spec/ARCHITECTURE_V2.md` | module contracts, object types, epistemic state machine, authority boundaries |
| `schema/module-interfaces.json` | machine-readable interfaces + state-transition table |
| `audits/SOURCE_INVENTORY.md` | files, hashes, provenance |
| `audits/CLAIM_LEDGER.md` | every load-bearing claim, its maturity, and verification owed |
| `audits/RELATED_WORK_MATRIX.md` | primary-source capability/authority audit (2026-07-12) |
| `audits/congress/reviews.md` | four fresh-context adversarial reviews of this draft |
| `audits/RESPONSE_TO_CONGRESS.md` | disposition of every review finding |
| `audits/FINAL_ARXIV_CHECK.md` | pre-upload checklist |

## Status

An architecture and research-program paper grounded in a requirements-elicitation
pilot (Bang's affine plank problem, n=1), with a falsifiable readiness ladder
(R0–R9). Two modules are implemented prototypes; one computation is certified;
governance and the adversarial Congress are so far only manually exercised; the
discovery, formalization, and scheduling planes are specified, not built. See the
maturity ledger (Table 1) — nothing here has yet passed external peer review as a
system. The paper makes **no** promise of solving a Millennium Prize Problem; a
Millennium problem is a gated frontier stress test whose success cannot be
self-declared.

## License

MIT — see [`LICENSE`](LICENSE).
