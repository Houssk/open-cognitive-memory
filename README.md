# Open Cognitive Memory (OCM)

**An open research framework for human cognition, associative memory, knowledge representation, agent memory, and continual learning.**

Open Cognitive Memory (OCM) is an open-source research initiative exploring how knowledge and experience are encoded, associated, structured, consolidated, retrieved, and updated over time — in humans and artificial systems.

The project brings together cognitive science, memory research, knowledge graphs, information retrieval, agent architectures, and continual learning. It aims to create shared concepts, reproducible experiments, open datasets, and measurable benchmarks.

> OCM is a research programme, not a claim that human cognition can be fully replicated by a single computational model.

## Research scope

- **Human cognition:** memory, learning, recall, forgetting, and individual knowledge structures.
- **Associative memory:** free association, spreading activation, semantic relationships, and retrieval.
- **Knowledge representation:** concepts, relations, episodes, temporal context, uncertainty, and provenance.
- **Agent memory:** episodic and semantic memory, memory selection, retrieval, and external memory systems.
- **Continual learning:** incremental knowledge acquisition, consolidation, interference, and adaptation.
- **Open science:** protocols, datasets, benchmarks, reproducibility, and community review.

## A working lifecycle abstraction

OCM uses the following lifecycle as an initial organizing model:

`WAKE → ENCODE → ASSOCIATE → SLEEP → DREAM → VALIDATE → WAKE`

- **Wake:** retrieve relevant knowledge and interact with the environment.
- **Encode:** capture observations, experiences, and information with context and provenance.
- **Associate:** connect new information to existing concepts, episodes, and relations.
- **Sleep:** run consolidation processes over accumulated memories.
- **Dream:** explore candidate connections, abstractions, and hypotheses.
- **Validate:** assess candidate updates for evidence, consistency, utility, and provenance.

This is an experimental computational abstraction inspired by research on memory and consolidation. It does **not** claim that biological sleep or dreaming is equivalent to an AI processing cycle.

## Research principles

1. **Evidence before analogy.** Distinguish empirical findings, theoretical interpretations, and engineering hypotheses.
2. **Operational definitions.** Define constructs in terms that can be observed, annotated, or measured.
3. **Reproducibility.** Publish protocols, evaluation procedures, baselines, and limitations.
4. **Pluralism.** Compare multiple representations and algorithms instead of assuming one architecture is universally best.
5. **Provenance.** Preserve the origin, context, confidence, and transformation history of information.
6. **Privacy by design.** Personal cognitive data is private by default and is never made public without explicit, informed consent.
7. **Open collaboration.** Welcome contributions from cognitive science, neuroscience, psychology, information science, and AI engineering.

## Initial research hypotheses

- Spontaneous associations may reveal aspects of an individual's knowledge organization that standard questionnaires do not capture.
- Longitudinal cognitive graphs may represent changes in knowledge and interests over time.
- Explicit consolidation may improve retrieval quality, consistency, or storage efficiency in some settings.
- Human and language-model association patterns may differ in measurable ways.
- Provenance-aware representations may improve the reliability of knowledge reuse.
- Shared evaluation protocols can help compare graph-based, retrieval-based, parametric, and hybrid memory systems.

These are hypotheses to test, not established conclusions.

## Repository map

- `research/` — foundations, related work, hypotheses, questions, bibliography.
- `cognitive-model/` — concepts, associations, episodic and semantic memory, time, ontology, provenance.
- `memory-lifecycle/` — lifecycle stages and candidate operations.
- `research-programs/` — human cognition, agent memory, continual learning, knowledge structuring.
- `datasets/` — specifications, protocols, annotations, synthetic data, dataset cards.
- `benchmarks/` — evaluation tasks and metrics.
- `experiments/` — reproducible experiment proposals and results.
- `applications/` — possible applications built on validated components.

## Getting involved

Start with [CONTRIBUTING.md](CONTRIBUTING.md), review the open [issues](https://github.com/Houssk/open-cognitive-memory/issues), or open a discussion for a research question.

Contributions can include literature reviews, protocol design, ontology proposals, datasets, baselines, benchmark implementations, critical reviews, and documentation.

## Privacy and data governance

Cognitive and personal-memory data can reveal sensitive information. OCM therefore separates open-source software from permission to collect, process, or publish personal data.

- Personal-level data must remain private by default.
- Collection requires a clear purpose and informed consent.
- Public release requires separate, explicit consent and a documented risk review.
- De-identification is not treated as a guarantee against re-identification.
- Every dataset must have a dataset card, provenance record, access policy, and license.
- Contributors must not upload identifiable or sensitive personal data without authorization.

See [GOVERNANCE.md](GOVERNANCE.md) and [DATASET_STRATEGY.md](datasets/DATASET_STRATEGY.md).

## Licensing

The initial proposal is:
- Software and code: **Apache-2.0**
- Documentation: **CC-BY-4.0**
- Datasets: licensed individually according to provenance, consent, third-party rights, and applicable restrictions.

Dataset licensing must be reviewed separately before publication. The software license does not grant rights to personal or third-party data.

## Status

OCM is in its foundation phase. The first milestones are to establish shared vocabulary, map existing research, define an initial ontology, formalize testable hypotheses, and agree on dataset and benchmark standards.

## Citation

A formal citation will be added once the project has a stable research release.