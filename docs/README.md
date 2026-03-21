# Reflexio

An Explainable Affective Ledger Architecture

## What Reflexio is

Reflexio is a conceptual framework for modeling how an interactive system can preserve emotional continuity over time without hiding its internal changes inside opaque mutable state.

The core idea is simple:

- interactions are treated as meaningful events
- events are compared against expectations
- expectation gaps create discrepancy
- discrepancy is interpreted through appraisal
- emotional consequences are written into an append-only ledger
- current state is derived from that history rather than silently overwritten
- past events can later be replayed, reinterpreted, repaired, or integrated without rewriting the past

This makes the model explainable, auditable, and better suited for long-term relational behavior.

## Why it exists

Most systems that try to simulate emotion or tone rely on simple mutable state, short-lived memory, or direct prompt manipulation. That makes it hard to answer questions like:

- Why did this event matter so much?
- Why did the system react differently this time?
- Why did a past interaction still affect the present?
- Why did its interpretation change later?

This project proposes a different approach: preserve the causal chain.

## Core ideas

The framework is built around a few central concepts:

- **Self-State** — the system’s global internal condition
- **Relationship State** — the system’s persistent state with respect to a specific counterparty
- **Expectation** — what the system thinks will happen, wants to happen, or believes should happen
- **Discrepancy** — the gap between expectation and actual outcome
- **Appraisal** — the meaning assigned to that gap
- **Emotion Ledger** — an append-only record of emotionally meaningful effects
- **State Resolver** — the mechanism that derives current active and structural state from history
- **Echo Processing** — replay of past events under current context
- **Insight Events** — new events generated when later understanding changes earlier meaning
- **Reflective Adjustments** — bounded changes that improve processing without denying facts

## Read the docs

A recommended reading path is:

1. [Executive Summary](01-executive-summary.md)
2. [Simply Put](02-simply-put.md)
3. [Concepts and Processes Inventory](03-concepts-and-processes-inventory.md)
4. [Core Architectural Principles](04-core-architectural-principles.md)
5. [Visualization Index](visualizations.md)
6. [End-to-End Processing Flow](35-end-to-end-processing-flow.md)

## Documentation sections

### Introduction
- [Executive Summary](01-executive-summary.md)
- [Simply Put](02-simply-put.md)
- [Concepts and Processes Inventory](03-concepts-and-processes-inventory.md)
- [Core Architectural Principles](04-core-architectural-principles.md)

### Core model
- [State Model Overview](05-state-model-overview.md)
- [Self-State](06-self-state.md)
- [Counterparty](07-counterparty.md)
- [Relationship State](08-relationship-state.md)
- [Event](09-event.md)
- [Event History](10-event-history.md)

### Expectation framework
- [Expectation Framework Overview](11-expectation-framework-overview.md)
- [Expectation](12-expectation.md)
- [Predictive Expectation](13-predictive-expectation.md)
- [Desired Outcome](14-desired-outcome.md)
- [Deserved Outcome](15-deserved-outcome.md)
- [Expectation Confidence, Importance, and Rigidity](16-expectation-confidence-importance-and-rigidity.md)
- [Discrepancy](17-discrepancy.md)
- [Appraisal](18-appraisal.md)

### Ledger framework
- [Emotion Ledger](19-emotion-ledger.md)
- [Ledger Entry](20-ledger-entry.md)
- [State Resolver](21-state-resolver.md)
- [Active State vs Structural State](22-active-state-vs-structural-state.md)
- [Decay, Persistence, and Reactivation](23-decay-persistence-and-reactivation.md)
- [Pattern Detection and Consolidation](24-pattern-detection-and-consolidation.md)

### Reflection framework
- [Reflection and Echo Processing Overview](25-reflection-and-echo-processing-overview.md)
- [Echo Processing](26-echo-processing.md)
- [Relationship Lens](27-relationship-lens.md)
- [Insight Events](28-insight-events.md)
- [Reflective Review](29-reflective-review.md)
- [Reflective Adjustments](30-reflective-adjustments.md)
- [Integration and Repair](31-integration-and-repair.md)

### System behavior and synthesis
- [Cross-Relationship Spillover](32-cross-relationship-spillover.md)
- [Response Policy](33-response-policy.md)
- [Explainability and Auditability](34-explainability-and-auditability.md)
- [End-to-End Processing Flow](35-end-to-end-processing-flow.md)
- [Health and Adaptiveness Criteria](36-health-and-adaptiveness-criteria.md)
- [Open Design Questions](37-open-design-questions.md)

## Visual entry points

If you prefer diagrams first, start here:

- [Visualization Index](visualizations.md)
- [State Model Overview](05-state-model-overview.md)
- [Expectation Framework Overview](11-expectation-framework-overview.md)
- [Reflection and Echo Processing Overview](25-reflection-and-echo-processing-overview.md)
- [End-to-End Processing Flow](35-end-to-end-processing-flow.md)

## Site map

For the documentation structure itself, see:
- [Documentation Site Map](site-map.md)

## Status

This is the first full documentation pass. The current material defines the conceptual architecture and documentation structure. Future iterations can add:
- schemas
- examples
- implementation notes
- test scenarios
- reference datasets
- comparative design alternatives

---
**Start here:** [Executive Summary](01-executive-summary.md)  
**Also useful:** [Visualization Index](visualizations.md), [Documentation Site Map](site-map.md)
