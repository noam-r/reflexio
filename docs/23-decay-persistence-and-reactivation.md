# Decay, Persistence, and Reactivation

This page explains how the influence of past emotional impacts changes over time.

## Purpose

Define the temporal mechanics that determine whether a ledger entry remains active, fades, stabilizes, or becomes emotionally alive again.

## Core Idea

An emotional impact does not remain equally active forever. Its present influence changes over time. The architecture therefore needs a temporal model that can explain at least three things:

- how an effect fades
- how an effect remains
- how an effect returns

These are captured here as **decay**, **persistence**, and **reactivation**.

This page is about present influence, not about rewriting history. A ledger entry remains part of history even when its active contribution becomes small.

## Decay

Decay is the reduction of an entry’s active contribution over time.

Decay explains why:
- immediate irritation may soften
- surprise may fade quickly
- acute hurt may lessen
- a recent event may matter less after time passes

Decay should be understood as a read-time property used by the state resolver. It does not mean the event did not matter. It means the entry contributes less to current active state than it did before.

### Important distinction
Decay is not the same as repair, insight, or integration. Those are meaningful changes in interpretation or structure. Decay is simply a reduction in present activation.

## Persistence

Persistence is the tendency of an effect to remain influential over time.

Some entries fade quickly. Others remain influential because they are:
- intense
- repeated
- unresolved
- structurally important
- reinforced by similar later events
- tied to a high-salience relationship

Persistence explains why some impacts remain emotionally or structurally important long after the original event.

Persistence may affect:
- active state
- structural state
- both

## Reactivation

Reactivation is the return of emotional influence from an older entry that had become less active.

An old event may become active again because of:
- a similar new event
- a repeated phrase or pattern
- a change in relationship context
- a reflective replay
- a reminder tied to the same wound or bond

Reactivation is important because emotional material does not always disappear when it becomes quiet. Sometimes it remains latent and becomes active again later.

## Why These Three Must Be Separate

If decay, persistence, and reactivation are collapsed into one vague process, the architecture loses temporal precision.

The system needs to distinguish:
- something is fading
- something is enduring
- something is returning

These are different phenomena with different implications for explanation and repair.

## Example

A dismissive comment may create strong active hurt at first. Over time, the hurt may decay. If no further harm occurs, active pain may become quiet. But if a later event resembles the earlier dismissal, the older entry may reactivate, making the current emotional response stronger than the new event alone would explain.

That history only makes sense if the architecture can distinguish decay from reactivation.

## Temporal Reading vs Historical Record

This page concerns how entries are read in the present, not whether they continue to exist.

- history remains
- present influence changes

This principle is essential for the whole ledger architecture.

## Design Rule

A good temporal model should allow the system to say:
- this mattered a lot then
- it matters less now
- it still changed something
- it can become active again under the right conditions

## How It Connects

The next page moves from individual temporal effects to repeated structures across many events: pattern detection and consolidation.

---
**Previous:** [Active State vs Structural State](22-active-state-vs-structural-state.md)  
**Next:** [Pattern Detection and Consolidation](24-pattern-detection-and-consolidation.md)  
**Related:** [State Resolver](21-state-resolver.md), [Insight Events](28-insight-events.md), [Integration and Repair](31-integration-and-repair.md)
