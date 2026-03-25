# Modules and Application Patterns

This page explains how Reflexio modules differ from end-user applications.

## Purpose

Define the middle layer between Reflexio's infrastructure and the concrete tools that may be built on top of it.

## Core Idea

Reflexio should support a modular ecosystem.

A **module** is a reusable capability built on the infrastructure. It is not a full application by itself. A module exposes a coherent processing ability that can later be assembled into one or more applications.

An **application** is a concrete product, workflow, or interface that uses one or more Reflexio modules to solve a specific problem.

This distinction allows the same underlying machinery to be reused across many different contexts.

## Modules

Modules are infrastructure-level capabilities such as:
- retrospective reflection
- prospective reflection
- simulation sandboxing
- relationship modeling
- response policy derivation
- insight generation
- audit query resolution

A module should be defined by:
- what inputs it accepts
- what state it reads
- what outputs it produces
- what part of the ledger or resolver it interacts with
- what guarantees it preserves

Modules should remain use-case agnostic wherever possible.

## Applications

Applications are specific compositions of modules around concrete goals.

Examples:
- a retrospective reflection application
- a prospective decision simulation application
- a blended reflection and planning application
- a relational review application
- a journaling interface

Applications may share the same infrastructure and even the same modules while offering very different user experiences.

## Example Separation

### Infrastructure
Reflexio defines expectation, discrepancy, appraisal, ledger, resolver, and reflection rules.

### Module
Prospective Reflection uses those rules to simulate possible future events in a sandbox.

### Application
A salary-negotiation planner or sensitive-conversation planner may use Prospective Reflection as one of its core engines.

This separation keeps the architecture abstract and durable.

## Why This Matters

Without a module layer, the system tends to jump directly from infrastructure to application. That makes the infrastructure harder to reuse and harder to describe cleanly.

With a module layer, Reflexio can support:
- independent capability design
- cleaner interfaces later
- multiple application families built on the same conceptual base
- better future extensibility

## Initial Module Families

A useful first pass on Reflexio module families is:

### Retrospective modules
Used to analyze, replay, reinterpret, repair, and integrate past events.

### Prospective modules
Used to simulate future events, compare scenario branches, and prepare for healthier outcomes.

### Relational modules
Used to manage relationship state, relationship lens, and cross-relationship spillover.

### Output modules
Used to derive response policy, explanations, and audit views.

### Hybrid modules
Used to combine backward-looking analysis with forward-looking simulation.

## Design Rule

A page about Reflexio should specify whether it is describing:
- infrastructure
- a reusable module
- an application example

## How It Connects

After this clarification, the rest of the site returns to the infrastructure itself. Later module pages, such as **Prospective Reflection**, should now be read explicitly as reusable capability modules rather than as fixed applications.

---
**Previous:** [Reflexio as Infrastructure](04a-reflexio-as-infrastructure.md)  
**Next:** [State Model Overview](05-state-model-overview.md)  
**Related:** [Prospective Reflection](38-prospective-reflection.md), [Reflective Review](29-reflective-review.md), [README / Homepage](index.md)
