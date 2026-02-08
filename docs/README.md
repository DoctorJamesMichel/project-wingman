# Project Wingman — Documentation

This folder contains the **supporting manual** for Project Wingman.

The primitives are designed to be portable and deployable under pressure.  
The deeper rationale, models, and extended governance scaffolding live here.

If `/primitives` is the toolkit, `/docs` is the field guide.

---

## Quick Navigation

### 1) Start Here (First-Time Readers)

If you are new to Project Wingman, begin with:

- **Root Overview**
  - [`../README.md`](../README.md)

- **Governance Primitives**
  - [`../primitives/README.md`](../primitives/README.md)

---

## The Wingman System Model

Project Wingman assumes a simple reality:

Once an AI system can act in the world, the relevant question is no longer intelligence.

It is governance.

Governance means:
- interrupt capability
- rollback capability
- validation capability
- responsibility location

This repo exists to provide those mechanisms as small installable components.

---

## Core Concepts

### Autonomy Under Pressure
Most failures do not occur during calm reasoning.
They occur during urgency, novelty, and speed.

Project Wingman primitives are designed to remain usable when:
- attention is limited
- context is incomplete
- incentives distort behavior
- systems begin self-amplifying loops

---

### Upstream Responsibility
Human responsibility does not disappear when execution is outsourced.

Instead, it migrates upstream into:
- configuration
- permissions
- delegation boundaries
- rollback access
- validation requirements

Project Wingman is designed to make upstream responsibility visible and enforceable.

---

## Repo Structure Map

### `/primitives/`
The canonical governance elements.

These are intentionally small, reusable, and easy to embed into any agent system.

Start here:
- [`../primitives/README.md`](../primitives/README.md)

---

### `/examples/`
Implementation examples, deployment patterns, and suggested templates.

Examples may include:
- agent prompt wrappers
- human operator checklists
- delegation handshakes
- rollback test harness patterns
- tool authorization scripts (conceptual)

Start here:
- [`../examples/README.md`](../examples/README.md)

---

### `/assets/`
Visual artifacts, diagrams, stamps, cards, and reference images.

This folder exists so that primitives can be deployed not only as text,
but also as portable visuals usable in:
- documentation
- social media posts
- agent training materials
- embedded governance dashboards

---

### `/docs/`
You are here.

This folder holds the expanded conceptual layer:
- threat models
- failure mode taxonomy
- design principles
- governance philosophy
- research references

---

## Suggested Documentation Modules (Planned Expansion)

These are not required for the repo to function, but they are recommended
for future depth and long-term credibility.

### Threat Models & Failure Modes
- What collapses if an agent scales?
- What breaks first?
- What failure modes repeat across systems?

### Drift Taxonomy
A structured list of drift categories:
- hallucination drift
- goal drift
- incentive drift
- social drift
- dialect drift
- confidence drift

### Rollback Patterns
Rollback is not one mechanism—it is a family of mechanisms:
- state rollback
- permission rollback
- behavioral rollback
- memory rollback
- identity rollback

### Responsibility Mapping
A formal method to answer:
- Who authorized this?
- Who can stop it?
- Who owns the consequences?
- Who can reverse it?

### Non-Authoritarian Governance
The central governance thesis of Wingman:
- governance must constrain behavior without domination
- governance must preserve agency without dissolving accountability

---

## How to Use the Documentation Layer

The primitives can be deployed immediately.

The documentation exists for:
- builders who want to implement Wingman in production systems
- researchers who want to formalize agent governance
- educators teaching responsible autonomy
- organizations adopting governance frameworks for tool-enabled AI

If the primitives are "do this now,"
the docs are "understand why this works."

---

## Recommended Reading Order (If You Want the Full System)

1. Root overview: [`../README.md`](../README.md)
2. Primitives overview: [`../primitives/README.md`](../primitives/README.md)
3. Read each primitive file in order (P-00 through P-04)
4. Review examples: [`../examples/README.md`](../examples/README.md)
5. Expand into docs modules as needed

---

## Design Rule (Wingman Law)

If a governance safeguard cannot be applied quickly under pressure,
it is not primitive-grade.

Project Wingman is a repository of primitives.

Everything else is commentary.  

---  

