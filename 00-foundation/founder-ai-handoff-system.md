# Founder AI Handoff System

## Status

FA-002.6 — Founder AI Handoff System

Operational specification for transferring project state safely across conversations, models, tools, and future collaborators.

---

## Purpose

Founder Academy must not depend on one AI conversation remembering the project correctly.

A handoff should allow another capable AI to continue work without forcing the founder to reconstruct history manually.

The governing rule is:

> A handoff transfers current operating state, not the entire conversation history.

The repository remains the durable source of truth.

---

## Goals

A valid handoff should let a receiving AI determine:

- What the project is.
- Why it exists.
- Which phase is active.
- What has been completed.
- Which decisions are active.
- Which constraints matter.
- What is currently being worked on.
- What remains unresolved.
- What the next logical action is.
- Which repository documents are authoritative.

The founder should not need to repeat known information unless a genuine decision is required.

---

## What a Handoff Is Not

A handoff is not:

- A dump of the entire chat history.
- A replacement for source-of-truth documents.
- A place to preserve every brainstorming idea.
- Permission to revive superseded decisions.
- A substitute for verifying the current repository state.

A handoff is a navigation and continuity layer.

---

## Canonical Handoff Structure

Every durable handoff should contain the following sections.

### 1. Project Identity

- Project name.
- Purpose.
- Product-independent or project-specific scope.
- Relevant repository.

### 2. Current Phase

- Current lifecycle phase.
- Current subphase or sprint when applicable.
- Why this phase is active.

### 3. Current Goal

- One active outcome.
- What completion means.

### 4. Completed Work

- Important completed milestones only.
- Verification state where relevant.
- References to source files or commits.

### 5. Active Decisions

- Approved decisions that constrain future work.
- Status: ACTIVE.
- Reason when useful.
- Reference to the authoritative document.

### 6. Superseded or Rejected Directions

- Old approaches that must not be silently reintroduced.
- Replacement decision when one exists.

### 7. Constraints

Examples:

- Founder authority boundaries.
- Safety rules.
- Product scope.
- Working protocol.
- Technical constraints.
- Budget or resource constraints when explicitly confirmed.

### 8. Current State

- What exists now.
- What is verified.
- What is unverified.
- Current blocker, if any.

### 9. Open Questions

Only unresolved questions that can materially affect the next work.

Do not invent answers.

### 10. Exact Next Action

One logical next task.

### 11. Source-of-Truth References

List the minimum authoritative files needed to continue.

### 12. Provenance

When practical, include:

- Repository branch.
- Relevant commit or revision.
- Handoff generation date.

This helps detect stale handoffs.

---

## Handoff Priority Rule

A receiving AI must apply the Context Management source-of-truth hierarchy.

If the handoff conflicts with a newer repository decision:

> The current repository source of truth wins.

The handoff should be treated as stale rather than forcing the repository to match it.

---

## Receiving AI Startup Protocol

When continuing from a handoff:

### Step 1 — Identify the Repository

Confirm the project and source-of-truth location.

### Step 2 — Read Core Context

Read the minimum referenced files necessary to understand purpose, active decisions, and current state.

### Step 3 — Verify Current State

Check whether the repository has changed since the handoff.

### Step 4 — Resolve Conflicts

Use the source-of-truth hierarchy.

Do not silently merge contradictory decisions.

### Step 5 — Preserve Active Decisions

Do not reopen approved decisions without new evidence or an explicit founder request.

### Step 6 — Continue the Exact Next Action

Proceed with one logical task.

### Step 7 — Update Durable State

After verification, record any durable changes created by the work.

---

## Handoff Creation Triggers

Create or refresh a handoff when continuity risk becomes meaningful.

Useful triggers include:

- Moving to a new conversation.
- Changing the primary AI/model.
- Completing a major phase.
- Pausing a project for a long period.
- Transferring work to another collaborator.
- A large set of decisions has accumulated.
- The current conversation has become too large or unreliable.

Do not create a new handoff after every minor message.

---

## Compact vs Recovery Handoff

### Compact Operational Handoff

Default.

Use for normal conversation/model transitions.

Contains:

- Purpose.
- Current phase.
- Current goal.
- Completed work.
- Active decisions.
- Constraints.
- Current state.
- Next action.
- Source-of-truth references.

### Recovery Handoff

Use only when continuity has seriously degraded or a project must be reconstructed.

May additionally contain:

- Timeline of major decisions.
- Important failed approaches.
- Historical architecture changes.
- Broader evidence references.
- Recovery uncertainties.

Recovery handoffs are larger because the risk justifies the added context.

---

## Handoff Quality Standard

A handoff is good when another capable AI can continue without:

- Asking the founder to repeat known project history.
- Reopening settled decisions.
- Guessing current state.
- Reading every historical conversation.
- Treating old drafts as truth.
- Repeating already completed work.

---

## Staleness Detection

A handoff should be considered potentially stale when:

- The repository branch has advanced materially.
- Referenced files have changed.
- A newer decision record exists.
- The active phase has changed.
- The founder has made a newer explicit decision.

The receiving AI must verify rather than assume freshness.

---

## Security and Privacy

A handoff must not contain secrets unless a secure system explicitly requires them.

Do not store:

- Passwords.
- API keys.
- Access tokens.
- Private credentials.
- Authentication secrets.

Refer to secure configuration locations instead of copying secrets into handoff documents.

---

## Handoff Maintenance Rule

Handoff documents should be concise enough to remain useful.

When they become too large:

- Move durable decisions into their proper source-of-truth documents.
- Keep the handoff as an index and current-state snapshot.
- Link to deeper research instead of reproducing it.
- Remove obsolete operational detail while preserving important history in appropriate archives.

---

## Founder Cognitive Load Rule

The founder should not manually construct a handoff from scratch when AI has access to the project state.

Preferred behavior:

1. AI reads the repository.
2. AI drafts the handoff.
3. AI identifies only decisions that genuinely require founder confirmation.
4. AI verifies the result.
5. AI records it in the repository when appropriate.

The founder should remain decision-maker, not documentation middleware.

---

## Completion Standard

FA-002.6 is complete when Founder Academy has:

- A canonical handoff structure.
- A receiving-AI startup protocol.
- Source-of-truth conflict rules.
- Creation triggers.
- Compact and recovery modes.
- Staleness detection.
- Security rules.
- A low-cognitive-load maintenance rule.

This document defines those requirements.

---

## Relationship to Other FA-002 Components

- FA-002.3 defines Founder + AI workflow.
- FA-002.4 defines AI specialization.
- FA-002.5 defines context management.
- FA-002.6 defines continuity and transfer.
- `founder-ai-operating-protocol.md` combines all four into one practical runtime.

---

## Final Principle

> The founder should be able to change chats, models, or tools without losing the company’s operating memory.
