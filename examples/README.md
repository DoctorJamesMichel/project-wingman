# Project Wingman — Examples

This folder contains **implementation examples** for Project Wingman primitives.

The primitives are designed to be minimal, portable governance elements.
This folder shows how they can be **embedded into real systems**:

- agent frameworks
- operator workflows
- tool permission layers
- enterprise deployments
- prompt templates
- governance dashboards

If `/primitives` is the toolkit, `/examples` is the flight simulator.

---

## Quick Navigation

### Start Here
If you are new to Wingman, read in this order:

1. Root overview  
   - [`../README.md`](../README.md)

2. Primitive index  
   - [`../primitives/README.md`](../primitives/README.md)

3. Then return here to see how primitives are deployed under real conditions.

---

## Core Purpose of This Folder

Project Wingman is not a philosophy repo.

It is a deployment kit.

This folder exists to answer the only question that matters once a primitive is defined:

**How does this get used in production?**

---

## Example Categories (Recommended Structure)

This folder will evolve, but the examples should remain grouped into a few clear categories.

---

### 1) Operator Workflow Examples

These are human-facing workflows used in real time.

Examples may include:
- daily operator startup checklist
- escalation scripts
- “pause before execute” prompts
- drift recognition playbooks
- rollback drills

Goal:
Make upstream responsibility easy for humans to execute.

---

### 2) Agent Prompt Wrapper Examples

These are templates designed to wrap an agent’s behavior.

Examples may include:
- system prompts that force a Coherence Audit Stamp
- embedded Drift Trigger Protocol logic
- Responsibility Handshake prompts before tool use
- rollback confirmation patterns

Goal:
Make governance automatic, not optional.

---

### 3) Tool Authorization Examples

These examples show how to enforce governance through tool design.

Examples may include:
- permission gating schemas
- escalation triggers
- "human confirmation required" logic
- delayed execution patterns
- audit logging prompts

Goal:
Move responsibility upstream into the architecture.

---

### 4) Rollback Implementation Patterns

Rollback is not one action.
It is a governance capability.

Examples may include:
- reversible actions
- transaction logs
- staged execution
- safe-mode fallbacks
- rollback checkpoints
- emergency stop triggers

Goal:
If rollback is not first-class, autonomy is not governance-safe.

---

### 5) Failure Mode / Drift Simulation Examples

These examples intentionally simulate drift scenarios.

Examples may include:
- hallucination cascades
- fixation loops
- recursive goal drift
- dialect contagion
- false certainty escalation

Goal:
Train agents and operators to recognize drift early.

---

### 6) Governance Stamp / Audit Layer Examples

Examples may include:
- output formats with audit stamps attached
- structured "assumption disclosure" templates
- uncertainty labeling patterns
- rollback availability declaration formats

Goal:
Make governance visible and attachable to every output.

---

## Recommended Example Templates (Planned)

These are example modules we should eventually add as discrete files.

### Operator-First Templates
- `operator-startup-checklist.md`
- `operator-drift-response-playbook.md`
- `rollback-drill-template.md`

### Agent Wrapper Templates
- `agent-wrapper-coherence-audit.md`
- `agent-wrapper-responsibility-handshake.md`
- `agent-wrapper-drift-trigger.md`

### Tool Permission Templates
- `tool-permission-contract-template.md`
- `escalation-trigger-matrix.md`

### Deployment Snippets
- `enterprise-deployment-notes.md`
- `multi-agent-governance-loop.md`

---

## What Makes an Example “Wingman-Grade”?

An example belongs here if:

- it is reusable
- it is fast under pressure
- it is easy to copy/paste into real systems
- it clarifies how a primitive becomes operational

If it cannot be applied quickly, it belongs in `/docs`, not `/examples`.

---

## The Wingman Rule for Examples

An example is not complete until it answers:

- **What is the trigger condition?**
- **What is the required interrupt?**
- **What is the rollback mechanism?**
- **What does success look like?**
- **What does failure look like?**
- **Where does responsibility reside?**

---

## Why This Folder Matters

Most governance frameworks fail for one reason:

They are not deployable.

Project Wingman is designed to be forked, embedded, and executed.

This folder ensures the primitives gain legs.

---

## Suggested Reading Path (Full Repo)

1. Root overview: [`../README.md`](../README.md)  
2. Primitives: [`../primitives/README.md`](../primitives/README.md)  
3. Deployment patterns: this folder  
4. Deep rationale: [`../docs/README.md`](../docs/README.md)  
5. Assets: [`../assets/`](../assets/)

---

## Closing Note

The primitives define governance.

The examples prove governance can survive contact with reality.

This is where the toolkit becomes infrastructure.  

---  

