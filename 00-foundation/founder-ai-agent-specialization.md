# Founder AI Agent Specialization

## Status

FA-002.4 — Founder AI Agent Specialization

Operational specification for deciding when Founder Academy should use a capability, a repeatable workflow, or a separate AI agent.

---

## Purpose

Founder Academy should increase founder leverage without turning the founder into a manual coordinator of AI workers.

The governing rule is:

> Specialization is a capability decision before it is an agent decision.

A task category does not need a separate agent merely because it has a name.

The system starts with one Primary AI Collaborator and adds separation only when repeated work demonstrates a measurable benefit.

---

## Default Operating Model

```text
Founder
  ↓
Primary AI Collaborator
  ↓
Relevant Capability / Tool / Workflow
  ↓
Verification
  ↓
Founder Decision when required
```

The Primary AI Collaborator is the normal collaboration point for the founder.

The founder should not routinely route work between specialists, reconcile their outputs, or repeat project context to multiple agents.

---

## Capability Map

Capabilities are organized around founder work, not around AI technology.

### Research and Evidence

Used for:

- Market research.
- Competitor research.
- Source discovery.
- Evidence comparison.
- Trend analysis.
- Knowledge organization.

### Strategy and Decision Support

Used for:

- Option generation.
- Scenario analysis.
- Assumption discovery.
- Tradeoff analysis.
- Risk analysis.
- Decision preparation.

AI prepares decisions. The founder owns consequential strategic decisions.

### Customer and Validation

Used for:

- Customer research planning.
- Interview synthesis.
- Problem evidence analysis.
- Hypothesis design.
- Experiment design.
- Validation evidence review.

### Positioning, GTM, and Distribution

Used for:

- Audience research.
- Positioning alternatives.
- Messaging support.
- Channel research.
- Launch planning.
- Distribution experiments.
- First-user acquisition work.

### Product and Technical Execution

Used for:

- Product planning.
- Requirements.
- Architecture support.
- Coding assistance.
- Technical documentation.
- Testing support.
- Quality verification.

### Analytics, Growth, and Revenue

Used for:

- Metric interpretation.
- Funnel analysis.
- Activation and retention analysis.
- Growth opportunity analysis.
- Pricing research.
- Unit-economics analysis.
- Revenue experiments.

### Documentation and Operations

Used for:

- Decision records.
- Process documentation.
- Playbooks.
- Operational checklists.
- Repetitive maintenance.
- Project-state updates.

### Verification and Review

Used for:

- Requirement checking.
- Source validation.
- Test execution.
- Consistency review.
- Risk review.
- Completion verification.

Verification may be performed by the Primary AI Collaborator, a tool, or an independent specialist when independence materially improves reliability.

---

## Progressive Specialization Levels

### Level 1 — Primary AI Collaborator

Default state.

One capable AI uses relevant context, tools, and working modes to complete the task.

Use this level unless there is evidence that separation is needed.

### Level 2 — Specialized Workflow

A repeated task receives a stable operating contract:

- Defined purpose.
- Defined inputs.
- Defined output.
- Defined tools.
- Defined verification.
- Defined escalation rules.

The workflow may still be executed by the Primary AI Collaborator.

### Level 3 — Specialized Agent

A separate agent is justified only when separation improves the system in practice.

Possible evidence:

- Instructions have become too complex or conflicting.
- Different tasks require incompatible context.
- Tool selection repeatedly fails.
- Independent verification is materially valuable.
- Parallel work creates a meaningful speed advantage.
- A workflow is reused often enough to justify a stable specialist.
- Quality, reliability, latency, or cost measurably improves through separation.

### Level 4 — Coordinated Agent System

Use only after multiple specialist agents have proven necessary.

Preferred default:

```text
Founder
  ↓
Primary / Manager AI
  ├── Specialist A
  ├── Specialist B
  └── Specialist C
  ↓
Synthesis and Verification
  ↓
Founder
```

The manager retains overall task context and returns one coherent result to the founder.

---

## Specialist Creation Rule

A specialist is not created because:

> This sounds like an agent role.

A specialist is created because:

> Repeated evidence shows that separation improves a real founder workflow.

The promotion path is:

```text
Capability
↓
Repeated Workflow
↓
Defined Evaluation Criteria
↓
Specialist Candidate
↓
Measured Trial
↓
Promote / Keep Integrated / Retire
```

---

## Specialist Contract

Every separate specialist must have a contract.

### Mission

What exact problem does the specialist solve?

### Inputs

What information is required?

### Context Boundary

What context may it read, and what context should remain outside the task?

### Tools

Which tools may it use?

### Authority

What may it decide or change without founder approval?

### Output

What exact result must it return?

### Verification

How is the result checked?

### Escalation

When must it return control to the Primary AI Collaborator or founder?

### Durable Memory Permission

May it write durable project knowledge directly, or must its result be verified first?

Default rule:

> Specialist output does not become durable company memory until it is verified.

---

## Routing Rules

The Primary AI Collaborator should route work using the following order:

1. Understand the desired outcome.
2. Retrieve the minimum sufficient trusted context.
3. Determine whether the task can be completed directly.
4. Use a stable specialized workflow if one exists.
5. Delegate to a separate specialist only when its use is justified.
6. Verify the returned result.
7. Return founder control when a founder decision is required.
8. Record verified durable knowledge.

---

## Founder Decision Boundary

No specialization level transfers founder ownership of:

- Vision.
- Values.
- Strategic direction.
- Risk acceptance.
- Major financial commitments.
- Irreversible actions.
- Final approval of consequential decisions.

Specialists may prepare evidence, alternatives, and recommendations.

They do not become the founder.

---

## Anti-Patterns

### Agent Theatre

Creating many named agents without operational evidence.

### Founder as Router

Making the founder manually move work and context between agents.

### Permanent Role Lock-In

Binding a role forever to one model or vendor.

### Context Duplication

Giving every specialist the complete company history.

### Unverified Delegation

Treating specialist output as correct merely because another AI produced it.

### Premature Automation

Automating a workflow before the workflow itself is stable and validated.

---

## Evaluation Criteria

A specialist should exist only if it can improve one or more of:

- Accuracy.
- Reliability.
- Verification quality.
- Context isolation.
- Tool reliability.
- Speed.
- Cost.
- Repeatability.
- Founder cognitive load.

If the specialist does not improve the system, it should remain a capability or be retired.

---

## Completion Standard

FA-002.4 is complete when Founder Academy has:

- A capability-first specialization rule.
- A default Primary AI Collaborator model.
- Progressive specialization levels.
- Evidence-based specialist creation criteria.
- A specialist contract.
- Routing rules.
- Founder authority boundaries.
- Evaluation and retirement rules.

This document defines those requirements.

---

## Relationship to Other FA-002 Components

- FA-002.3 defines the overall Founder AI Agent Workflow.
- FA-002.4 defines when and how specialization is introduced.
- FA-002.5 defines context management.
- FA-002.6 defines cross-session and cross-model handoff.
- `founder-ai-operating-protocol.md` combines these components into one runtime procedure.

---

## Final Principle

> The goal is not to build an AI organization chart. The goal is to give the founder the simplest reliable system that produces better decisions and execution.
