# Related-work matrix — primary-source audit

**Access date for all URLs: 2026-07-12.** Every 2026 arXiv id below was verified
by fetching the abstract page, not a search snippet. Capability legend:
**Gen**erate · **Retr**ieve · **Form**alize · **Cert**ify (independent
checker/certificate) · **Pers**ist corpus across campaigns · **Gov**ern
promotion (admission gate) · **Inv**alidate dependencies on refutation · build
cumulative **Theory**. Y/P/N = Yes/Partial/No.

## A. Autonomous-mathematics agents

| System | Citation (verified) | Gen | Retr | Form | Cert | Pers | Gov | Inv | Theory | Optimizes |
|---|---|---|---|---|---|---|---|---|---|---|
| Aletheia | Feng, Trinh, Bingham, … (Google DeepMind), *Towards Autonomous Mathematics Research*, arXiv:2602.10177, 10 Feb 2026 | Y | Y | N | **N** | N | N | N | N | NL research proofs; Gemini Deep Think + inference-time scaling |
| QED | An, Ye, Pan, Zhang, *QED: an open-source multi-agent system…*, arXiv:2604.24021, 27 Apr 2026 (v4 rev 26 Jun 2026) | Y | P | N | **N** | N | P | P | N | reliable NL proofs by splitting plan/prove/verify |
| RMA | Zhao, Yuan, Choi, Chen, *RMA: an agentic system for research-level mathematical problems*, arXiv:2605.22875, 20 May 2026 | Y | Y | N | **N** | P | P | N | N | long-horizon proofs; literature grounding + shared memory |
| Prover Agent | Baba, Liu, Kurita, Sannai, *Prover Agent…*, arXiv:2506.19923, 24 Jun 2025 | Y | N | Y | **Y** (Lean) | N | N | N | N | MiniF2F 88.1% / PutnamBench at low sample budget |
| LEAP | Kung, Song, Hwang, … Le, Luong, Peng (DeepMind/UCLA), *LEAP…*, arXiv:2606.03303, 2 Jun 2026 | Y | N | Y | **Y** (Lean) | N | N | N | N | LLM formal solve rate via agentic Lean interaction |
| AlphaEvolve | Novikov, Balog, Vũ, et al. (Google DeepMind), tech report, 14 May 2025 (**not arXiv**) | Y | N | N | P (evaluator) | Y (programs DB) | Y (selection) | N | N | evolutionary code search on an automated objective |
| FunSearch | Romera-Paredes et al., *Nature* 625:468–475 (2023/24) | Y | N | N | P | P | P | N | N | program search discoveries |

## B. Retrieval / knowledge-graph / representation

| System | Citation (verified) | Gen | Retr | Form | Cert | Pers | Gov | Inv | Theory | Epistemic state / hard filter |
|---|---|---|---|---|---|---|---|---|---|---|
| LeanSearch v1 | Gao et al., arXiv:2403.13310, Mar 2024 | N | Y | N | N | N | N | N | N | none; similarity only |
| LeanSearch v2 | Gao, Sun, Jiang, … Dong, arXiv:2605.13137, May 2026 | P | Y | N | N | N | N | N | N | none; nDCG ranking, no hard reject |
| TheoremGraph | Kurgan et al., arXiv:2606.25363, 24 Jun 2026 (11.7M envs, 18.3M cand. deps confirmed) | P | Y | N | N | P | N | N | P | none; cosine linking, LLM-judge matches |
| MaRDI / Bravo MaRDI | Schubotz et al., arXiv:2309.11484, Sep 2023 | N | Y | N | N | Y | P | N | P | none; expert curation gates entries |
| OMDoc / MMT | Kohlhase (OMDoc, Springer 2006); MMT, KWARC | N | P | P | P | Y | N | P | Y | statement roles (conjecture/theorem), no live refutation |
| OpenMath | OpenMath Standard v2.0 rev.2, 2019 | N | N | N | N | N | N | N | N | none (interchange format) |
| MathML | W3C MathML 3.0 2nd ed, 2014 | N | N | N | N | N | N | N | N | none (markup) |

## C. Verification / formalization / truth-maintenance (established lineage)

| Topic | Citation | Note |
|---|---|---|
| Proof-producing SAT/UNSAT | Heule, Kullmann, Marek (SAT 2016); DRAT/LRAT | static certificate + independent checker — the standard the engine adopts |
| Flyspeck / Kepler | Hales et al., *Forum Math. Pi* 5 (2017) e2 | machine-checked; search ≠ proof |
| TMS / ATMS | Doyle (1979); de Kleer (1986) | justification-recording / assumption-based truth maintenance |
| iCoq | Celik, Palmskog, Gligoric (ASE 2017) | invalidates the upward transitive closure of changed entities — mirror of SUSPECT propagation |
| leanblueprint | Massot; Tao (2023) | propagates PROVED (`fully_proved`) UP the ancestor closure — engine adds the missing propagation of BAD news |
| Autoformalization faithfulness | (category, 2025–26) | whether a Lean/Isabelle statement matches the intended informal theorem; **no verified system treats statement–formalization correspondence as a separately audited claim** — this is the engine's Principle (correspondence). Specific citation pending final primary-source confirmation. |

## FLAGS (citation integrity)

- **All draft-cited 2026 arXiv ids RESOLVE and MATCH** their titles: 2602.10177
  (Aletheia), 2604.24021 (QED), 2605.22875 (RMA), 2606.25363 (TheoremGraph),
  2403.13310 / 2605.13137 (LeanSearch v1/v2), 2309.11484 (MaRDI). **No fabricated
  citations were found** — the earlier suspicion about these ids was unfounded.
- **Aletheia**: title is *Towards **Autonomous Mathematics** Research*; first
  author Tony Feng (Berkeley). Fixed in the manuscript.
- **QED version drift**: v1 = 5 problems / 3 correct; v4 = 18 projects / 5
  original works. The manuscript makes no version-specific numeric claim about
  QED, so no correction needed.
- **AlphaEvolve is NOT an arXiv paper** — DeepMind technical report (2025). Cited
  as a report with URL, not an arXiv id.
- **Certification coding**: only Prover Agent and LEAP have a genuine independent
  certificate (Lean). AlphaEvolve = empirical evaluator (Partial). Aletheia / QED
  / RMA rely on LLM self/verifier-agent checking + human experts, which is **not**
  certification (No). The manuscript's certification column and §3 prose enforce
  this distinction.
- **"LeanGraph" is ambiguous**: (a) `patrik-cihal/lean-graph`, a viz tool with no
  paper and no visible license — **not cited**; (b) TheoremGraph's internal formal
  extractor. Not used as an independent citation.
- **OMDoc book record** (LNAI number/year) not confirmed on the page read; OMDoc/MMT
  is discussed in this audit but **not added as a cited row** in the manuscript to
  avoid an unverified bibliographic entry.
- **"Mathematical RAG" has no single primary source**; treated as a category, not
  a citable system. Prover Agent (2506.19923) is the one verified representative.

## Systemic gap (the engine's delta)

Across every verified system: **none carries a live epistemic state
(OPEN/PROMOTED/REFUTED) together with hard-filter retrieval that rejects an
incompatible-but-similar match, under a governed cross-campaign corpus.** The
formal lineage certifies and invalidates but inside one consistent environment;
the agent systems generate and (some) gate but do not persist a governed corpus;
the knowledge graphs persist and retrieve but hold no epistemic authority. The
composition is the contribution.
