# Architecture v2 — module contracts, objects, states, authority

Companion specification to the manuscript. Normative for platform documents.

## 1. Planes and authority membrane

```
corpus (Éléments)
  → ProofContext retrieval        [proposes; NO promotion authority]
  → Discovery Plane operators      [proposes candidates; may be wrong]
  → candidate cells/edges
  → Formalization + Certified computation
  → Trust Plane / Congress         [SOLE promotion authority]
  → promoted corpus
  → (loop)
```

Authority is one-way: retrieval and discovery may **propose** nodes and edges;
only the Trust Plane may **promote**. The generating role holds no write access
to the corpus (enforced as DB permissions).

## 2. Module contracts (interfaces only)

### 2.1 MIRADOR — representation (prototype; `zenodo.21324524`)
- **In**: cells and typed edges to store/version.
- **Out**: canonical claim identity = hash(statement + context); object type ⊥
  epistemic state; first-class transformation/reduction edges each with a
  soundness obligation; semantic diffs; NL/computation/proof-assistant links
  recorded (never inferred from compilation); deterministic invalidation over an
  append-only hash-chained event log.
- **Guarantees**: byte-identical rebuild of every derived view from the log.

### 2.2 ProofContext — retrieval (prototype+eval; `zenodo.21325288`)
- **In**: a Problem Signature compiled from a natural-language query.
- **Out**: a typed, hashed Evidence Bundle = {definitions, assumptions,
  exclusions, relevant claims @ exact versions, dependency paths, proofs /
  certificates / formal decls, counterexamples, barriers, provenance manifest,
  epistemic states + warnings}.
- **Invariants**: hard typed-compatibility filters reject incompatible candidates
  regardless of similarity score; **authority membrane** (rank/annotate, never
  promote); version-aware invalidation of indexes and emitted bundles.

### 2.3 Discovery Plane — generation (conceptual)
Operators emit MIRADOR cells in `DRAFT`/`CANDIDATE`; none may emit `PROMOTED`.
Each declares: admissible input · precondition · produced object type · initial
state · required retrieval context · validation obligation · predictable failure.
Operators: `SPECIALIZE`, `GENERALIZE`, `COUNTEREXAMPLE_FIRST`, `NEGATE_AND_SEARCH`,
`DUALIZE`, `CHANGE_REPRESENTATION`, `TRANSFER`, `MINIMAL_MISSING_LEMMA`,
`EXTREMALIZE`, `STABILITY`, `BARRIER_SEARCH`, `FORMALIZE_EARLY`,
`SYNTHESIZE_DEFINITION`.

### 2.4 Formalization + Certified computation (conceptual; one certified instance)
Pipeline: informal → MIRADOR IR → formal decl → proof state → kernel feedback →
localized repair. Every lab output labelled `heuristic` | `evidence` |
`certificate` | `proof`. Statement–formalization correspondence is a **separate
asserted claim**, audited, never inferred from a green kernel.

### 2.5 Trust Plane / Congress (manually exercised)
Roles: Stratège, Scribe, Expérimentateur, Bibliothécaire, Réfutateurs, Auditeur,
Greffier. Promotion requires unanimity; any veto is a **structured object**
{target, concrete objection, affected dependency paths, discharge condition}.
Six standing lenses: correspondence · novelty/priority · retrieval-provenance ·
assumption/scope · checker-independence · integration/invalidation.

### 2.6 Hierarchical scheduler (conceptual)
Three levels: tactical obligations · research programs · meta-program (method
families/representations). Score is a resource heuristic, **never** evidence.
Hard rules: time-boxing, retreat rule, milestone insurance.

## 3. Object types (fixed at creation)

`DEFINITION`, `QUESTION`, `CONJECTURE`, `CLAIM`, `REDUCTION`, `EQUIVALENCE`,
`EXAMPLE`, `COUNTEREXAMPLE`, `BARRIER`, `EXPERIMENT`, `CERTIFICATE`, `CHECKER`,
`HEURISTIC`, `TRANSLATION`, `PROGRAM`.

## 4. Epistemic states and transitions (changed only by logged events)

| From | Event | To |
|---|---|---|
| — | `proposed` | `DRAFT` |
| `DRAFT` | posed to frontier | `OPEN` |
| `OPEN` | `evidence-added` (exact experiment) | `EVIDENCE` |
| `OPEN`/`EVIDENCE` | operator/scribe output | `CANDIDATE` |
| `CANDIDATE` | kernel check + correspondence asserted | `FORMALIZED` |
| `FORMALIZED` | Congress lenses discharged | `AUDITED` |
| `AUDITED` | unanimous promotion | `PROMOTED` |
| any | counterexample on record | `REFUTED` |
| `OPEN` route | impossibility proved | `NO_GO` |
| `PROMOTED` | dependency refuted/definition revised | `SUSPECT` *(automatic, only auto-entry)* |
| `SUSPECT` | re-audit through Congress | `PROMOTED` or `REFUTED` |
| any version | superseded by new version | `RETIRED` |

**Orthogonality**: object type and epistemic state are independent axes. A
`CONJECTURE` may be `PROMOTED` (as a conjecture); a `CLAIM` labelled "Theorem"
in prose may sit at `DRAFT`. The literary label is intent; the state is evidence.

## 5. Invariants audited on the graph

- **Acyclicity of justification**: no node reachable from its own obligations.
- **Definition–proof consistency**: object named in a statement is hash-identical
  to the object manipulated in its proof.
- **Edge soundness**: every `REDUCTION`/`EQUIVALENCE`/`TRANSLATION` edge discharges
  its obligation before either endpoint is promoted through it.
