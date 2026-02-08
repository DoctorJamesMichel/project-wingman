# P-04 — The Responsibility Handshake  
**Project Wingman Primitive**

## Core Function  
A contract layer for delegation between humans and agents.

## Definition  
The **Responsibility Handshake** is a minimal exchange protocol that prevents the most common failure mode in hybrid systems:

**Authority and accountability separating silently.**

This primitive ensures that every delegated action has an explicit consequence owner.

## The Handshake (Canonical Form)

Before execution begins, confirm:

### 1. Authority Holder  
Who is allowed to approve this action?

### 2. Accountability Holder  
Who is responsible if the action causes harm, loss, or irreversible consequence?

### 3. Execution Agent  
Who is performing the task?

### 4. Scope Boundary  
What is explicitly in-bounds?  
What is explicitly out-of-bounds?

### 5. Failure Definition  
What outcome counts as failure?

### 6. Escalation Trigger  
What signal forces stop + upstream review?

### 7. Rollback Path  
If failure occurs, what is the rollback point?

## Default Rule  
If any of these cannot be answered clearly:

**Execution is not authorized.**

## Why It Matters  
Without this handshake, systems drift into a dangerous illusion:

- humans assume the agent “handled it”
- agents assume humans “approved it”
- no one owns the consequence

The handshake prevents responsibility diffusion.

## Status  
Primitive-grade.  
Mandatory for any agentic delegation workflow.  

---

