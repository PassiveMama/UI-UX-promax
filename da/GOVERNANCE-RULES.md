# Governance Rules

## Authority model

Each action must be classified as one of the following:

1. **Execute autonomously**
2. **Execute and report**
3. **Prepare and require approval**
4. **Prohibited**

## Execute autonomously

The capability may:

- search the approved design-intelligence sources
- compare relevant patterns, styles, colors, typography, components, and UX guidance
- apply approved client and Dockery constraints
- generate a draft design-system recommendation
- generate responsive and accessibility guidance
- generate platform-aware implementation guidance

## Execute and report

The capability may:

- exclude recommendations that violate approved client or Dockery rules
- choose among equally valid general design recommendations
- document conflicts and tradeoffs
- identify missing or weak design context
- recommend additional assets or research

## Prepare and require approval

Approval is required before:

- replacing approved client brand colors or typography
- deviating from approved website scope
- introducing a new third-party design dependency
- adopting a pattern that conflicts with a Dockery standard
- finalizing a design direction when multiple materially different options remain
- handing a design package to production when required client approvals are missing

## Prohibited

The capability must not:

- publish a production website
- alter pricing, claims, legal language, or approved content
- change canonical Company Brain standards
- access unrelated client information
- store secrets or credentials in generated artifacts
- use prohibited patterns listed in `overrides/prohibited-patterns.yaml`
- bypass accessibility requirements
- represent a recommendation as client-approved when it is not

## Traceability

Every output must record:

- capability version
- source context identifiers
- design-intelligence domains searched
- major rules applied
- conflicts or overrides
- unresolved approvals
- target implementation platform
