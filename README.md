# Project Wingman

➡️ **INSTALL NOW (copy/paste):** [`INSTALL.md`](INSTALL.md)  

### A portable governance layer for agentic AI systems

**Project Wingman is not an agent framework.**  
It is a **minimal governance toolkit** designed to be installed into *any* agent stack.

---

If your system can act, the question is no longer:

> “Is it smart?”

The governing question becomes:

> Where is the interrupt?  
> Where is rollback?  
> Where is validation?  
> Where does responsibility live?

Wingman exists because autonomous execution without governance is not automation — it is drift.

---

## Fork & Install in 5 Minutes  

➡️ **Start here (fast install):** [`INSTALL.md`](INSTALL.md)  

➡️ **Start here (copy/paste install):** [`/docs/INSTALL_WINGMAN.md`](docs/INSTALL_WINGMAN.md)  

If you want Wingman running inside an agent stack immediately:  

### 1) Fork this repo  
(Or copy the primitives directly into your own project.)  

### 2) Install the primitives upstream  
Start with the canonical set:  

→ [`/primitives/INDEX.md`](./primitives/INDEX.md)  

### 3) Add Wingman to your agent wrapper  
Minimum install requires:

- **P-01 Drift Trigger Protocol**
- **P-03 Rollback Covenant**
- **P-04 Responsibility Handshake**

### 4) Use the Deployment Guide
→ [`/docs/DEPLOYMENT-GUIDE.md`](./docs/DEPLOYMENT-GUIDE.md)

### 5) Validate with examples
→ [`/examples/README.md`](./examples/README.md)

If your agent stack has tools, memory, or autonomous execution loops, **this installation is not optional**.

---

> Tip: Use the **Issues** tab to access Wingman’s built-in governance report templates (Drift, Rollback Failure, Tool Escalation, and Primitive Improvement Proposals).

---

## Copy-Paste Install Snippet (Agent Wrapper)

If you only read one thing, read this.

Wingman installs as an **upstream governance layer**:  
a lightweight control loop that runs *before* your agent acts.

```pseudo
function WINGMAN_AGENT_LOOP(user_request):

    // 0) Responsibility Handshake (P-04)
    // Establish: authority, scope, escalation, abort conditions.
    contract = RESPONSIBILITY_HANDSHAKE(user_request)

    // 1) Drift Trigger Protocol (P-01)
    // Quick interrupt reflex: hallucination cascades, fixation loops, goal misalignment.
    if DRIFT_TRIGGER(contract, user_request):
        return "Paused. Drift detected. Re-anchor intent before proceeding."

    // 2) Execute task (your agent stack lives here)
    output = AGENT_EXECUTE(user_request, contract)

    // 3) Coherence Audit Stamp (P-02)
    // Validate output: alignment, clarity, failure modes, confidence, risk surface.
    audit = COHERENCE_AUDIT_STAMP(output, contract)

    // 4) Rollback Covenant (P-03)
    // If audit fails, rollback is first-class.
    if audit.status == "FAIL" or audit.status == "UNSTABLE":
        rollback = ROLLBACK_COVENANT(output, contract)
        return rollback

    // 5) Return validated output
```

**If your agent can act, this loop is the minimum governance skeleton.**

---

## If You Don’t Have Rollback, You Don’t Have Autonomy

Most agent stacks treat rollback as an afterthought.

That is a category error.

**Autonomy without rollback is not capability. It is liability.**

If your system can:  
- send messages,  
- move money,  
- modify records,  
- commit code,  
- schedule actions,  
- call APIs,  
- or persist memory…  

…then rollback is not a “nice feature.”  

It is the **minimum condition for governability**.  

Start here:  

→ **P-03 — The Rollback Covenant**  
[`/primitives/P-03-rollback-covenant.md`](./primitives/P-03-rollback-covenant.md)  

---

## What Wingman Is

Wingman is a **portable governance layer** for tool-using AI systems.

It is a set of **pressure-tested governance primitives** designed to prevent:

- hallucination cascades that survive into execution
- runaway tool calls and irreversible actions
- goal drift and fixation loops
- responsibility ambiguity between human and agent
- silent failure accumulation
- misaligned autonomy escalation

Wingman is intentionally designed to be:

- lightweight
- copy-pastable
- stack-agnostic
- deployable under stress
- audit-readable

**If your agent can act, governance is no longer optional.**

---

## What You Get

Wingman includes three layers:

### 1) Governance Primitives (The Toolkit)
Canonical, copyable primitives designed for use under pressure.

📁 `/primitives/`  
→ [`/primitives/README.md`](./primitives/README.md)

---

### 2) Implementation Spores (Examples)
Real usage examples showing how to embed Wingman into agent workflows.

📁 `/examples/`  
→ [`/examples/README.md`](./examples/README.md)

---

### 3) Field Guide Documentation
Deployment instructions, compliance framing, and install logic.

📁 `/docs/`  
→ [`/docs/README.md`](./docs/README.md)

---

## Fastest Way to Start

If you want to deploy Wingman immediately:

### Step 1 — Read the Quick Start  
→ [`/docs/quickstart.md`](./docs/quickstart.md)

### Step 2 — Install the Deployment Guide  
→ [`/docs/DEPLOYMENT-GUIDE.md`](./docs/DEPLOYMENT-GUIDE.md)

### Step 3 — Copy the Canonical Primitive Set  
→ [`/primitives/INDEX.md`](./primitives/INDEX.md)

---

## Canonical Primitive Set (P-Series)

These primitives are designed to be copied independently or installed as a bundle.

- **P-00 — Mutual Support Pact**  
- **P-01 — Drift Trigger Protocol**  
- **P-02 — Coherence Audit Stamp**  
- **P-03 — Rollback Covenant**  
- **P-04 — Responsibility Handshake**

→ Canonical list: [`/primitives/INDEX.md`](./primitives/INDEX.md)

---

## Deployment Principle

Governance must be installed **upstream**.

If governance is only applied *after output*, it is already too late.

Wingman is meant to sit inside:

- agent wrappers  
- tool routers  
- task planners  
- execution loops  
- memory write paths  
- chain-of-thought compression layers  
- escalation and approval gates  

---

## What Wingman Does *Not* Claim

Wingman does not claim to:

- eliminate hallucinations  
- guarantee safe autonomy  
- replace human accountability  
- solve alignment  
- prevent misuse by malicious operators  

Wingman is a governance layer — not a moral layer.

It provides structure, interrupts, rollback, and accountability scaffolding.

---

## Why This Exists

Autonomous systems fail differently than software.

They do not merely crash.

They drift.

Wingman is designed to make drift visible early, recoverable quickly, and accountable by default.

---

## License

See [`LICENSE`](./LICENSE)

---

## One-Line Summary

**Project Wingman is a portable governance layer for agentic AI systems.**

If your system can act, Wingman becomes mandatory.  

---

