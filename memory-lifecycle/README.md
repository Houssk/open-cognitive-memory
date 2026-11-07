# Wake–Sleep–Dream Memory Lifecycle

## Status and interpretation

The lifecycle is an experimental computational abstraction for organizing memory operations in OCM. It is inspired by research on memory, consolidation, and generative processing. It is not a literal model of biological sleep, dreaming, or brain function.

`WAKE → ENCODE → ASSOCIATE → SLEEP → DREAM → VALIDATE → WAKE`

## Stage contracts

### 1. WAKE — Retrieval and interaction
**Input:** current task, query, context, and available memory.
**Operation:** retrieve relevant records and make their provenance visible.
**Output:** selected context plus retrieval metadata.
**Evaluation:** relevance, recall, precision, latency, and source attribution.

### 2. ENCODE — Capture
**Input:** new observations or information.
**Operation:** store the source, context, time, and raw or minimally transformed content.
**Output:** provenance-bearing observation records.
**Safeguard:** preserve the distinction between raw input and interpretation.

### 3. ASSOCIATE — Candidate linking
**Input:** new observations and existing graph records.
**Operation:** propose typed relationships, semantic links, temporal links, or candidate abstractions.
**Output:** candidate associations with evidence, confidence, method, and source links.
**Safeguard:** do not promote generated candidates to verified facts automatically.

### 4. SLEEP — Consolidation
**Input:** accumulated records and candidate associations.
**Operation:** apply explicit policies such as deduplication, summarization, clustering, salience estimation, or index maintenance.
**Output:** proposed memory updates and a transformation log.
**Safeguard:** preserve source records and enable rollback or audit.

### 5. DREAM — Generative exploration
**Input:** consolidated memories and unresolved associations.
**Operation:** generate hypotheses, novel links, summaries, or questions for further investigation.
**Output:** speculative candidates separated from established information.
**Safeguard:** label generated content as hypothetical and record the generating model/configuration where relevant.

### 6. VALIDATE — Evidence and consistency checks
**Input:** candidate updates from association, consolidation, or generative exploration.
**Operation:** evaluate provenance, contradictions, task utility, confidence, privacy, and policy constraints.
**Output:** accepted, rejected, deferred, or human-review-required updates.
**Safeguard:** acceptance criteria must be task-specific and inspectable.

## Cross-cutting requirements

- Every operation has a version, timestamp, and reproducible configuration where applicable.
- Updates preserve links to the records from which they were derived.
- Uncertainty and contradiction are representable.
- Personal data access follows consent and retention policy.
- Failed or rejected candidate updates remain auditable without being served as trusted memory.
- The lifecycle may be interrupted, repeated, or partially executed; it need not be a strictly linear process.

## Candidate experiment dimensions

- Append-only memory vs consolidation.
- Retrieval with and without associative links.
- Human-reviewed vs automatic candidate validation.
- Single-pass vs repeated consolidation.
- Retrieval quality vs latency and storage cost.
- Retention of old information vs interference from new information.

## Open questions

- What triggers consolidation?
- Which information should be retained, summarized, or forgotten?
- How should salience be estimated without overfitting to recency?
- How can speculative links be validated?
- Which operations are reversible and which require explicit human approval?

See the lifecycle formalization issue for the next steps.