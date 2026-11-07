# OCM Benchmarks

OCM benchmarks should measure well-defined capabilities, include appropriate baselines, and publish enough detail for independent reproduction.

## Initial tracks

- Associative recall and retrieval.
- Cognitive graph structure and evolution.
- Memory consolidation quality and cost.
- Knowledge structuring and provenance fidelity.
- Human vs LLM association patterns.
- Continual learning, retention, and interference.

## Benchmark requirements

Every benchmark must specify:
- Task definition and intended construct.
- Data source, license, and split policy.
- Inputs, outputs, and reference labels.
- Metrics and aggregation procedure.
- Baseline methods and configurations.
- Leakage and contamination controls.
- Reproducibility instructions.
- Known limitations and failure cases.

## Evaluation principles

Avoid collapsing distinct properties into one opaque score. Report quality, cost, latency, robustness, and uncertainty separately where relevant. Human and model results should only be compared when task conditions and interpretation are defensible.

## Initial metrics to investigate

Depending on the task: precision/recall, ranking metrics, calibration, graph edit distance, edge prediction, temporal consistency, source attribution accuracy, retrieval utility, retention, interference, latency, and storage cost. Metric choice must follow the construct, not convenience.