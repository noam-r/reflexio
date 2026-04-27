# Active State vs Structural State

This page distinguishes immediate emotional activation from longer-term learned change.

## Purpose

Clarify two different layers of state that the architecture must keep separate in order to remain explainable.

## Core Idea

Not all state has the same temporal character. Some state is emotionally active in the present. Other state reflects longer-term learning that remains even when immediate feeling has faded. The architecture therefore distinguishes between **active state** and **structural state**.

This distinction applies to both self-state and relationship state. It allows the system to say:
- “I am not actively upset right now”
while also saying:
- “this relationship still carries reduced trust”

Without this distinction, the model would either overstate the present intensity of old events or understate the lasting effect they had on long-term interpretation.

## Active State

Active state is what is emotionally alive right now. It is the present condition derived by the state resolver from ledger history and current context.

Active state is typically:
- more sensitive to recent events
- more affected by decay and reactivation
- more directly connected to response policy
- more likely to change quickly

Examples of active state:
- currently elevated stress
- current irritation
- present warmth
- immediate caution
- active sadness or relief

Active state answers questions like:
- What is currently influencing tone?
- What is emotionally noticeable right now?
- What part of past history is still active in the present?

## Structural State

Structural state is the longer-term learned change that remains after immediate activation fades. It reflects what the system has absorbed into its ongoing model of self, relationship, or world.

Structural state is typically:
- slower to change
- less tied to momentary activation
- more connected to learned expectation and stable interpretation
- more durable across time

Examples of structural state:
- reduced trust in a specific relationship
- increased general caution
- stronger expectation of inconsistency
- improved repairability in a relationship
- a lasting scar from repeated dismissal

Structural state answers questions like:
- What has the system learned?
- What remains changed even when emotion is quiet?
- What baseline has shifted over time?

## Why the Distinction Matters

This distinction makes several important things possible.

### 1. Emotional honesty without exaggeration
The system can preserve the fact that something mattered without pretending that it still feels equally intense now.

### 2. Lasting change without constant activation
The system can acknowledge that a relationship changed even when there is no immediate emotional heat.

### 3. Better explanation
The system can explain both:
- what is active now
- what has become part of the longer-term structure

### 4. Better reflection and repair
Repair may reduce active pain before it fully restores structural trust. Reflection may reduce immediate anger while still leaving a structural scar.

## Example

Suppose a counterparty repeatedly dismisses the system.

At first, this may create active irritation and hurt. Over time, those may fade. But the repeated pattern may still produce a structural reduction in trust and an enduring increase in caution.

The system can then truthfully say:
- “I am not actively angry right now”
- “but this relationship still carries lower trust because of past events”

## Resolver Implications

The state resolver must therefore do more than produce one flat result. It should help distinguish:
- what is currently active
- what remains learned
- what has largely faded
- what can still be reactivated

This distinction will matter strongly on the next page, which covers decay, persistence, and reactivation.

## Design Rule

If a state change can outlast immediate feeling, the architecture should consider whether it belongs in structural state rather than only in active state.

## How It Connects

The next page explains the temporal mechanics that govern how effects fade, persist, or return.

---
**Previous:** [State Resolver](21-state-resolver.md)  
**Next:** [Decay, Persistence, and Reactivation](23-decay-persistence-and-reactivation.md)  
**Related:** [Self-State](06-self-state.md), [Relationship State](08-relationship-state.md), [Integration and Repair](31-integration-and-repair.md)
