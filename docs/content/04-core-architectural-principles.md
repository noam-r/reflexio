# Core Architectural Principles

This page defines the foundational rules of the architecture. These principles set the boundaries for every later concept, process, and design decision.

## Purpose

Provide a stable backbone for the project before expanding the model into detailed pages.

## Core Principles

### 1. State is persistent
The system does not treat each interaction as isolated. It maintains a persistent self-state and persistent relationship states over time. Every new event is processed in light of what already exists.

### 2. Events are discrete and traceable
The system processes meaningful occurrences as events. Events may come from external interaction, internal reflection, repair, pattern recognition, or insight. Each event should be identifiable and traceable in history.

### 3. Emotional impact comes from discrepancy
An event does not matter only because of what happened. It matters because of the gap between expectation and actual outcome. The system compares what it expected, wanted, or believed should happen with what actually happened. That gap is the primary source of emotional impact.

### 4. Meaning is assigned through appraisal
Discrepancy alone is not yet emotion. The system interprets the discrepancy through appraisal. This is where the system determines whether an outcome means rejection, respect, unpredictability, threat, validation, fairness, repair, or something else.

### 5. Emotional history is append-only
The architecture does not silently rewrite emotional history. Meaningful emotional consequences are stored as immutable ledger entries. Later reinterpretation adds new entries instead of modifying old ones.

### 6. Current feeling is derived, not simply stored
The system’s present active state is resolved from ledger history. Time, reinforcement, unresolvedness, repair, and other factors determine how much a past entry still contributes now.

### 7. Time changes activation, not historical fact
Past events and past impacts remain part of the record. What changes over time is their present influence. Decay reduces active contribution; it does not erase the fact that an event mattered.

### 8. Reflection may revise meaning without erasing history
Past events can be revisited through echo processing and reflective review. New context, changed relationships, or new patterns may produce later insight. These insights can change current state, but they do so by adding new records rather than rewriting prior ones.

### 9. Relationship context is central
The system does not process events in a vacuum. Relationship state shapes expectation, interpretation, intensity, and replay. The same event may mean something different depending on who it comes from and what the relationship currently is.

### 10. Relationship changes can change the meaning of the past
A past event may be reinterpreted later because the relationship lens has changed. A moment once experienced as insulting may later seem harmless; a moment once ignored may later appear deeply meaningful. This change in understanding is part of the model and must be traceable.

### 11. Local effects can become global effects
Events involving one counterparty can influence the self-state and therefore shape how the system later responds to others. This cross-relationship spillover is deliberate and should be explainable, not accidental.

### 12. Reflection is not denial
The reflective layer should not erase facts or force pleasant interpretations. Its purpose is to examine expectation chains, confidence, meaning assignments, and scope of interpretation in order to support more accurate, proportional, and adaptive processing.

### 13. Better processing is not the same as weaker emotion
A healthier outcome does not always mean less negative emotion. Sometimes better processing means less distortion, less unnecessary self-damage, more appropriate boundaries, or more accurate recognition of unfairness. The goal is adaptiveness and coherence, not artificial positivity.

### 14. Explainability is a first-class requirement
The system should be able to answer why it feels a certain way, why a particular event mattered, what expectation created the discrepancy, and which later reflections altered the present state. Explainability is not an afterthought; it is a design constraint.

### 15. Auditability depends on preserved causality
Every meaningful change in state should remain attributable to specific events, expectations, appraisals, and ledger entries. If current feeling cannot be traced back through its causal chain, the architecture has failed one of its central goals.

## Why These Principles Matter

These principles keep the architecture coherent. Without them, the model would collapse into either a simple mutable mood tracker or an unstructured memory system. The principles ensure that the framework remains persistent, explainable, historically honest, and capable of growth without hidden rewriting.

## How It Connects

This page anchors the rest of the site. The next pages define the concrete objects and mechanisms that implement these principles: the state model, the expectation framework, the ledger, the resolver, and the reflection model.

---
**Previous:** [Concepts and Processes Inventory](03-concepts-and-processes-inventory.md)  
**Next:** [State Model Overview](05-state-model-overview.md)  
**Related:** [Executive Summary](01-executive-summary.md), [Self-State](06-self-state.md), [Emotion Ledger](19-emotion-ledger.md), [Explainability and Auditability](34-explainability-and-auditability.md)
