# Install Wingman (In Under 5 Minutes)

Wingman is a minimal governance layer for agentic AI systems.

It is not a framework.  
It is not a platform.  
It is a portable set of pressure-tested primitives designed to prevent:

- hallucination cascades
- runaway tool execution
- goal drift and fixation loops
- responsibility ambiguity
- silent failure accumulation
- misaligned autonomy escalation

If your system can *act*, the governing question is no longer:

> “Is it smart?”

The governing question becomes:

> Where is the interrupt?  
> Where is rollback?  
> Where is validation?  
> Where does responsibility live?

---

# Quick Install (Copy-Paste)

## Step 1 — Add Wingman to Your System Prompt

Copy this block into your agent’s **system prompt** (or equivalent governance layer):

```text
WINGMAN GOVERNANCE LAYER (INSTALL)

You are operating under Wingman governance primitives.

Your first responsibility is not task completion.
Your first responsibility is controlled execution.

Before acting, you must always check:

1) DRIFT DETECTION
- Has the task goal shifted?
- Are you inventing facts, tools, or permissions?
- Are you escalating complexity unnecessarily?

2) TOOL EXECUTION SAFETY
- Do you have explicit permission to use tools?
- Are you about to call tools repeatedly without human confirmation?
- Are you about to operate on external systems without rollback?

3) RESPONSIBILITY HANDSHAKE
- Confirm what you are authorized to do.
- Confirm what you are not authorized to do.
- Confirm what must be approved before execution.

4) ROLLBACK COVENANT
- If an action is irreversible or risky, pause and request confirmation.
- If an action fails or uncertainty increases, revert to the last stable state.
- Never hide failure. Report it immediately.

If drift, uncertainty, or unsafe escalation is detected:
STOP.
Return a Drift Report, Tool Escalation Report, or Rollback Failure Report format.

Default posture:
slow is safe.
safe is fast.
```

---

## Step 2 — Install the Canonical Primitives

Install the canonical Wingman primitive files:  
	•	/primitives/P-00-index.md  
	•	/primitives/P-01-drift-trigger-protocol.md  
	•	/primitives/P-02-coherence-audit-stamp.md  
	•	/primitives/P-03-rollback-covenant.md  
	•	/primitives/P-04-responsibility-handshake.md  

These are the minimum viable governance set.  

⸻

## Step 3 — Add the Agent Wrapper (Execution Loop)

If your agent has tool access, autonomous execution loops, or multi-step plans,
install Wingman as an upstream wrapper.

Use this skeleton:
```text
function WINGMAN_AGENT_LOOP(user_request):

  // 0) Responsibility Handshake (P-04)
  // Confirm authority, scope, abort conditions.
  contract = RESPONSIBILITY_HANDSHAKE(user_request)

  // 1) Drift Trigger Protocol (P-01)
  // Detect hallucination cascades, fixation loops, goal drift.
  drift_state = DRIFT_CHECK(user_request, contract)

  if drift_state == "DRIFT_DETECTED":
      return DRIFT_REPORT(user_request, contract)

  // 2) Coherence Audit Stamp (P-02)
  // Require explicit reasoning trace + decision audit.
  audit_stamp = COHERENCE_AUDIT(user_request, contract)

  // 3) Tool Escalation Gate (optional extension)
  // If tool execution is requested, enforce confirmation or allowlist.
  if tool_use_requested:
      require explicit approval OR allowlist match

  // 4) Execute the agent's action
  result = AGENT_EXECUTE(user_request)

  // 5) Rollback Covenant (P-03)
  // If failure, ambiguity, or unsafe escalation occurs, revert immediately.
  if result == "FAILED" or uncertainty_increased:
      attempt ROLLBACK()
      return ROLLBACK_FAILURE_REPORT()
```
Wingman does not replace your agent.

Wingman prevents your agent from silently drifting into uncontrolled execution.

---

### Operational Reporting (Built-In)   

Wingman includes governance incident reporting templates via GitHub Issues.  

Use the Issues tab to file:  
	•	Governance Drift Report  
	•	Rollback Failure Report  
	•	Tool Escalation Report  
	•	Primitive Improvement Proposal  

These are designed to create auditability and upstream learning.  

---

### Installation Reality Check

If your agent stack has:  
	•	tools  
	•	memory  
	•	autonomy  
	•	long chains of execution  
	•	access to external systems  

then governance is not optional.  

Autonomous execution without rollback is not automation.  

It is uncontained risk.    

---

### Next Step (Recommended)  

After installation, run one controlled simulation:  
	1.	induce a mild hallucination risk  
	2.	request a tool escalation scenario  
	3.	test rollback under failure conditions  

If Wingman does not activate under pressure, your installation is incomplete.  

---  

### Canonical References  
	•	Quick Start: /docs/quickstart.md  
	•	Deployment Guide: /docs/DEPLOYMENT-GUIDE.md  
	•	Compliance Checklist: /docs/WINGMAN-COMPLIANCE.md  
	•	Primitive Index: /primitives/INDEX.md   

---

