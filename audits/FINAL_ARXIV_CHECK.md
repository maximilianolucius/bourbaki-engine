# Final arXiv checklist — Bourbaki Engine v2 (2026-07-12)

| Check | Status |
|---|---|
| Compiles from a clean environment (`latexmk -C` then `latexmk -pdf`) | ✅ exit 0, 16 pp |
| Undefined references / citations | ✅ 0 (log clean) |
| Cite keys vs `\bibitem` | ✅ 61 keys, 61 bibitems, all resolve |
| Cross-references (`\S`, `\ref`) render (no "??") | ✅ (R3, R4 confirmed) |
| Render-cut displays fixed | ✅ §4 loop and App B state chain now render fully |
| Largest overfull hbox | 3.95 pt (hairline, non-truncating) |
| Every 2026 citation verified against primary source | ✅ `audits/RELATED_WORK_MATRIX.md` (access 2026-07-12) |
| Hallucinated citations | ✅ none found (Aletheia/QED/RMA/TheoremGraph/LeanSearch/MaRDI ids all resolve) |
| Maturity ledger present; no row claims external validation | ✅ Table 1 |
| Table 2 codings ≤ maturity (no unbuilt-as-built) | ✅ fixed post-Congress |
| No Millennium-solution promise (title/abstract/body) | ✅ (R2 confirmed) |
| Engine cannot self-declare R9 | ✅ (R2 confirmed) |
| FTPR primary, never collapsed; estimator + undefined-status stated | ✅ post-Congress |
| Pilot disclaims MIRADOR/ProofContext/operators were implemented during it | ✅ §13 (R3 confirmed) |
| Marketing/budget diction removed | ✅ post-Congress |
| Backup of prior version preserved | ✅ `bourbaki-engine.pre-discovery.tex.bak` |
| Upload archive built | ✅ `bourbaki-engine-arxiv.tar.gz` (self-contained; inline bib, no external assets) |

## Artifact hashes

- `bourbaki-engine.tex` SHA-256 `31486a385ff2d03f7548215804f53e2970a1688e4b1c90287c19e92290dc4dd5`
- `bourbaki-engine.pdf` SHA-256 `9692462b3e5ffdbaa51a1ff937838b7e257f8400713cf2980f33ff6dda04b836`

## Blocking-before-submit (human decisions, NOT auto-fixable)

1. **Second author's affiliation city.** "Instituto Tecnológico de Buenos Aires,
   Córdoba" is geographically inconsistent (ITBA is in CABA). Set on user
   instruction; confirm or correct before submitting.
2. **Companion preprints on arXiv/Zenodo.** MIRADOR and ProofContext are cited by
   Zenodo DOI; if they are to be arXiv cross-references, add the arXiv ids once
   posted. The Bang pilot manuscript (`Lucius26`) is still a private manuscript —
   attach or arXiv it so the pilot evidence is verifiable.
3. **Author list.** Umbrella paper is Lucius + Minich; the two substrates are
   single-author (Lucius). Confirm this is intended.

## Not done (optional, out of scope of "update the paper")

- The `RELATED_WORK_MATRIX.md` autoformalization-faithfulness row is a category
  with no single citable primary source (marked pending); does not affect any
  manuscript claim.
