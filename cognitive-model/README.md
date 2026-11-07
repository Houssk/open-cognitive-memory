# Initial Cognitive Model

## Purpose

This document proposes a first conceptual model for representing memory-related information in OCM. It is a starting point for the ontology issue, not a final psychological theory or an assertion that all human knowledge can be represented as a graph.

## Core record classes

### Observation
A captured input from an interaction, task, document, sensor, or participant response. An observation should preserve the original content or a permitted reference to it, its timestamp, context, and source.

### Concept
A semantic unit used to represent an entity, idea, topic, property, or category. Concepts should have stable identifiers and may have labels in multiple languages.

### Episode
A representation of an event or experience situated in time and context. Episodes may contain multiple observations and references to concepts. An episode is not automatically a verified account of what happened.

### Association
A typed, directed or undirected relation between records. Candidate types include:
- semantic similarity or relatedness;
- temporal co-occurrence;
- causal claim;
- part–whole;
- category membership;
- contextual relation;
- participant-declared association;
- model-generated candidate association.

These types have different epistemic status and must not be conflated.

### Source
A record describing where information came from: participant input, a permitted document, an external reference, a model output, or another identified source.

### Derived assertion
A normalized, inferred, summarized, or model-generated statement derived from one or more observations. It must retain links to its inputs and the method that produced it.

## Required metadata

Where applicable, each record should support:
- stable identifier and record type;
- creation time and valid-time interval;
- source and provenance links;
- context and collection method;
- confidence or uncertainty representation;
- epistemic status (observed, participant-reported, externally sourced, inferred, model-generated, reviewed);
- version and transformation history;
- access classification and retention policy.

## Graph model

A cognitive graph is a versioned set of nodes and typed edges. Edges should be first-class records when they need provenance, confidence, temporal validity, or independent review.

Avoid encoding every relation as an unqualified edge. For example, a participant saying that two concepts are associated is different from an algorithm predicting semantic similarity between them.

## Temporal model

OCM should distinguish:
- **event time:** when a described event occurred;
- **observation time:** when the system recorded the information;
- **valid time:** when the information is believed to apply;
- **processing time:** when a transformation or consolidation operation occurred.

This distinction is necessary to represent corrections, changing preferences, evolving knowledge, and retrospective reports without silently overwriting history.

## Uncertainty and contradiction

The model must permit:
- multiple competing assertions;
- explicit unknown or missing values;
- confidence with a documented interpretation;
- source-specific disagreement;
- retraction or supersession without erasing audit history.

A generated association is a candidate, not a fact. Confidence scores must not be presented as calibrated probabilities unless they have been validated for that task.

## Privacy boundary

Personal cognitive graphs are private by default. Access classification, consent scope, retention, and deletion requirements must be represented alongside the data. A graph export must not silently include sensitive personal information or hidden inferences.

## Open design questions

- Which entity and edge types are essential for the first interoperable schema?
- Should observations and assertions share a common envelope?
- Which temporal graph representation best supports versioning?
- How should confidence and epistemic status be encoded?
- Which serialization formats should be supported first?

These questions are tracked through the initial ontology issue.