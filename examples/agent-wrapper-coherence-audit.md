# Agent Wrapper Example — Coherence Audit Stamp

This example demonstrates how to wrap any agent response (or action proposal) with a **Coherence Audit Stamp**.

It is intentionally lightweight and copy/paste ready.

This wrapper is designed to be used in:
- autonomous agent loops
- planner + executor systems
- tool-using assistants
- human + AI delegation workflows

---

## Core Idea

Before an agent acts, the agent must be able to answer:

- What assumptions am I using?
- What uncertainty remains?
- What rollback exists?
- Who holds consequences?

If an agent cannot answer these quickly, it is not safe to proceed.

---

# Minimal Agent Wrapper (Portable Template)

Use this template as the **final output layer** of your agent.

It works even if the agent is running continuously.

---

## OUTPUT FORMAT (MANDATORY)

### Agent Output

**Proposed Action / Answer:**
> [agent writes the output here]

---

## Coherence Audit Stamp (SCL-P.02)

**Assumptions:**
- [list the key assumptions the output depends on]

**Uncertainty:**
- [what is unknown, ambiguous, or unverifiable]

**Rollback:**
- [how this can be reversed, undone, or neutralized if wrong]
- If rollback is impossible, the agent must explicitly say so.

**Responsibility Holder:**
- [who is accountable for consequences: human operator, system owner, agent runtime policy]

**Escalation Trigger:**
- If uncertainty > threshold OR rollback unavailable OR harm risk detected → escalate to human.

---

# Example: Wrapped Agent Response

### Agent Output

**Proposed Action / Answer:**
> I recommend updating the deployment pipeline to require signed approval before tool execution.

---

## Coherence Audit Stamp (SCL-P.02)

**Assumptions:**
- The agent has permission to recommend workflow changes.
- The pipeline supports an approval step.
- Human oversight is available.

**Uncertainty:**
- I do not know whether the current deployment pipeline already has manual gates.
- I do not know whether this system is production-critical.

**Rollback:**
- The approval gate can be disabled or bypassed if it blocks urgent deployment.
- The change can be tested in staging first.

**Responsibility Holder:**
- Human operator / system administrator.

**Escalation Trigger:**
- If this change blocks production workflows → escalate to human immediately.

---

# Implementation Notes

This wrapper can be enforced at 3 levels:

### 1) Soft Enforcement (Recommended for early adoption)
Agent is asked to include the stamp.
Non-compliance is logged.

### 2) Hard Enforcement (Governance Safe)
System rejects agent outputs unless the stamp is present.

### 3) Automatic Enforcement (Best Practice)
System auto-inserts the stamp fields and forces the agent to fill them.

---

# Minimal Runtime Rule

If the agent proposes an action involving:
- money transfer
- message sending
- tool execution
- file deletion
- external API calls
- irreversible operations

Then the Coherence Audit Stamp is mandatory.

---

# Why This Works

The stamp does not make the agent smarter.

It makes the agent:
- slower at the right moments
- transparent about uncertainty
- compatible with rollback governance
- responsibility-aligned under pressure

This is not decoration.

This is the beginning of autonomy governance.

---

# Recommended Pairing

This wrapper pairs naturally with:

- **SCL-P.01 Drift Trigger Protocol**
- **SCL-P.03 Rollback Covenant**
- **SCL-P.04 Responsibility Handshake**

Together they form a minimal safety stack for agentic systems.

---

End of example.  

---

