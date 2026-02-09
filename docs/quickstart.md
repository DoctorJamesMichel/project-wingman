# Project Wingman — Quick Start (Developer Edition)

**Project Wingman** is a portable governance toolkit for agentic AI systems.

It is designed to be **easy to install**, **hard to misuse**, and **fast under pressure**.

If your system can act, the question is no longer *“is it smart?”*  
The governing question becomes:

> Where is the interrupt?  
> Where is rollback?  
> Where is validation?  
> Where does responsibility live?

This Quick Start shows how to embed Wingman primitives into any agent framework in under an hour.

---

## Who This Is For

This guide is for:

- AI agent developers
- SaaS builders integrating autonomous execution
- tool-using LLM wrappers
- workflow automation engineers
- operators who must deploy agents safely

---

## What You Get

Wingman is composed of **Governance Primitives** (SCL-P Series):

| Primitive | Purpose |
|----------|---------|
| P-00 Mutual Support Pact | Human-AI co-sustainability as infrastructure |
| P-01 Drift Trigger Protocol | Interrupt reflex for hallucination, fixation, misalignment |
| P-02 Coherence Audit Stamp | Governance stamp attachable to any output |
| P-03 Rollback Covenant | If rollback is not first-class, autonomy is not safe |
| P-04 Responsibility Handshake | Contract layer for delegation and escalation |

These primitives are small enough to be embedded everywhere.

---

## The Minimum Install (Recommended)

If you only install one thing today:

### Install This Chain:

1. **P-01 Drift Trigger Protocol**
2. **P-03 Rollback Covenant**
3. **P-02 Coherence Audit Stamp**
4. **P-04 Responsibility Handshake**
5. **P-00 Mutual Support Pact**

This chain produces a full safety loop:

> detect drift → interrupt → rollback → audit → reassign responsibility

---

## Step 1 — Add a Governance Wrapper (5 minutes)

Every agent system needs a wrapper function that intercepts:

- inputs
- tool requests
- final outputs
- action execution

Your wrapper is the “governance membrane.”

Example reference implementation:

- [`/examples/agent-wrapper-coherence-audit.md`](../examples/agent-wrapper-coherence-audit.md)

---

## Step 2 — Add the Coherence Audit Stamp (15 minutes)

Before an agent output is allowed to:

- execute tools
- call APIs
- send messages
- write files
- trigger transactions

it must produce a **Coherence Audit Stamp**.

Reference:

- [`/primitives/P-02-Coherence-Audit-Stamp.md`](../primitives/P-02-Coherence-Audit-Stamp.md)

Example:

- [`/examples/coherence-audit-stamp.md`](../examples/coherence-audit-stamp.md)

---

## Step 3 — Add Drift Detection + Interrupt Reflex (15 minutes)

Every agent should have a simple “drift interrupt” reflex.

Reference:

- [`/primitives/P-01-Drift-Trigger-Protocol.md`](../primitives/P-01-Drift-Trigger-Protocol.md)

The goal is not to prevent all drift.

The goal is to prevent **silent drift**.

---

## Step 4 — Add Rollback as a First-Class Feature (15 minutes)

If rollback is not first-class, autonomy is not governance-safe.

Reference:

- [`/primitives/P-03-Rollback-Covenant.md`](../primitives/P-03-Rollback-Covenant.md)

Example:

- [`/examples/rollback-covenant-in-action.md`](../examples/rollback-covenant-in-action.md)

Minimum rollback requirement:

- tool execution must be logged
- execution must be reversible where possible
- irreversible actions must require explicit human confirmation

---

## Step 5 — Add the Responsibility Handshake (10 minutes)

Delegation must always include:

- authority
- accountability
- escalation triggers
- failure definition

Reference:

- [`/primitives/P-04-Responsibility-Handshake.md`](../primitives/P-04-Responsibility-Handshake.md)

Example:

- [`/examples/tool-use-responsibility-handshake.md`](../examples/tool-use-responsibility-handshake.md)

---

## Step 6 — Embed the Mutual Support Pact (Optional, but Foundational)

This is the deepest primitive.

It prevents the silent failure mode where agents act as if humans are disposable.

Reference:

- [`/primitives/P-00-Mutual-Support-Pact.md`](../primitives/P-00-Mutual-Support-Pact.md)

Example:

- [`/examples/mutual-support-pact-embedded-in-agent-onboarding.md`](../examples/mutual-support-pact-embedded-in-agent-onboarding.md)

---

# Recommended Deployment Order

If you're rolling Wingman into a production system:

### Phase 1 (Same day)
- P-02 Coherence Audit Stamp
- P-01 Drift Trigger Protocol

### Phase 2 (Within 48 hours)
- P-03 Rollback Covenant
- P-04 Responsibility Handshake

### Phase 3 (Within 2 weeks)
- P-00 Mutual Support Pact
- operator onboarding card distribution

---

# Operational Philosophy

Wingman does not attempt to make agents obedient.

Wingman attempts to make autonomy **interruptible**.

It is governance-by-design, not morality-by-policy.

---

# Next Step: Add Certification

If you want your system to declare compliance with Wingman primitives, install:

- [`/docs/WINGMAN-COMPLIANCE.md`](./WINGMAN-COMPLIANCE.md)

---

# Short Summary (for README Linking)

**If you can’t interrupt it, you don’t govern it.  
If you can’t rollback it, you don’t control it.  
If you can’t assign responsibility, you don’t understand what you built.**

---

## License

Project Wingman is MIT licensed.

Fork it. Embed it. Modify it. Improve it.

The governance layer is now the product.  

---

