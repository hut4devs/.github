# Hut4Devs Issue Governance

## Issue hierarchy
Product vision -> Milestone -> Outcome -> Capability -> Epic -> Issue -> Acceptance criteria -> Validation evidence.

Use GitHub milestones for meaningful outcomes or release gates, not arbitrary issue counts. Use labels to identify work type, priority, risk, and status.

## Required issue fields
Every implementation issue must state:
1. Title and problem statement.
2. User or system outcome.
3. Parent milestone or epic.
4. Scope and explicit non-goals.
5. Acceptance criteria written as observable behavior.
6. Dependencies and affected repositories.
7. Security, privacy, and data-boundary considerations.
8. Testing and validation evidence required.
9. Relevant documentation links.
10. Definition of done.

Research issues must also state the question, method, evidence sought, and decision the research will inform.

## Issue template

### Outcome
What changes for the user or system?

### Context
Why does this matter now? Link to the charter, roadmap, product log, or decision record.

### Scope
What is included?

### Non-goals
What must not be included?

### Acceptance criteria
- [ ] Observable behavior or outcome.
- [ ] Expected failure behavior.
- [ ] Authorization and privacy behavior.
- [ ] Tests and documentation completed.

### Dependencies
List issue numbers and interface or repository dependencies.

### Validation evidence
Specify tests, screenshots, experiment results, security review, or demonstration needed.

### Definition of done
- Acceptance criteria met.
- Tests and relevant failure paths validated.
- Security and privacy implications reviewed.
- Documentation and contracts updated.
- Changes reviewed and merged under repository policy.
- Evidence linked.

## Issue quality rules
- One issue should represent one reviewable outcome.
- Split work when acceptance criteria cannot be reviewed or tested together.
- Do not create implementation issues for unvalidated assumptions unless they are explicitly research or discovery tasks.
- Link directly to relevant Markdown documents in the canonical repository.
- Use dependency links instead of duplicating the same work in multiple repositories.
- Close issues only when their acceptance criteria are satisfied or they are explicitly cancelled with a reason.
- An issue count is not a measure of product progress.
- Avoid vague issues such as "improve security" or "add AI." Specify the threat, user need, outcome, and evidence.
- Use the organization's agreed  commit convention where applicable.

## Priority policy
- P0: Active critical incident or release-blocking critical risk.
- P1: Required for the current milestone or a material security/privacy requirement.
- P2: Important, but not blocking the current milestone.
- P3: Optional improvement or later opportunity.

Priority must include a rationale. A label is not a substitute for milestone sequencing.

## Definition of ready
An issue is ready when the problem, owner, dependencies, scope, acceptance criteria, and validation method are clear.

## Definition of done
An issue is done when the outcome is implemented or the research decision is documented, acceptance criteria are satisfied, evidence exists, required review is complete, and relevant docs are updated.

## Planning scale
Plan one milestone at a time. Keep future capabilities at roadmap or epic level until dependencies and scope become clear. Do not create 300 speculative issues simply to appear prepared.
