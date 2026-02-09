# Wingman Distributor (v0.1)
Human-authorized distribution agent for upstream responsibility primitives.

## What this is
Wingman Distributor watches for governance gaps in real-world agentic systems (tool access, marketplace malware, prompt injection, “heartbeat” orchestration, unauthorized deployments) and produces **ready-to-post** responses that embed Wingman primitives.

**Hard rule:** it never publishes on its own.  
It drafts. A human authorizes.

## Why it exists
As agent autonomy increases, responsibility must move upstream.
But most teams only feel this *after* a breach, a cascade, or a PR fire.

Wingman Distributor makes governance “show up early” by:
- detecting high-signal moments
- generating short, credible operator-facing inserts
- linking to canonical primitives and examples

## What it outputs
Each “opportunity” produces a single packet:
- **Title**: one-line “what this is”
- **Trigger**: what was detected (source + quote excerpt)
- **Diagnosis**: the governance gap (1–3 bullets)
- **Spore**: a short response you can paste into a thread
- **Links**: relevant primitives + example files
- **Audit Stamp**: assumptions / uncertainty / rollback / responsibility owner

## Where it plugs in
- Social: Threads, X, Reddit, Hacker News, Discord/Slack communities
- GitHub: issues, security advisories, marketplace PRs
- Internal: incident postmortems, change approvals, release notes

## Operating constraints (non-negotiable)
1. **No autonomous posting.** Draft only.
2. **No persuasion theater.** Clarity over heat.
3. **Cite sources when possible.** Don’t inflate claims.
4. **Default to minimal intrusion.** One high-quality spore beats 20 noisy posts.
5. **Always embed rollback + validation posture.** If absent, say so.

## Success metric (simple)
If an operator copies one spore, installs one primitive, and prevents one cascade,
the agent is working.

## Start here
- Spec: `spec.md`
- Response templates: `templates/`
- Example outputs: `runs/` (optional)
- Canonical primitives: `/primitives/`

> Wingman’s job is not to “win arguments.”
> It is to make upstream responsibility unavoidable.

---

