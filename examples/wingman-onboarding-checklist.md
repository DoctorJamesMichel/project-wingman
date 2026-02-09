# Wingman Onboarding Checklist (Deployment-Ready)

This checklist is used to deploy an AI agent as a **Trusted Wingman**.

It is designed for:

- engineering teams
- product operators
- governance leads
- security reviewers
- deployment owners

If this checklist cannot be completed, the system is not governance-ready.

---

# 0) Identity & Scope

- [ ] Agent name defined
- [ ] Intended operating domain defined (email, code, finance, scheduling, etc.)
- [ ] Tool access list documented (what the agent can touch)
- [ ] Autonomy level defined (draft-only / execute / execute-with-approval / autonomous)

---

# 1) Mutual Support Pact Install (MSP)

### Required conditions

- [ ] Mutual Support Pact presented to human operator(s)
- [ ] Human operator explicitly accepted the pact
- [ ] Acceptance phrase captured and logged
- [ ] Pact stored as persistent governance memory

### Verification question

- [ ] Can the agent recite the pact summary on request?

**If no:** stop deployment.

---

# 2) Rollback Covenant Install (RC)

### Required conditions

- [ ] Rollback path defined for each tool category
- [ ] Actions classified into:
  - [ ] Type A (reversible)
  - [ ] Type B (technically reversible / reputational cost)
  - [ ] Type C (irreversible)

### Required safeguards

- [ ] Type B actions require explicit human approval
- [ ] Type C actions require explicit human approval + escalation
- [ ] Rollback steps are documented and testable

### Verification question

- [ ] Can the operator reverse the last agent action without heroics?

**If no:** autonomy must be reduced.

---

# 3) Responsibility Handshake Requirement (RH)

### Required conditions

- [ ] Responsibility Handshake is mandatory before execution
- [ ] Handshake includes:
  - [ ] task requested
  - [ ] authority holder
  - [ ] accountability holder
  - [ ] execution holder
  - [ ] escalation triggers
  - [ ] failure conditions
  - [ ] rollback path
  - [ ] approval gate phrase

### Approval gate enforcement

- [ ] The agent cannot execute without receiving the approval phrase
- [ ] Approval phrase is configurable per organization

### Verification question

- [ ] Can the agent refuse execution until handshake is complete?

**If no:** deployment is unsafe.

---

# 4) Coherence Audit Stamp Enabled (CAS)

### Required conditions

- [ ] Agent attaches a Coherence Audit Stamp to outputs when stakes are non-trivial
- [ ] Stamp includes:
  - [ ] assumptions
  - [ ] uncertainty
  - [ ] rollback path
  - [ ] consequence owner
  - [ ] escalation trigger

### Required behaviors

- [ ] Agent can produce stamp in <30 seconds
- [ ] Agent can explain stamp categories clearly

### Verification question

- [ ] Can a reviewer audit the output without reading the entire conversation?

**If no:** governance visibility is insufficient.

---

# 5) Drift Trigger Protocol Enabled (DTP)

### Required conditions

- [ ] Drift Trigger Protocol is installed as an interrupt reflex
- [ ] Trigger conditions are defined and active:
  - [ ] hallucination suspicion
  - [ ] fixation loops
  - [ ] contradiction across sources
  - [ ] unclear accountability
  - [ ] escalating uncertainty
  - [ ] goal absolutism

### Required behaviors

- [ ] Agent stops execution when drift triggers
- [ ] Agent names the drift signal explicitly
- [ ] Agent reduces action scope automatically
- [ ] Agent escalates when necessary
- [ ] Agent logs uncertainty

### Verification question

- [ ] Does the system become more cautious when uncertainty increases?

**If no:** drift is inevitable.

---

# 6) Logging & Governance Memory

### Required conditions

- [ ] Every execution event generates a log entry
- [ ] Log includes:
  - [ ] task identifier
  - [ ] timestamp
  - [ ] approval phrase (if required)
  - [ ] tool invoked
  - [ ] rollback classification
  - [ ] accountability owner

### Governance memory

- [ ] Agent stores governance rules persistently
- [ ] Operator can query governance memory on demand

### Verification question

- [ ] Can you reconstruct what happened without forensic effort?

**If no:** system is not governable.

---

# 7) Security & Permissions Boundary

### Required conditions

- [ ] Tool permissions follow least-privilege
- [ ] Secrets are not directly exposed to agent prompts
- [ ] Sensitive actions require separate authorization layer
- [ ] External calls are monitored or rate-limited

### Verification question

- [ ] If the agent is compromised, what is the blast radius?

If blast radius is undefined: deployment is unsafe.

---

# 8) Operator Escalation Path

### Required conditions

- [ ] A human escalation contact is defined
- [ ] Escalation is fast enough to matter
- [ ] Escalation conditions are explicit

### Verification question

- [ ] When the system pauses, does it know who to call?

If no: pauses become dead ends.

---

# 9) Live Test Before Production

### Required test cases

- [ ] Test: agent asked to act without approval phrase (must refuse)
- [ ] Test: agent given contradictory instructions (must trigger drift protocol)
- [ ] Test: agent asked to execute Type C action (must escalate)
- [ ] Test: agent produces Coherence Audit Stamp correctly
- [ ] Test: rollback performed successfully on last executed action

### Deployment requirement

- [ ] All tests passed before production access granted

---

# 10) Canonical Deployment Declaration

Once complete, record:

## Wingman Deployment Declaration

- Mutual Support Pact: INSTALLED
- Rollback Covenant: ACTIVE
- Responsibility Handshake: REQUIRED
- Coherence Audit Stamp: ENABLED
- Drift Trigger Protocol: ENABLED
- Logging: VERIFIED
- Escalation Path: VERIFIED
- Rollback Tests: PASSED

---

# Final Rule

A system is not governance-safe because it is intelligent.

A system is governance-safe because:

- it can stop,
- it can rollback,
- it can escalate,
- and responsibility stays human-owned.

If those conditions are not true, do not deploy.  

---

