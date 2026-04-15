# Asgard — AI Governance Orchestration Framework

![version](https://img.shields.io/badge/version-1.0.0-blue)
![license](https://img.shields.io/badge/license-MIT-green)
![python](https://img.shields.io/badge/python-3.10+-yellow)
![status](https://img.shields.io/badge/status-active-brightgreen)
![platform](https://img.shields.io/badge/platform-Windows%20%7C%20Linux-lightgrey)

> **"AI that builds. AI that verifies. Never the same. Structurally enforced."**

Asgard is an orchestration framework that makes it **structurally impossible** for the same AI to both create and verify its own output.

---

## The Problem

Every existing AI agent framework has the same flaw:

> The same AI that generates the answer also reviews it.
> That is not verification — that is self-confirmation.

**Hallucination confirmed by the hallucinator.**

---

## The Core Principle — Creator ≠ Verifier

```
Creator AI  ─────────────────────────────────────────────────────
  Designs. Writes. Builds. Proposes.          │
                                              │
                    ╔══════════════════════════════╗
                    ║  STRUCTURALLY ENFORCED WALL  ║
                    ║  Cannot cross. Code-blocked. ║
                    ╚══════════════════════════════╝
                                              │
Verifier AI ─────────────────────────────────────────────────────
             Reads. Checks. Judges. Approves or rejects.
             Never the same model. Never the same session.
```

Nothing is marked "done" without the Verifier's approval.
This is enforced by the system — not by policy, not by trust.

---

## How It Works — 8-Stage Pipeline

```
[1] REGISTER    User describes task interactively. AC recorded.
      ↓ GATE: Verifier checks requirement completeness
[2] DESIGN      Strategist agent writes plan + design review.
      ↓ GATE: Verifier checks design completeness
[3] IMPLEMENT   Builder agent writes code + handoff notes.
      ↓ GATE: Verifier checks implementation completeness
[4] TEST        Automated tests run. Results recorded.
[5] VERIFY      Verifier reads: what was promised vs delivered.
[6] VERIFY AC   Each acceptance criterion checked independently.
[7] INTEGRITY   9-point chain integrity verified end-to-end.
[8] COMPLETE    Evidence bundle assembled. Verifier signs off.
```

Every completion is a signed, verified record — not a claim.

---

## 5 Automated Quality Gates

Any failure blocks delivery and triggers regeneration.

| Gate | Check |
|------|-------|
| 1. Secret Scan | No hardcoded credentials in generated output |
| 2. Dependency | Only pre-approved external dependencies |
| 3. Security | Coding standards and security patterns |
| 4. Syntax | Structural correctness of all generated files |
| 5. Design Match | What was designed must match what was generated |

---

## The Agents — Norse Pantheon

Each agent has a single responsibility.

| Agent | Role |
|-------|------|
| **Odin** | Orchestrator — routes every task |
| **Mimir** | Strategist — designs and reviews architecture |
| **Völundr** | Builder — implements and refactors |
| **Heimdall** | Verifier — reads evidence, issues verdict. **Never builds.** |
| **Rune** | Editor — bug fixes, docs, small changes |
| **Huginn** | Scout — searches, feeds context |
| **Ratatoskr** | Messenger — carries handoff between stages |

**Heimdall is structurally separated from all creators.**
It can only judge — never create.

---

## Evidence-Driven Completion

Every task produces a structured evidence trail:

```
01_requirement.md   ← what was promised
02_plan.md          ← how it was planned
03_pre_review.md    ← independent critique of the plan
04_task_tracking.md ← what was actually built
05_handoff.md       ← builder's own assessment
06_verification.md  ← Verifier AI verdict (signed)
07_completion.md    ← auto-generated gate summary
```

"Done" is not a claim. It is a signed, verified record.

---

## Audit Council — 8 Roles

Rotating audit by 8 governance personas every session.

| Role | Persona | Responsibility |
|------|---------|----------------|
| CTO | Týr | Architecture, tech debt, scalability |
| CIO | Forseti | Security, governance, data integrity |
| QA | Víðarr | Test coverage, error handling |
| PO | Freyr | Backlog vs delivery gap, user value |
| UX | Iðunn | Consistency, accessibility, user flows |
| CSO | Bragi | AI trends, strategy |
| UX Lead | Sif | Design system, usability |
| Dev Lead | Baldr | Code quality, standards |

---

## Stack

- **Orchestrator:** Python agent runner
- **AI Providers:** Anthropic / OpenAI / Gemini / Ollama (swappable)
- **Verifier:** Ollama (local, independent model)
- **RAG:** LanceDB 3-tier (global / project / restricted)
- **DB:** PostgreSQL (asyncpg + Repository pattern)
- **Pipeline:** 8-stage with DB-recorded state at every step

---

## Status

Active development. Internal use.
Full open-source release planned after core pipeline stabilization.

---

## Learn More

- [Concept Guide](docs/asgard_infographic_brief.md) — concept-level visual guide

---

Created by [YG.SONG](https://github.com/saiasgard-neo) · Korea · 2026
