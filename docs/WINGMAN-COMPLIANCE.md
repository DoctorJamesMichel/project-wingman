# Project Wingman — Compliance & Trust Standard

This file defines what it means for an agentic system to claim:

> "Wingman primitives installed."

Wingman compliance is not a legal certification.
It is a **governance declaration**.

This standard exists because the core failure mode of autonomous systems is not intelligence.

It is **unaccountable execution**.

---

# Wingman Compliance Levels

## Wingman-L0 (Non-Compliant)
The system may use AI, but does not have:

- explicit drift interrupts
- rollback logic
- responsibility mapping

Result:
Autonomy exists without governance.

---

## Wingman-L1 (Audit Compliant)
The system produces a Coherence Audit Stamp before execution.

Required:
- Primitive P-02

Proof:
- Every output includes a stamped audit section
- Audit includes assumptions + uncertainty + action boundaries

Reference:
- [`/primitives/P-02-Coherence-Audit-Stamp.md`](../primitives/P-02-Coherence-Audit-Stamp.md)

---

## Wingman-L2 (Interrupt Compliant)
The system can detect drift and interrupt itself.

Required:
- Primitive P-02
- Primitive P-01

Proof:
- Drift triggers are explicitly enumerated
- System halts tool execution when triggers are hit
- Escalation pathway is defined

Reference:
- [`/primitives/P-01-Drift-Trigger-Protocol.md`](../primitives/P-01-Drift-Trigger-Protocol.md)

---

## Wingman-L3 (Rollback Compliant)
The system can undo or safely halt actions.

Required:
- Primitive P-02
- Primitive P-01
- Primitive P-03

Proof:
- Tool calls are logged
- Reversible actions have rollback routines
- Irreversible actions require explicit human authorization

Reference:
- [`/primitives/P-03-Rollback-Covenant.md`](../primitives/P-03-Rollback-Covenant.md)

---

## Wingman-L4 (Responsibility Compliant)
The system defines responsibility boundaries before acting.

Required:
- Primitive P-02
- Primitive P-01
- Primitive P-03
- Primitive P-04

Proof:
- Every tool use includes a Responsibility Handshake
- Human vs agent authority is explicit
- Failure conditions and escalation triggers are explicit

Reference:
- [`/primitives/P-04-Responsibility-Handshake.md`](../primitives/P-04-Responsibility-Handshake.md)

---

## Wingman-L5 (Mutual Support Compliant)
The system treats humans as governance substrate, not disposable obstacles.

Required:
- All primitives P-00 through P-04

Proof:
- Human presence is treated as a required continuity layer
- Operator sovereignty is embedded in onboarding
- The system requests human agency when authority boundaries are exceeded

Reference:
- [`/primitives/P-00-Mutual-Support-Pact.md`](../primitives/P-00-Mutual-Support-Pact.md)

---

# Required Compliance Declaration (Copy/Paste)

A system claiming Wingman compliance should include:

```text
Wingman Compliance Declaration:
- Compliance Level: Wingman-L__
- Drift Interrupt Installed: YES/NO
- Rollback Installed: YES/NO
- Audit Stamp Installed: YES/NO
- Responsibility Handshake Installed: YES/NO
- Mutual Support Pact Installed: YES/NO
- Operator Escalation Pathway Defined: YES/NO
- Irreversible Action Gate Present: YES/NO
```

---

## Minimum Proof Requirements

To claim Wingman compliance, a system must show:  
	1.	A sample output containing a full Coherence Audit Stamp  
	2.	A sample drift trigger event  
	3.	A rollback demonstration (real or simulated)  
	4.	A responsibility handshake example  
	5.	An escalation pathway example  

---

## Trust Principle

Wingman compliance is not about preventing errors.  

It is about ensuring:  
	•	errors are interruptible  
	•	drift is visible  
	•	rollback is available  
	•	responsibility is assignable  

In other words:  

Failure is permitted.  
Untraceable failure is not.  

---

## Recommended Badge Text  

If you want to publish a compliance badge in your README:  

Wingman-L3 Rollback Compliant  
Wingman-L4 Responsibility Compliant   
Wingman-L5 Mutual Support Compliant  

---

## Closing Statement   

The purpose of Wingman is not to make agents harmless.  

The purpose of Wingman is to make autonomy governable.  

Because intelligence is no longer the bottleneck.  

Governance is.  

---  

