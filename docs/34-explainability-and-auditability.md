# Explainability and Auditability

This page explains what kinds of “why” questions the architecture should be able to answer.

## Purpose

Define the transparency goals of the system and show how the architecture supports traceable causal explanations.

## Core Idea

Explainability is the system’s ability to account for why it currently feels, interprets, or responds in a particular way. Auditability is the system’s ability to trace those explanations back through concrete history: events, expectations, discrepancies, appraisals, ledger entries, and later reflective changes.

These are not optional features. They are core design goals of the architecture.

## Why Explainability Matters

The architecture is built around the idea that emotional processing should not be a hidden black box. The system should be able to answer questions such as:
- why do I feel this way right now?
- why did this event affect me so strongly?
- what expectation made this outcome matter?
- why did my interpretation change later?
- why did I respond more cautiously to this counterparty?
- why does this relationship differ from another one?

These questions are central to the value of the model.

## Why Auditability Matters

Explainability alone is not enough if it cannot be verified against preserved history. Auditability means that explanations should be supported by the architecture’s records.

This includes:
- event history
- expectation state
- discrepancy and appraisal logic
- emotion ledger entries
- insight events
- repair and integration history
- current state resolution

Auditability makes the architecture historically accountable.

## Types of Questions the System Should Answer

A strong architecture should support at least these question types:

### Current-state questions
- Why is stress high right now?
- Why is trust low in this relationship?

### Event-impact questions
- Why did that comment matter so much?
- Which expectation made it painful?

### Change-over-time questions
- Why do I feel differently now than I did then?
- What changed the meaning of that event?

### Behavioral questions
- Why was my response shorter or firmer?
- Why did I become more cautious with this counterparty?

### Cross-relationship questions
- Why did what happened with A affect how I responded to B?

## What Makes an Explanation Good

A good explanation should be:
- specific
- causal
- historically grounded
- proportionate
- understandable

It should identify:
- the relevant event or pattern
- the active expectation
- the discrepancy
- the appraisal
- the resulting ledger effects
- any later reinterpretation or repair

## Example

A good explanation might say:
- I expected acknowledgment with high confidence
- the actual outcome was silence
- this created a strong predictive and normative discrepancy
- I appraised the silence as likely rejection
- that produced entries affecting trust and self-regard
- later reflection softened the rejection interpretation but did not erase the original hurt

This is much stronger than simply saying:
- I felt hurt

## Design Rule

The architecture should preserve enough structure that significant states and behaviors can be traced through a visible causal chain.

## How It Connects

The next page, **End-to-End Processing Flow**, ties the architecture together by walking through the full lifecycle from event to response to later reflection.

---
**Previous:** [Response Policy](33-response-policy.md)  
**Next:** [End-to-End Processing Flow](35-end-to-end-processing-flow.md)  
**Related:** [Emotion Ledger](19-emotion-ledger.md), [Event History](10-event-history.md), [Reflective Review](29-reflective-review.md)
