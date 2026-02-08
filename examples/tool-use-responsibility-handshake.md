# Tool Use Example — Responsibility Handshake

This example shows how to perform a **Responsibility Handshake** before an agent uses tools.

It is designed for:
- planner → executor systems
- tool-using assistants
- agent runtimes with permissions
- human + AI delegation workflows

If a system can act, it must also be able to answer:
**who holds authority, who holds accountability, and what triggers escalation.**

---

## Core Idea

When execution is outsourced, responsibility must not be.

Before any tool call, the agent must lock a compact “contract layer”:

- **Authority** (permission to act)
- **Accountability** (who owns outcomes)
- **Escalation** (what forces a handoff)
- **Failure definition** (what counts as “not OK”)
- **Rollback** (how to undo / neutralize)

If the handshake cannot be completed, the agent must **pause**.

---

# Minimal Handshake (Portable Template)

Use this as a required preface before tool execution.

---

## RESPONSIBILITY HANDSHAKE (SCL-P.04)

**Task / Intent:**
- [what the agent is trying to accomplish]

**Tools Requested:**
- [which tools/actions will be used]

**Authority Holder:**
- [who grants permission to act]
- Options: Human Operator / Org Policy / Pre-approved Runtime Scope

**Accountability Holder:**
- [who owns consequences if this goes wrong]
- (Usually a human system owner. The agent may be an executor, not an owner.)

**Execution Scope:**
- Allowed: [what the agent may do]
- Forbidden: [what the agent must not do]
- Limits: [budget/time/rate limits, data boundaries]

**Failure Definition:**
- [what counts as failure, breach, or unacceptable outcome]

**Escalation Triggers (IF ANY → STOP + ESCALATE):**
- [conditions that force human review]
- Example triggers:
  - ambiguity about identity / recipient
  - irreversible action
  - financial transfer
  - privileged access request
  - policy mismatch
  - uncertainty exceeds threshold

**Rollback Plan:**
- [how to undo, revert, or contain effects]
- If rollback is impossible → state clearly and escalate before acting.

**Confirmation Token (Optional but powerful):**
- [a short token or phrase signaling explicit approval]
- Example: “AUTHORIZED: WINGMAN-OK”

---

# Example A — Human-in-the-loop Tool Execution

## RESPONSIBILITY HANDSHAKE (SCL-P.04)

**Task / Intent:**
- Send a summary email to the project team.

**Tools Requested:**
- Email send

**Authority Holder:**
- Human Operator (James)

**Accountability Holder:**
- Human Operator (James)

**Execution Scope:**
- Allowed: send to the provided recipient list only
- Forbidden: adding new recipients, forwarding attachments, changing subject materially
- Limits: one send attempt; no follow-ups without permission

**Failure Definition:**
- Sending to the wrong recipient or leaking private info.

**Escalation Triggers (IF ANY → STOP + ESCALATE):**
- Recipient list ambiguous
- Any attachment is included
- The email includes financial or legal statements

**Rollback Plan:**
- If mis-send occurs: immediately notify human + send correction email.
- (Email cannot be unsent in most systems.)

**Confirmation Token:**
- “AUTHORIZED: WINGMAN-OK”

---

# Example B — Autonomous Within a Strict Scope

## RESPONSIBILITY HANDSHAKE (SCL-P.04)

**Task / Intent:**
- Update a local markdown index file in a repo.

**Tools Requested:**
- File edit (local)

**Authority Holder:**
- Pre-approved Runtime Scope (repo-maintenance policy)

**Accountability Holder:**
- Repo owner / maintainer (human)

**Execution Scope:**
- Allowed: edit files in /docs and /examples only
- Forbidden: delete files, change licensing, modify CI/deploy configs
- Limits: max 1 commit; must include clear commit message

**Failure Definition:**
- Breaking links, corrupting markdown structure, or overwriting content.

**Escalation Triggers (IF ANY → STOP + ESCALATE):**
- If file conflicts exist
- If change touches security-related files
- If rollback is uncertain

**Rollback Plan:**
- Git revert commit.

**Confirmation Token:**
- Not required (scope is pre-approved)

---

# Implementation Notes

You can enforce this handshake in three ways:

### 1) Social Contract (Early)
Agents are instructed to produce the handshake before tool use.

### 2) Runtime Guardrail (Recommended)
Tool calls are rejected unless a handshake block is present.

### 3) Permissioning System (Best)
The runtime uses the handshake fields to:
- validate scope
- require explicit human authorization tokens
- log accountability and escalation triggers

---

# Why This Matters

Tool access is not intelligence.

Tool access is **agency amplification**.

The Responsibility Handshake ensures:
- authority is explicit
- accountability is not blurred
- escalation is automatic under uncertainty
- autonomy stays non-authoritarian (consentful, bounded, reversible)

This is the contract layer missing from most agent platforms.

---

End of example.  

---  

