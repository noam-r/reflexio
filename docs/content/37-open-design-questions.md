# Open Design Questions

This page preserves the major architectural choices that remain unresolved.

## Purpose

Keep the framework honest about what is still undecided and provide a place for future design refinement.

## Core Idea

The architecture is already conceptually strong, but many important choices remain open. These choices should remain visible rather than being buried inside implementation details. Open design questions are not signs of weakness. They are part of the architecture’s future growth.

## Major Open Questions

### 1. Which variables belong in self-state?
The model has described self-state in principle, but the exact list of variables still needs to be chosen carefully.

### 2. Which variables belong in relationship state?
Some dimensions are obvious, but the final relational schema is still open.

### 3. How granular should events be?
The architecture depends on events being discrete, but the right level of granularity still needs refinement.

### 4. How should expectation objects be represented?
The framework distinguishes prediction, desire, and deservedness, but the exact structure of these expectation objects is still open.

### 5. How should discrepancy be quantified?
The conceptual model is clear, but the exact form of discrepancy weighting remains undecided.

### 6. Which appraisal dimensions are essential?
The architecture has named many possible dimensions, but the core mandatory set is still open.

### 7. How should ledger magnitudes be scaled?
The model assumes signed effects, but the numeric or symbolic scale is not yet defined.

### 8. How should the state resolver treat decay and persistence?
The conceptual distinction is clear, but the exact temporal mechanics remain open.

### 9. What should trigger echo processing?
Not every old event should be replayed. Selection logic still needs to be refined.

### 10. What counts as sufficient evidence for reinterpretation?
A later understanding should not become arbitrary. The threshold for insight remains an open design choice.

### 11. How should repair be validated?
Not every apology or positive signal should count as meaningful repair. Criteria still need to be defined.

### 12. How much spillover should be allowed?
Some relationship effects should remain local. Others should become global. The thresholds remain open.

### 13. How expressive should response policy be?
The architecture should shape outward behavior, but the acceptable range of expression still needs careful boundary design.

### 14. Which explanations should be exposed directly?
The system may be able to explain many internal chains, but not every explanation needs to be surfaced in the same way.

### 15. How should the architecture balance realism and usability?
The model aims for emotional continuity, but it should also remain coherent, safe, and useful.

## Why This Page Matters

A system like this can grow in many directions. Keeping the open questions visible helps preserve clarity, prevents premature closure, and creates a roadmap for future design work.

## Design Rule

Unresolved architectural choices should remain explicit until they are deliberately settled.

## How It Connects

This is currently the final page in the first full documentation pass. Future iterations may loop back from here into deeper schema, examples, implementation notes, or testing methodology.

---
**Previous:** [Health and Adaptiveness Criteria](36-health-and-adaptiveness-criteria.md)  
**Next:** none  
**Related:** [Concepts and Processes Inventory](03-concepts-and-processes-inventory.md), [Core Architectural Principles](04-core-architectural-principles.md), [Documentation Site Map](site-map.md)
