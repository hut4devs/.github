# Hut4Devs Product Roadmap

## Roadmap policy
This is a capability-based roadmap, not a fixed delivery-date promise. Progress depends on evidence, dependencies, security, and milestone exit criteria.

## M0  Product foundation and governance
Outcomes:
- Approve the Product Charter and initial problem hypothesis.
- Inventory existing repositories, prototypes, and reusable work.
- Establish product, architecture, decision, experiment, and issue logs.
- Define repository ownership, contribution rules, security baseline, and definition of done.
- Identify assumptions, risks, and unresolved decisions.

Exit gate:
- A reviewer can explain the target user, initial problem, non-goals, repository boundaries, and how new work is approved.

## M1  Discovery and validated scope
Outcomes:
- Conduct user research and document evidence.
- Map current workflows and pain points.
- Define personas or user roles, jobs, and permission expectations.
- Compare candidate problems by impact, frequency, feasibility, and risk.
- Select one core user journey and define success measures.

Exit gate:
- The first problem and MVP journey are supported by evidence, with known assumptions and measurable outcomes.

## M2  Core coordination MVP
Candidate capabilities:
- Authentication and authorization.
- Community membership and role boundaries.
- Accommodation records and shared responsibilities.
- Contribution records and activity history.
- Basic status tracking and transparent corrections.
- Minimum viable frontend, backend, data model, tests, and deployment workflow.

Exit gate:
- A test user can complete the approved core journey end to end.
- Permissions, failure paths, data handling, backups, and recovery have been validated.
- No unresolved critical security findings remain.

## M3  Peer support and accountability
Candidate capabilities:
- Gifts, contributions, and peer-support records.
- Lending terms, expected repayment dates, partial repayments, and balances.
- Overdue status and careful risk communication.
- Renegotiation, correction history, and dispute workflows.
- Notifications and community activity summaries.

Exit gate:
- Important state transitions are deterministic, auditable, tested, and understandable to affected users.

## M4  Trust trails and Stellar/Soroban
Candidate capabilities:
- Define which facts need external verification and why.
- Separate private application data from public verifiable evidence.
- Establish an approved event and data contract.
- Prototype Stellar Testnet integration and Soroban contract behavior.
- Test authorization, replay protection, resource budgets, failure recovery, and event interpretation.
- Document transaction boundaries and reconciliation.

Exit gate:
- A threat-reviewed, testable use case demonstrates a real benefit over an off-chain-only alternative.
- No personal or sensitive records are exposed on-chain.
- Production deployment requires a separate explicit approval gate.

## M5  AI and workflow automation
Candidate capabilities:
- Search and retrieve approved project knowledge.
- Summarize activity for authorized users.
- Assist with repetitive administrative workflows.
- Suggest inconsistencies or unusual activity for human review.
- Provide explainable, permission-aware recommendations.
- Evaluate model quality, cost, privacy, and failure behavior.

Exit gate:
- Each AI feature has a validated user need, evaluation dataset or test method, measurable quality criteria, privacy review, abuse analysis, and human fallback.
- AI cannot independently make consequential lending, dispute, access, or trustworthiness decisions.

## M6  Advanced cybersecurity and resilience
Candidate capabilities:
- Formal threat modelling and abuse-case reviews.
- Automated dependency, secret, and vulnerability scanning.
- Authorization and adversarial testing.
- Security monitoring, audit trails, incident response, and recovery exercises.
- Rate limiting, abuse prevention, and secure service-to-service communication.
- AI prompt-injection, data-exfiltration, model-output, and tool-permission defenses where AI is deployed.
- Independent security review for high-risk changes.

Exit gate:
- Release risks have owners and explicit acceptance decisions.
- Incident response, recovery, access revocation, and vulnerability handling have been exercised.
- No unresolved critical security findings remain.

## M7  Scale, ecosystem, and governance
Candidate capabilities:
- Reliability and performance improvements based on measured usage.
- Community onboarding and accessibility improvements.
- Maintainer and contributor experience.
- Approved integrations and interoperability.
- Governance, funding sustainability, and release management.
- Long-term observability, operational ownership, and support.

Exit gate:
- Scale work responds to observed usage and defined service objectives, not speculative demand.

## Cross-cutting requirements
Every milestone must consider:
- Security, privacy, consent, and data retention.
- Accessibility and user experience.
- Automated tests and failure-path validation.
- Documentation and operational support.
- Observability and recovery.
- Cost, feasibility, and maintainability.
- Contributor onboarding and governance.

## Change control
Roadmap changes require a recorded rationale, evidence or explicit assumption, affected milestones, dependencies, risks, and a decision-log entry.
