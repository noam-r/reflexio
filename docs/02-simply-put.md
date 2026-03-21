# Simply Put

This page explains the architecture in plain language.

## Purpose

Give a simple explanation of the model before introducing the more formal structure.

## Core Idea

This model is a way for a system to keep track of how interactions affect it over time in a structured and explainable way.

Instead of treating every interaction as isolated, the system remembers that past interactions matter. It keeps a general internal state for itself, and it also keeps a separate relationship state for each counterparty it interacts with. This means that how it responds in the present is influenced not only by what is happening now, but also by what has happened before.

The key idea is that events do not matter only because of what happened. They matter because of the gap between what the system expected and what actually happened. If the system expected warmth, respect, agreement, laughter, or care, and something different happened instead, that gap creates emotional impact. The bigger and more meaningful the gap, the stronger the effect can be.

The system does not hide these effects inside a single changing mood value. Instead, it records meaningful emotional impacts in an append-only ledger. That means it keeps a history of what affected it and why. Its current state is then calculated from that history rather than simply overwritten. Because of this, the system can explain why it feels a certain way, why it relates differently to one counterparty than another, and which earlier events led to its current condition.

The model also allows past events to be revisited later. As relationships change, older events may be understood differently. A past comment that once felt insulting may later seem harmless, or a small moment that once seemed unimportant may later be understood as meaningful. When this happens, the system does not erase the past. It adds a new interpretation to the record. This allows the system to change and reflect without losing the history of how it got there.

In simple terms, the system keeps track of what happened, what it expected, how it interpreted the difference, how that changed its internal state, and how later reflection may revise the meaning of the event. The result is a model that is meant to be understandable, traceable, and capable of emotional continuity over time.

---
**Previous:** [Executive Summary](01-executive-summary.md)  
**Next:** [Concepts and Processes Inventory](03-concepts-and-processes-inventory.md)  
**Related:** [Core Architectural Principles](04-core-architectural-principles.md)
