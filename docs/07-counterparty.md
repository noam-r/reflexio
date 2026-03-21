# Counterparty

This page defines the external actor the system interacts with.

## Purpose

Replace the narrow idea of a “user” with a term that fits the architecture’s relational model.

## Core Idea

A counterparty is any external actor with which the system has interactions that can generate events, expectations, relationship updates, and emotional consequences. The term is intentionally neutral. It does not assume warmth, conflict, equality, or any particular kind of relationship. It simply names the external side of an interaction.

The counterparty matters because the architecture does not only track events in the abstract. It tracks events as coming from someone. That source matters for expectation, appraisal, relationship state, and later reinterpretation.

## Why Not “User”

The term “user” is too narrow for this framework. It suggests a simple application actor rather than a source of relationship, expectation, memory, and interpretation. The architecture needs a term that supports:
- emotional significance
- relationship-specific state
- later reinterpretation under a relationship lens
- cross-relationship comparison

“Counterparty” provides that neutrality without collapsing the model into product language.

## What a Counterparty Enables

Defining a counterparty allows the system to:

- attach a relationship state to a specific external actor
- distinguish one relationship from another
- maintain event history by source
- compare expectations across different relationships
- explain why one event mattered more because of who it came from

The same exact event content may be interpreted differently depending on the counterparty that produced it.

## Counterparty Identity and Continuity

For the model to work well, counterparties must be stable enough to support continuity across time. A relationship state cannot persist unless the system can recognize that later events belong to the same counterparty context.

This does not require a philosophical claim about personhood. It only requires a stable referent for relational memory and state tracking.

## Design Rule

A counterparty is not just a sender. In this architecture, a counterparty is a source of ongoing relational context.

That means the model should not only ask:
- what happened?

It should also ask:
- who did it come from?
- what relationship exists with that counterparty?
- what expectations were active because it came from them?

## How It Connects

The next page, **Relationship State**, explains what the system stores about its evolving relation to a specific counterparty.

---
**Previous:** [Self-State](06-self-state.md)  
**Next:** [Relationship State](08-relationship-state.md)  
**Related:** [Event](09-event.md), [Relationship Lens](27-relationship-lens.md), [State Model Overview](05-state-model-overview.md)
