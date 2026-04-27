# Simulation Sandbox

This page defines the temporary infrastructure space used to model hypothetical futures without polluting real history.

## Purpose

Explain how Reflexio can simulate future events safely without treating imagined outcomes as actual history.

## Core Idea

A simulation sandbox is a temporary, non-historical workspace where Reflexio modules can model hypothetical future events and their projected consequences. It exists so the system can reuse the same reasoning principles as the main architecture without inserting imagined futures into the real event history or emotion ledger.

This distinction is essential. Real history records what happened. The sandbox models what could happen by storing projected outcomes and projected consequences.

## Why a Sandbox Is Needed

If simulated futures were inserted directly into the real ledger, the architecture would lose one of its central guarantees: historical honesty.

The sandbox prevents that by separating:
- actual events
from
- hypothetical branches

This allows Reflexio to explore possible outcomes while preserving the integrity of the real event history and emotion ledger.

## What the Sandbox Contains

A simulation sandbox may contain:
- a proposed future event
- a current expectation model
- current self-state and relationship state used as starting context
- multiple scenario branches
- projected outcomes
- projected discrepancies
- projected appraisals
- projected emotional and relational effects

These projections are temporary and comparative, not historical truth.

## Sandbox vs Real Ledger

The real ledger answers:
- what affected me?

The sandbox answers:
- what might affect state if this branch occurs?

That is the key distinction.

## Why This Improves Decision Support

The sandbox allows Reflexio to help with decisions such as:
- whether to take action
- how to frame a difficult conversation
- what risks are worth taking
- what fears are exaggerated
- how to prepare for the most adaptive path

Because the sandbox can compare branches side by side, it supports clearer decision-making than a single imagined future.

## Example

Suppose the user is considering asking for a raise.

The sandbox can create branches such as:
- ask directly now
- first ask for feedback and timing
- delay the conversation
- avoid the conversation entirely

Each branch can then be evaluated for:
- likely emotional discomfort
- likely relational effects
- likely self-respect outcome
- likelihood of regret
- likely discrepancy between hope and reality

## Design Rule

The simulation sandbox should preserve a strict boundary between projected futures and actual recorded history. Projected outcomes are not actual outcomes and must not be treated as such by the real ledger.

## How It Connects

The next page defines how the sandbox explores multiple possible paths through **Scenario Branches**.

---
**Previous:** [Prospective Reflection](38-prospective-reflection.md)  
**Next:** [Scenario Branches](40-scenario-branches.md)  
**Related:** [Emotion Ledger](19-emotion-ledger.md), [End-to-End Processing Flow](35-end-to-end-processing-flow.md), [Open Design Questions](37-open-design-questions.md)
