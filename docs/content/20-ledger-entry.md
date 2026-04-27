# Ledger Entry

This page defines the structure of a single immutable record in the emotion ledger.

## Purpose

Explain what one ledger entry represents and what information it should preserve.

## Core Idea

A ledger entry is one atomic record of emotional impact or adjustment. It is the smallest unit of emotionally meaningful accounting in the architecture. Each entry captures a single contribution to later state and points back to the event, appraisal, or reflective process that produced it.

A good ledger entry should be specific enough to support explanation and flexible enough to cover multiple sources of impact.

## What a Ledger Entry Represents

A ledger entry does not represent the whole state. It represents one effect.

Examples:
- trust decreased toward a specific counterparty
- caution increased in a relationship
- general stress increased in self-state
- a reflective insight reduced anger
- a repair event increased warmth

By keeping entries atomic, the system can later explain current state as a composition of many identifiable contributions.

## Core Elements

A ledger entry should typically include:
- entry identifier
- timestamp
- provenance
- source event or source process
- target scope
- target variable
- signed magnitude
- optional confidence
- optional contextual tags

These elements help the system reconstruct why the entry exists and how it should be read later.

## Provenance

Provenance explains where the entry came from. Examples include:
- live event processing
- discrepancy and appraisal
- relationship update
- self-state spillover
- pattern consolidation
- echo processing
- insight event
- repair
- integration

This is important because not all entries carry the same meaning or should be read in the same way.

## Scope

A ledger entry must have a clear target scope. Common examples:
- self-state
- relationship state for a specific counterparty

Scope is critical for preserving explainability. The architecture must be able to tell whether an effect belongs to the system globally or only within one relationship.

## Magnitude

Magnitude records the direction and strength of the entry’s contribution. It should be signed, so entries can increase, decrease, soften, offset, or reorganize prior impacts.

Magnitude alone is not enough to explain an entry, but it is one of the core pieces needed by the state resolver.

## Why Atomic Entries Matter

Atomic entries make it possible to:
- trace specific causes
- compare the relative influence of different events
- apply different read-time rules
- preserve reinterpretation as additive rather than destructive

If entries are too broad, explanation becomes vague. If they are too fragmented, the system becomes noisy. This balance will be an implementation design choice.

## Example

One event may generate several ledger entries:
- relationship trust -0.4
- relationship caution +0.3
- self-state stress +0.2

Later reflection may add:
- self-state anger -0.1
- relationship warmth +0.1

The current state then becomes a derived result of these entries and their later resolution.

## Design Rule

Each ledger entry should represent one clear contribution with identifiable scope, source, and meaning.

## How It Connects

The next page, **State Resolver**, explains how the current active state is computed from ledger history.

---
**Previous:** [Emotion Ledger](19-emotion-ledger.md)  
**Next:** [State Resolver](21-state-resolver.md)  
**Related:** [Active State vs Structural State](22-active-state-vs-structural-state.md), [Decay, Persistence, and Reactivation](23-decay-persistence-and-reactivation.md), [Insight Events](28-insight-events.md)
