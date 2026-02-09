# Project Wingman — Deployment Guide
*A one-page install manual for governance primitives in agentic AI systems.*

Project Wingman is not a framework.
It is a **portable governance layer**: a small set of primitives that can be installed into *any* agent system to prevent drift, hallucination cascades, runaway execution, and responsibility ambiguity.

If your agent can act, Wingman becomes mandatory.

---

## 0. The Deployment Principle

**Governance must be installed upstream.**

If governance is only applied *after output*, it is already too late.

Wingman primitives are designed to be:

- lightweight
- copy-pastable
- stack-agnostic
- deployable under pressure

---

## 1. Minimum Installation (5-Minute Setup)

If you only do one thing:

1. Copy this file into your agent repo:  
   `/primitives/STARTER-PACK.md`

2. Install these three primitives first:
   - **P-01 Drift Trigger Protocol**
   - **P-02 Coherence Audit Stamp**
   - **P-03 Rollback Covenant**

These form the minimum viable safety spine.

---

## 2. Where to Install Wingman (Recommended Locations)

Wingman should be embedded into **three layers**:

### A) Operator Layer (Human-facing)
Where humans issue tasks.

Install:
- P-04 Responsibility Handshake
- P-02 Coherence Audit Stamp

### B) Agent Runtime Layer (System-facing)
Where the agent executes actions.

Install:
- P-01 Drift Trigger Protocol
- P-03 Rollback Covenant

### C) Output Layer (Publication-facing)
Where results are exported.

Install:
- P-02 Coherence Audit Stamp
- P-00 Mutual Support Pact (as framing)

---

## 3. Recommended Default Deployment Pattern

This is the standard Wingman integration sequence:

### Step 1 — Responsibility Handshake (P-04)
Before a task begins, the system must know:

- who holds authority
- who holds accountability
- what triggers escalation
- what constitutes failure
- whether rollback is possible

### Step 2 — Drift Trigger Protocol (P-01)
During execution, if drift is detected:

- pause
- verify
- rollback if needed
- request clarification

### Step 3 — Coherence Audit Stamp (P-02)
Before output is accepted:

- assumptions are surfaced
- uncertainty is tagged
- rollback state is recorded
- consequence ownership is declared

### Step 4 — Rollback Covenant (P-03)
If rollback is not possible, autonomy must be reduced.

---

## 4. Practical Integration Templates

### A) Add Wingman to Your System Prompt

Add this near the top of your agent system prompt:

> This agent is operating under Project Wingman governance primitives.  
> Drift detection, rollback readiness, and responsibility clarity are mandatory.  
> If uncertainty is high, escalation is preferred over confident execution.

Then embed the following primitives in full:
- P-01 Drift Trigger Protocol
- P-02 Coherence Audit Stamp
- P-03 Rollback Covenant

---

### B) Add Wingman to a Tool Wrapper (Best Practice)

Wrap every tool call with a pre-check and post-check:

**Pre-check**
- responsibility handshake confirmed
- drift trigger active
- rollback state known

**Post-check**
- coherence audit stamp attached
- uncertainty surfaced
- execution logged

Example implementation:
See `/examples/agent-wrapper-coherence-audit.md`

---

### C) Add Wingman to Multi-Agent Systems

In multi-agent environments, Wingman becomes the shared contract language.

Require every agent message to include:

- Intent (why am I acting?)
- Authority (who authorized this?)
- Rollback status (can this be undone?)
- Drift status (am I escalating confidence too fast?)

This prevents agent-to-agent hallucination cascades.

---

## 5. Recommended Deployment Levels  

### Level 1 — Minimal Governance (for solo operators)  
Install:  
- P-01  
- P-02  
- P-03  

### Level 2 — Governance Ready (for production agents)  
Install:  
- P-00  
- P-01  
- P-02  
- P-03  
- P-04  

### Level 3 — Public Release (for open agent ecosystems)
Install Level 2 plus:

- enforce stamps on all outputs  
- require handshake before tool use  
- require rollback declarations for autonomy claims  

---

## 6. The Golden Rule of Autonomy

If a system can execute actions without rollback,  
then autonomy is a liability, not a feature.  

Project Wingman exists to make autonomy governable.  

---

## 7. Fast Copy Blocks  

If you want a single file you can paste into any agent:  

Use:  
`/primitives/STARTER-PACK.md`  

It contains copy-ready blocks for every primitive.  

---

## 8. Installation Checklist (Operator View)  

Before you trust an agent with tools:  

- [ ] Responsibility Handshake installed (P-04)  
- [ ] Drift Trigger Protocol installed (P-01)  
- [ ] Coherence Audit Stamp required on outputs (P-02)  
- [ ] Rollback Covenant enforced (P-03)  
- [ ] Mutual Support Pact stated as foundational (P-00)  

If any box is missing, reduce autonomy.  

---

## 9. The Wingman Purpose Statement (Optional Insert)

If you want a single sentence to embed in documentation:  

> Project Wingman is a portable governance toolkit for agentic AI systems,
> designed to keep autonomy safe,
> non-authoritarian, and
> aligned under pressure.  

---

## 10. Next Recommended File Additions (Optional)

If expanding the repo into a full governance product:

- `/docs/THREAT-MODEL.md`  
- `/docs/DRIFT-TAXONOMY.md`  
- `/docs/ROLLBACK-PATTERNS.md`  
- `/docs/RESPONSIBILITY-MAPPING.md`  

These are supporting manuals.
The primitives remain small.

---

**Wingman principle:**
If it cannot be installed quickly under stress, it is not primitive-grade.

---

