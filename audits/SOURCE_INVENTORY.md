# Source inventory — Bourbaki Engine v2

Generated 2026-07-12. Phase 0 of the reorientation protocol
(`07_PROMPT_CLAUDE_ADECUAR_BOURBAKI_ENGINE_DISCOVERY_ARXIV.md`).

## Manuscript artifacts (this directory)

| File | Role | SHA-256 |
|---|---|---|
| `bourbaki-engine.tex` | v2 source (governed-discovery reorientation) | `2e04883adebf6be1d7b3f55c05494e77ff1ef907b1253baf6c368b112cef52aa` |
| `bourbaki-engine.pdf` | v2 compiled, 15 pp | `32ba287668bba8ff2418ded74679ee825445c35de01729b9de2258060c8b6aa5` |
| `bourbaki-engine.pre-discovery.tex.bak` | v1 source (claim-promotion paper), preserved | `11951ff5d03e0595976512984184dec223100fa9ca352493bc6f0aff442dfaef` |
| `bourbaki-engine.pre-claimpromotion.tex.bak` | earlier draft, preserved | (unchanged from repo) |

The prompt's declared input PDF (`bourbaki-engine(3).pdf`, SHA-256
`59c58615dec75d8ba4f8a61f09bc30076c66d356dc1fb3425fe69256d5b0e9c3`) is
**byte-identical** to the pre-discovery compiled PDF that this revision started
from — i.e. the reorientation was applied to exactly the version the prompt
targeted (authors Lucius + Minich, two-stage validation plan with USD budgets).

## Prompt / planning documents consumed

- `07_PROMPT_CLAUDE_ADECUAR_BOURBAKI_ENGINE_DISCOVERY_ARXIV.md` — master reorientation prompt (executed).
- `01_REORIENTACION_BOURBAKI_ENGINE_MILLENNIUM.md` — strategic diagnosis (read).
- `02_PROMPT_CLAUDE_FABLE_REORIENTACION.md` — earlier reorientation prompt (present, not separately executed).
- `03_REFUNDACION_OPERATIVA_DE_LA_MATEMATICA.md`, `04_MATHRAG_CONOCIMIENTO_MATEMATICO.md` — **NOT PRESENT** in the tree; their content is covered by the MIRADOR / ProofContext papers below.

## Companion substrates (sibling repositories, verified)

| Module | Repo | Paper | DOI | Maturity |
|---|---|---|---|---|
| MIRADOR (representation) | `~/PycharmProjects/VS/mirador` | `paper/mirador-typed-versioned-ir.tex` | `10.5281/zenodo.21324524` | prototype + 13-cell Bang case study, 28 deterministic tests |
| ProofContext (retrieval) | `~/PycharmProjects/VS/proof-context` | `paper/proofcontext-dependency-aware-retrieval.tex` | `10.5281/zenodo.21325288` | prototype + controlled eval on MathScopeBench |

Both are single-authored (Lucius) and already cite the Bourbaki Engine as their
governance companion. The v2 paper cites both by DOI and states their maturity
in Table 1 rather than reproducing their content.

## Pilot artifact referenced (not in this tree)

- Bang manuscript `Lucius26` (35 pp) + `812,651`-leaf exact-rational certificate
  and independent checker — repository `maximilianolucius/bang-plank-affine-triangle`.
  Not yet on arXiv / not journal-accepted (hence maturity ledger row M for
  certified computation, no external-validation column).
