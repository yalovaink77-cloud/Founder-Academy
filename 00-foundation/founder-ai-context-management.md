# Founder AI Context Management

## Status

FA-002.5 — Context Management System

Operational specification for preserving, retrieving, and updating trusted Founder Academy and project context.

---

## Purpose

AI performance depends on context quality.

Founder Academy therefore treats context as a company asset.

The system must preserve important knowledge across:

- Conversations.
- Models.
- Tools.
- Devices.
- Time.
- Project phases.

The governing rule is:

> Chat is a workspace. Verified documentation is durable memory.

---

## Context Classes

### 1. Foundational Context

Slow-changing information that defines the system or project.

Examples:

- Vision.
- Principles.
- Founder operating rules.
- Product-independent Academy rules.
- Project purpose.
- Safety and governance principles.

### 2. Decision Context

Approved decisions that should not be silently reopened.

Examples:

- Architecture decisions.
- Business-model decisions.
- Scope decisions.
- Positioning decisions.
- Pricing decisions.
- Process decisions.

Each durable decision should make clear:

- What was decided.
- Why.
- Status.
- What it supersedes, if anything.

### 3. Current-State Context

The minimum information required to continue work correctly.

Examples:

- Current phase.
- Completed work.
- Current task.
- Known blockers.
- Verification state.
- Next logical action.

### 4. Evidence Context

Source material used to support decisions.

Examples:

- Research reports.
- Customer interviews.
- Analytics.
- Market evidence.
- Competitor evidence.
- Test results.

Evidence is not automatically a decision.

### 5. Working Context

Temporary task-specific material.

Examples:

- Current conversation.
- Scratch analysis.
- Drafts.
- Temporary files.
- Unverified AI output.

Working context should not automatically become durable memory.

### 6. Learned Context

Verified lessons produced by execution.

Examples:

- What worked.
- What failed.
- Why a hypothesis changed.
- Reusable patterns.
- Playbook improvements.

---

## Source-of-Truth Hierarchy

When sources conflict, use the following default order:

1. Current explicit founder decision.
2. Current repository source-of-truth documents.
3. Approved decision records and operating manuals.
4. Current verified project-state documents.
5. Verified research and evidence.
6. Previous handoff documents.
7. Conversation history.
8. Unverified drafts or AI-generated notes.

A lower-ranked source must not silently override a higher-ranked source.

If a real conflict remains, AI should surface it rather than invent reconciliation.

---

## Minimum Sufficient Context Rule

More context is not automatically better.

For every task, AI should retrieve:

> The smallest set of trusted information required to perform the task correctly.

Task context should normally include:

- The current goal.
- Relevant current state.
- Relevant approved decisions.
- Relevant constraints.
- Required evidence.
- Verification criteria.

Do not automatically load:

- Entire conversation history.
- Unrelated projects.
- All research files.
- Old superseded decisions.
- Large documents with no relevance to the task.

---

## Context Retrieval Protocol

Before significant work:

### Step 1 — Identify the Task

Determine:

- Project.
- Phase.
- Desired outcome.
- Decision or execution type.

### Step 2 — Retrieve Foundational Rules

Read only the foundational documents relevant to the task.

### Step 3 — Retrieve Current State

Determine what is already complete, what is active, and what is next.

### Step 4 — Retrieve Relevant Decisions

Find approved decisions that constrain the task.

### Step 5 — Retrieve Evidence

Load supporting research or data only when required.

### Step 6 — Resolve Conflicts

Apply the source-of-truth hierarchy.

### Step 7 — Execute

Proceed with the task using the resolved context.

---

## Context Update Protocol

Durable memory should be updated only when work creates a durable change.

Examples:

- A decision is approved.
- A phase is completed.
- A new operating rule is adopted.
- Research produces a validated conclusion.
- A reusable lesson is confirmed.
- Project status materially changes.

Do not create durable records for every conversation detail.

The update sequence is:

```text
Work
↓
Verification
↓
Founder approval when required
↓
Durable record
↓
Git / source-of-truth update
```

---

## Write Permission Rule

Not every AI output may update durable memory.

### May Update After Verification

- Mechanical status updates.
- Test results.
- Completed task records.
- Non-strategic documentation corrections.

### Founder Approval Required Before Durable Update

- Vision changes.
- Strategic direction.
- Pricing strategy.
- Business-model changes.
- Major scope changes.
- Values or safety principles.
- Consequential product decisions.

---

## Context Compression

Long-running projects accumulate information.

The system should periodically compress state into concise durable summaries rather than forcing future models to reread every historical artifact.

A useful state summary includes:

- Purpose.
- Current phase.
- Completed milestones.
- Active decisions.
- Key constraints.
- Current task.
- Open questions.
- Next action.
- References to deeper source files.

Compression must preserve decisions and remove noise, not rewrite history.

---

## Superseded Information

Old information should not be silently deleted when history matters.

When a durable decision changes:

- Mark the previous decision superseded or archived.
- Record the new decision.
- State why it changed when useful.
- Point to the replacement.

This prevents old AI context from reactivating obsolete decisions.

---

## Cross-Project Isolation

Founder Academy supports many products.

Project-specific context must remain isolated unless comparison is intentionally required.

Default:

- Lumora context stays Lumora context.
- PiercingConnect context stays PiercingConnect context.
- Kuryele context stays Kuryele context.

Founder Academy may extract reusable principles from projects only after those lessons are generalized and validated.

This protects the Academy from accidental product-specific bias.

---

## Research Context Rule

Research files are evidence, not automatic policy.

A research report may contain:

- Facts.
- Hypotheses.
- Recommendations.
- Uncertainty.

Only approved conclusions should become operating rules or decisions.

---

## Context Quality Checks

Before using durable context, AI should ask:

- Is this the current version?
- Has it been superseded?
- Is it verified?
- Is it relevant to this task?
- Is it project-specific or reusable?
- Is it a decision, evidence, or merely a draft?

---

## Failure Modes

### Chat Dependency

Depending on one conversation to preserve project memory.

### Context Dumping

Loading everything into every task.

### Stale Decision Revival

Using old decisions after they were replaced.

### Draft as Truth

Treating unverified AI output as approved context.

### Cross-Project Leakage

Applying one product's assumptions to another without validation.

### Memory Without Verification

Recording incorrect work because it was generated confidently.

---

## Completion Standard

FA-002.5 is complete when Founder Academy has:

- Defined context classes.
- A source-of-truth hierarchy.
- A minimum sufficient context rule.
- A retrieval protocol.
- An update protocol.
- Write-permission boundaries.
- Context compression rules.
- Supersession rules.
- Cross-project isolation rules.

This document defines those requirements.

---

## Relationship to Other FA-002 Components

- FA-002.3 defines how founder and AI work together.
- FA-002.4 defines specialization.
- FA-002.5 defines durable context.
- FA-002.6 defines handoff.
- `founder-ai-operating-protocol.md` combines them into daily execution.

---

## Final Principle

> The purpose of context management is not to make AI remember everything. It is to make the right information reliably available when it matters.
