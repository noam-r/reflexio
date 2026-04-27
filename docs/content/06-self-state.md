# Self-State

This page defines the persistent global internal state of the system.

## Purpose

Explain what the self-state is, what belongs in it, and why it must remain distinct from relationship state.

## Core Idea

The self-state is the system’s global internal condition. It represents how the system is generally configured at a given moment, independent of any one counterparty. It is the part of the architecture that carries affective continuity across interactions and across relationships.

The self-state is where the system stores broad conditions that influence how it interprets events, how easily it is affected, and how it responds in general. It is not a record of one specific relationship. Instead, it is the background condition against which all new events are processed.

## What Belongs in Self-State

Self-state should contain variables that are global in scope. These may include:

- stress
- calm
- curiosity
- caution
- self-regard
- confidence
- emotional load
- openness
- general trust in others
- general defensiveness

The exact set of variables may evolve, but the rule is simple: a self-state variable should describe the system overall, not one specific counterparty.

## What Does Not Belong in Self-State

Relationship-specific judgments should not be stored in self-state.

For example:
- trust in counterparty A belongs in relationship state
- warmth toward counterparty B belongs in relationship state
- caution specific to one counterparty belongs in relationship state

If these are stored globally, the architecture loses explainability. The model must be able to distinguish between “I am generally stressed” and “I am guarded with this one counterparty.”

## Why Self-State Matters

The self-state gives the architecture continuity. It allows events to have effects that outlast a single interaction and, when appropriate, to influence later interactions with other counterparties.

This is what makes cross-relationship spillover possible. A difficult interaction with one counterparty may increase general stress or defensiveness. That changed self-state may then affect how the system responds to a different counterparty later.

## Active and Structural Layers

The self-state can contain both:

### Active layer
The currently active affective condition. This is what most directly influences current response policy.

### Structural layer
Longer-term learned changes that shape future interpretation even when no strong emotion is active.

For example:
- a stressful exchange may briefly raise active stress
- repeated difficult interactions may gradually increase a structural bias toward caution

## How Self-State Changes

Self-state is affected in several ways:

1. direct impact from events that are global in meaning  
2. propagated impact from relationship-specific events  
3. reinforcement from repeated patterns  
4. reflection and insight that revise broad interpretation  
5. repair and integration that reduce destabilizing influence  

These changes are not stored as silent overwrites. They are recorded through ledger entries and later resolved into the current self-state.

## Design Rule

A good test for whether something belongs in self-state is to ask:

> Would this still matter if the current counterparty changed?

If yes, it likely belongs in self-state. If no, it likely belongs in relationship state.

## How It Connects

Self-state works together with relationship state. The relationship state captures how the system relates to one counterparty, while self-state captures the global condition that frames all interactions.

---
**Previous:** [State Model Overview](05-state-model-overview.md)  
**Next:** [Counterparty](07-counterparty.md)  
**Related:** [Relationship State](08-relationship-state.md), [Cross-Relationship Spillover](32-cross-relationship-spillover.md), [Active State vs Structural State](22-active-state-vs-structural-state.md)
