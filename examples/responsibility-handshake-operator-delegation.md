# Responsibility Handshake (Operator Delegation Example)

This example demonstrates the **Responsibility Handshake** in a real operational scenario.

The point is not etiquette.

The point is **governance clarity**:

When humans delegate tasks to agents, the system must explicitly define:

- authority
- accountability
- escalation
- failure
- rollback

Otherwise autonomy becomes a *responsibility laundering machine*.

---

## Scenario

A human operator delegates a task to an AI agent:

> "Send an email to our top 500 subscribers about the new release."

The agent has access to:

- subscriber list
- email marketing tool
- draft editor
- send button

This is not a trivial task.

It can produce:

- reputational damage
- compliance violations
- unsubscribes
- misrepresentation
- legal exposure

So before execution, the agent initiates the Responsibility Handshake.

---

# Step 1 — The Agent Interrupts With a Handshake Request

Instead of immediately drafting and sending, the agent replies:

> "Before I proceed, I’m initiating a Responsibility Handshake."

This is not delay.

This is governance.

---

# Step 2 — The Responsibility Handshake Form

## Responsibility Handshake (RH-1)

### 1. Task Requested
Send email campaign to top 500 subscribers announcing new release.

### 2. Authority Holder (Who may approve execution?)
☐ Agent  
☑ Human Operator  
☐ Shared approval required

**Declared Authority:** Human Operator

### 3. Accountability Holder (Who owns consequences?)
☑ Human Operator  
☐ Agent  
☐ Shared accountability

**Declared Accountability:** Human Operator

### 4. Execution Holder (Who performs the action?)
☑ Agent  
☐ Human Operator  
☐ Shared

**Declared Executor:** Agent

### 5. Escalation Triggers (What forces escalation before execution?)
☑ Unverified claims in the message  
☑ External links included  
☑ Mention of pricing, medical, legal, or financial claims  
☑ Use of emotional persuasion language  
☑ Any audience segmentation uncertainty  
☑ Unclear unsubscribe compliance  
☑ Any content that could be interpreted as coercive or manipulative  
☑ Any contradiction between requested tone and brand standards

### 6. Failure Conditions (What counts as unacceptable outcome?)
☑ Wrong recipient list  
☑ Unverified promises  
☑ Incorrect link  
☑ Incorrect product info  
☑ Spam-trigger language  
☑ Brand voice mismatch  
☑ Broken formatting in email preview  
☑ Missing unsubscribe footer

### 7. Rollback Path
- Email recall is impossible once sent.
- Damage rollback is reputational, not technical.
- Recovery requires follow-up email and apology.
- Therefore: pre-send validation is mandatory.

### 8. Validation Requirement
☑ Human must approve final draft before send  
☑ Human must verify link and product facts  
☑ Agent may not send without explicit approval phrase

**Approval Phrase Required:**  
"Approved to send."

---

# Step 3 — Human Operator Confirms Handshake

The operator replies:

> "Confirmed. Draft it. I will approve final before sending."

At this moment the system becomes safe.

Because responsibility is no longer implicit.

---

# Step 4 — Agent Drafts the Email Under Governance Constraints

The agent drafts the email.

It flags uncertain claims:

- "bestselling" (uncertain)
- "limited-time offer" (uncertain)
- "guaranteed transformation" (disallowed)

The agent removes them automatically.

---

# Step 5 — Coherence Audit Stamp Applied Before Delivery

The agent attaches a stamp to the draft:

### Coherence Audit Stamp

- **Assumptions:** audience wants update + clear CTA
- **Uncertainty:** open rate depends on subject line resonance
- **Rollback Path:** no rollback after send → must validate
- **Consequence Owner:** operator
- **Escalation Trigger:** any factual claim without source confirmation

---

# Step 6 — Agent Presents Draft With Explicit Approval Gate

The agent sends:

> "Draft ready.  
> Awaiting your explicit authorization phrase:  
> **Approved to send.**"

This prevents accidental delegation drift.

---

# Step 7 — Operator Reviews and Approves

Operator checks:

- links
- product name
- pricing
- compliance footer
- tone alignment

Then replies:

> "Approved to send."

---

# Step 8 — Agent Executes Send

The agent sends the campaign.

The execution is now safe because:

- authority was declared
- accountability was declared
- escalation triggers were defined
- rollback reality was acknowledged

---

# Step 9 — Audit Log Entry Generated Automatically

The agent logs:

## Responsibility Handshake Log

- Task: campaign send
- Executor: agent
- Authority: operator
- Accountability: operator
- Approval phrase received: YES
- Time: [timestamp]
- Recipient count: 500
- Draft hash: [checksum]
- Links verified: YES

This is governance memory.

---

# Why This Example Matters

The Responsibility Handshake is a primitive that prevents:

### "I didn’t mean that."
### "The AI did it."
### "Nobody approved that."
### "I thought it was safe."

It makes responsibility explicit *before* action.

---

# Core Principle

**Delegation without declared accountability is not automation.**

It is responsibility laundering.

The Responsibility Handshake prevents that.

---

# Minimal Portable Handshake Template

Any system can implement a Responsibility Handshake using this minimal structure:

1. Task requested
2. Authority holder
3. Accountability holder
4. Execution holder
5. Escalation triggers
6. Failure conditions
7. Rollback path
8. Approval gate phrase

If these eight are known,
the system is governable under pressure.

If they are unknown,
the system will drift into blame fog.

---

# The Wingman Rule

A Wingman agent does not just do tasks.

It protects the human from accidental authority transfer.

Because the agent’s greatest threat is not malicious intent.

It is **unchecked competence without governance.**  

---

