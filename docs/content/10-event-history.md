# Event History

This page explains how events are recorded over time independently of later interpretation.

## Purpose

Separate the record of what happened from the later layers that interpret, weight, or emotionally process it.

## Core Idea

Event history is the ordered record of events that have occurred over time. It preserves the factual and structural timeline of the system’s experience. This record should remain distinct from emotional interpretation, because the same event may be understood differently at different times.

The event history answers a simple question:

> What happened, and in what order?

This is different from:
- what it meant
- how strongly it mattered
- how much it still affects current state

Those later questions belong to the appraisal layer, the emotion ledger, and the state resolver.

## Why Event History Matters

Without event history, the architecture loses temporal grounding. The system may still have current state, but it will not be able to clearly reconstruct:
- what sequence of events led there
- what came first and what came later
- which events were reinterpreted
- how insight and repair relate back to original occurrences

Event history is what allows the system to preserve factual order even when emotional meaning changes.

## Event History vs Emotion Ledger

These two records must remain separate.

### Event history
Records that something happened.

### Emotion ledger
Records how that event affected the system.

For example:
- event history may record that counterparty A did not laugh at a joke
- the emotion ledger may record that this created disappointment, self-regard impact, and later reflective adjustment

This separation allows the system to say:
- the event stayed the same
- the emotional interpretation changed

## What Event History Should Preserve

A useful event history should preserve:
- event identifier
- timestamp
- source
- event type
- actual outcome
- structural links to related events where appropriate

It should not collapse into opinion. The event history exists so later processing has a stable reference point.

## Why Order Matters

Order is essential because emotional meaning often depends on sequence.

For example:
- a blunt statement before trust is established may feel harsh
- the same statement after many supportive interactions may feel playful
- an apology after repeated harm means something different from an apology before harm

Without sequence, these distinctions are lost.

## Role in Reflection

The reflection framework depends on event history because replay needs access to past events as they originally occurred. Reflection can add new understanding, but it should not rewrite the sequence itself.

This is especially important for insight events, which must remain distinguishable from the original events that later gave rise to them.

## Design Rule

Event history should preserve stable reference points that later layers can interpret, question, reinforce, or revise without destroying the underlying timeline.

## How It Connects

The next page, **Expectation Framework Overview**, introduces the key idea that emotional impact comes from the gap between what was expected and what actually happened.

---
**Previous:** [Event](09-event.md)  
**Next:** [Expectation Framework Overview](11-expectation-framework-overview.md)  
**Related:** [Emotion Ledger](19-emotion-ledger.md), [Explainability and Auditability](34-explainability-and-auditability.md), [End-to-End Processing Flow](35-end-to-end-processing-flow.md)
