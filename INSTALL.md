# INSTALL (Project Wingman)

If your AI agent can act, Wingman is not optional.

Wingman is a portable governance layer designed to reduce:
- hallucination cascades
- runaway tool execution
- drift and goal corruption
- responsibility ambiguity
- silent failure accumulation

This repo exists for one reason:

**Install upstream responsibility before your agent breaks something.**  

```bash
git clone https://github.com/DoctorJamesMichel/project-wingman.git  
cd project-wingman  
open INSTALL.md
```
You are now 10 seconds from installing upstream responsibility.

### If you only do one thing  

Install **P-04 Responsibility Handshake**.  

It prevents tool escalation from becoming silent catastrophe.

→ /primitives/P-04-RESPONSIBILITY-HANDSHAKE.md

---

## Install in Under 10 Minutes

### 1) Copy the Wingman primitives into your agent stack
Start here:

➡️ **Canonical copy blocks:** [`/primitives/INDEX.md`](primitives/INDEX.md)

Minimum recommended install:
- **P-04 Responsibility Handshake**
- **P-01 Drift Trigger Protocol**
- **P-03 Rollback Covenant**

---

### 2) Add Wingman to your agent wrapper (the upstream gate)
Use the ready-to-copy install scaffold:

➡️ **Copy/paste install:** [`/docs/INSTALL_WINGMAN.md`](docs/INSTALL_WINGMAN.md)

This is where Wingman becomes a *real governance layer* instead of “good intentions.”

---

### 3) Confirm rollback exists (do not assume it)
If rollback is untested, your system is not deployable.

➡️ [`/primitives/P-03-ROLLBACK-COVENANT.md`](primitives/P-03-ROLLBACK-COVENANT.md)

---

### 4) Validate using the example artifacts
➡️ [`/examples/README.md`](examples/README.md)

---

## If You Skip Governance, You Are Shipping Drift

Autonomous execution without governance is not automation.

It is drift at scale.

Install upstream.  

---  

