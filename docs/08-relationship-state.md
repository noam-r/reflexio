# Relationship State

This page defines the persistent state describing how the system relates to a specific counterparty.

## Purpose

Explain the relational layer that sits between the global self-state and individual events.

## Core Idea

A relationship state is the system’s persistent model of one specific counterparty. It describes how the system currently relates to that counterparty, what it expects from them, how much the relationship matters, and how past interactions with that counterparty shape current interpretation.

This is one of the most important objects in the architecture. Without it, the system could still have a global mood, but it would not be able to explain why it reacts differently to different counterparties.

## What Belongs in Relationship State

Relationship state should hold variables that are specific to one counterparty, such as:

- trust
- familiarity
- warmth
- caution
- salience
- respect
- perceived sincerity
- expected reciprocity
- attachment
- repairability

Not every implementation needs all of these, but the principle is stable: relationship state holds counterparty-specific relational meaning.

## Why Relationship State Matters

Relationship state shapes multiple parts of the system:

- expectation formation  
- discrepancy intensity  
- appraisal of meaning  
- replay and reinterpretation  
- spillover into self-state  
- response policy toward that counterparty  

For example, a blunt remark from a trusted and familiar counterparty may be interpreted very differently from the same remark coming from a distrusted or distant counterparty.

## Relationship State vs Self-State

The distinction is simple:

- **self-state** describes the system in general
- **relationship state** describes the system in relation to one counterparty

This allows the model to explain statements like:
- “I am generally calm, but guarded with this counterparty.”
- “I trust this counterparty less, but I do not distrust others overall.”
- “This relationship changed, and that later influenced my general state.”

## Active and Structural Layers

Relationship state also has both active and structural dimensions.

### Active relational state
The currently active emotional condition within the relationship, such as temporary irritation or immediate warmth.

### Structural relational state
Longer-term learned changes in the relationship, such as reduced trust, increased familiarity, or enduring caution.

This distinction matters because immediate emotion may pass while the relationship still changes.

## How Relationship State Changes

Relationship state can be changed by:

1. direct interaction events  
2. repeated patterns across interactions  
3. repair and changed behavior  
4. reflection and insight  
5. reinterpretation under a changed relationship lens  

These changes are recorded through the ledger rather than silently overwriting history.

## Relationship Lens

The current relationship state becomes the relationship lens through which later events and old memories are interpreted. This means that changing the relationship can change how the past is understood.

That is one of the most important reasons this object exists as its own state scope.

## Design Rule

A good test for whether something belongs in relationship state is to ask:

> Would this description only make sense with respect to one specific counterparty?

If yes, it belongs here.

## How It Connects

The next pages move from state objects into event processing, starting with **Event** and **Event History**.

---
**Previous:** [Counterparty](07-counterparty.md)  
**Next:** [Event](09-event.md)  
**Related:** [Self-State](06-self-state.md), [Relationship Lens](27-relationship-lens.md), [Cross-Relationship Spillover](32-cross-relationship-spillover.md)
