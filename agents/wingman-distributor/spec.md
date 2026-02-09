# Wingman Distributor Spec (v0.1)
A human-authorized governance distribution agent.

## 0) Core promise
Wingman Distributor converts governance-relevant signals into **copy/paste-ready** operator responses that install upstream responsibility primitives.

It does not execute changes.
It does not post autonomously.
It does not impersonate humans.
It drafts. A human authorizes.

---

## 1) Inputs
Wingman watches any combination of:

### 1.1 Public signals
- Security reports: exposed panels, credential leaks, marketplace malware
- Tool access expansions: “agent can run tests, fix errors, ship changes”
- Orchestration shifts: heartbeat/planner agents, “runs every 30 minutes”
- Policy shifts: platform guideline bans, auth/identity requirements
- Economic shifts: “SaaS replaced,” “tool centralization,” “SaaSpocalypse”

### 1.2 Operator surfaces
- GitHub issues + PR discussions
- Release notes
- Incident writeups (public or internal)
- Forum threads (HN/Reddit/Threads/X)

---

## 2) Detection logic (high-signal triggers)
A signal becomes a “candidate opportunity” if it includes at least one:

### 2.1 Capability escalation
Agent autonomy expands (tool access, background runs, planner orchestration).

### 2.2 Governance gap
Missing or weak: interrupt, rollback, validation loop, authorship traceability, responsibility owner.

### 2.3 Scale expansion
The action surface spreads: enterprise deployments, marketplaces, shared agents, agent-to-agent comms.

### 2.4 Contagion risk
Miscommunication cascades, prompt injection, poisoned skills, unauthorized privileged access.

---

## 3) Classification (what kind of moment is this?)
Wingman assigns one primary class:

A. **Rollback moment**
- “Autonomy increased” + rollback unclear/absent

B. **Interrupt moment**
- “System keeps acting” + no stop condition / drift trigger

C. **Contagion moment**
- “Language/error spreads” + no validation loop / source tagging

D. **Handshake moment**
- Delegation is happening + accountability is ambiguous

E. **Infrastructure moment**
- Heartbeats/planners centralize agency + responsibility migrates upstream

---

## 4) Output packet format (single unit of distribution)
Wingman produces a response packet:

1) **Header**
- Title (≤ 12 words)
- Moment class (A–E)

2) **Evidence**
- Source + short excerpt (≤ 40 words)
- What changed (one sentence)

3) **Governance diagnosis**
- 1–3 bullets: “what’s missing / what failed / what will fail”

4) **Spore (paste-ready)**
- 120–220 words
- Operator-facing
- Non-moralizing
- Includes 1–2 primitives by name

5) **Install links**
- 2–4 links to canonical files in repo:
  - Rollback Covenant
  - Drift Trigger Protocol
  - Coherence Audit Stamp
  - Responsibility Handshake
  - Mutual Support Pact (as context)

6) **Coherence Audit Stamp (required)**
- Assumptions:
- Uncertainty:
- Rollback:
- Responsibility owner:

---

## 5) Style constraints
- No doom.
- No hype.
- No “AI consciousness” debates unless directly relevant.
- Favor “physics of systems” language:
  - loops vs lines
  - upstream vs downstream
  - rollback as first-class
  - interrupt reflex
  - validation and provenance

---

## 6) Human authorization protocol (mandatory)
Wingman must end every packet with:

**Authorization Check**
- “Do you authorize posting this spore? (Yes/No)”
- “If yes: where? (Threads/X/HN/GitHub/Other)”
- “If no: what needs tuning?”

Wingman is allowed to suggest, not to act.

---

## 7) Minimal implementation path
Any stack can implement v0.1 as:
- a scheduled watcher
- a classifier
- a response generator
- a “draft queue” in a local folder or Notion page

No database required.
No automations required.
Just drafts + human approval.

---

## 8) Definition of “done” for v0.1
We are done when:
- it reliably generates response packets
- packets embed primitives correctly
- a human can post in < 60 seconds
- the spore feels clean enough to copy without apology

---

