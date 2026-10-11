# Hut4Devs Architecture and Repository Boundaries

## Governing principle
Each repository owns a clear technical responsibility. Cross-repository behavior is defined by documented contracts and reviewed decisions, not duplicated assumptions.

## Organization-level .github repository
Owns:
- Product charter, roadmap, milestones, and product log.
- Architecture and decision records.
- Issue governance and contribution standards.
- Organization-wide security, privacy, and release expectations.
- Cross-repository links and onboarding guidance.

It does not replace implementation-specific documentation in each repository.

## Frontend
Owns:
- User interface, accessibility, navigation, and interaction states.
- Client-side validation and clear error presentation.
- Secure session handling consistent with the approved architecture.
- API consumption and user-facing consent and visibility controls.

Does not own authoritative authorization, financial state, or trust decisions.

## Backend and data
Owns:
- Application APIs, domain rules, persistence, and integrations.
- Authentication integration and server-side authorization.
- Validation, idempotency, reconciliation, audit records, and data retention.
- Private application data and authoritative application state.

Does not assume frontend checks are security boundaries. It does not put sensitive personal records on-chain.

## Soroban / Stellar
Owns:
- Approved smart-contract state and transition rules.
- Contract authorization and event semantics.
- On-chain verification, resource budgets, and Testnet workflows.
- Contract tests, deployment tooling, and chain-specific integration contracts.

Only data explicitly approved for on-chain use may be stored there. No identity documents, private accommodation details, personal payment records, or secrets on-chain.

## AI and automation
Owns:
- Approved model integrations, retrieval, evaluation, and automation workflows.
- Permission-aware access to approved knowledge.
- Model quality, cost, latency, monitoring, and fallback behavior.
- AI-specific abuse controls and evaluation.

AI does not become the source of truth for domain state or independently decide consequential outcomes.

## Cybersecurity and assurance
Cross-cutting responsibility across every repository:
- Threat modelling, security requirements, and risk tracking.
- Secure design reviews, authorization tests, and adversarial testing.
- Dependency and secret scanning, vulnerability handling, and incident response.
- Privacy, resilience, and release assurance.

Security is not deferred until a future cybersecurity milestone.

## Shared contracts
Cross-repository interfaces require:
- Named owner and version.
- Input/output schemas and validation rules.
- Authentication and authorization expectations.
- Error and retry semantics.
- Idempotency and consistency rules where applicable.
- Compatibility policy and contract tests.
- Privacy classification and logging restrictions.

## Change boundaries
A cross-repository change must identify every affected repository, interface, migration, test, and documentation update. Architecture changes require a decision record before broad implementation.
