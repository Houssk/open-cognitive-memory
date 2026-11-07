# Open Dataset Strategy

## Goals

OCM datasets should enable comparison, replication, and extension while respecting participant rights, data provenance, and third-party licenses.

## Proposed dataset families

- **Association Norms:** controlled free-association responses with prompt, language, context, and protocol metadata.
- **Cognitive Graph Evolution:** consent-based longitudinal graph snapshots and documented transformations.
- **Human–LLM Associations:** matched association tasks with model/version/prompt metadata and human protocol information.
- **Memory Consolidation Benchmark:** controlled input memories and expected evaluation targets for consolidation strategies.
- **Knowledge Structuring:** source documents or permitted excerpts paired with structured representations and provenance annotations.

These are proposed dataset families, not existing published datasets.

## Dataset specification

Each dataset must document:
- Name, version, maintainers, and contact.
- Purpose and intended use.
- Collection or generation protocol.
- Data provenance and ownership.
- Population, sampling, and relevant exclusions.
- Fields, units, schemas, and annotation conventions.
- Quality checks and known limitations.
- Consent and ethics basis where human data is involved.
- Privacy risk assessment and de-identification methods.
- Access policy, license, retention, and withdrawal process.
- Train/validation/test split policy and leakage controls.

## Privacy baseline

- Personal cognitive graphs and raw responses are private by default.
- Collection must be purpose-limited and data-minimized.
- Informed consent must describe intended processing and possible sharing.
- Public release requires separate explicit consent and a documented risk review.
- Pseudonymization does not guarantee anonymity.
- Do not publish raw personal narratives or inferred sensitive traits by default.
- Define retention, deletion, and withdrawal procedures before collection.
- Restrict access when residual re-identification risk is unacceptable.

## Licenses

Do not select a dataset license until ownership, consent, third-party rights, and applicable legal constraints are understood. Code and documentation licenses do not automatically apply to datasets.

## Dataset card template

1. Dataset overview.
2. Motivation and intended use.
3. Composition and collection.
4. Processing and annotation.
5. Consent, privacy, and ethics.
6. Distribution and licensing.
7. Evaluation splits.
8. Limitations and risks.
9. Maintenance and version history.