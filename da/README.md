# Dockery Automations UI/UX Design Intelligence

## Purpose

This directory is the Dockery Automations governance and integration layer for the UI UX Pro Max design-intelligence engine.

The original engine remains under `src/ui-ux-pro-max/` and continues to provide broad design knowledge, search, reasoning rules, and platform guidance.

The `da/` layer defines how Dockery Automations may invoke that engine during Client Website Delivery.

## Responsibility

This capability converts approved client, scope, brand, audience, platform, and Dockery-standard context into a governed UI/UX design specification.

It does not:

- identify the client
- approve scope
- manage the full website workflow
- publish a production website
- control domain, payment, or financial integrations
- promote execution observations into canonical Company Brain knowledge

## Version 1 Structure

- `CAPABILITY.md` defines the capability and its boundaries.
- `CONTEXT-REQUIREMENTS.md` defines required runtime context.
- `GOVERNANCE-RULES.md` defines authority and escalation rules.
- `COMPLETION-CONTRACT.md` defines what must be true for the output to be complete.
- `INTEGRATION-CONTRACT.md` defines the handshake with the Company Brain and execution engine.
- `schemas/design-input.schema.json` defines the accepted machine-readable input.
- `schemas/design-output.schema.json` defines the required machine-readable output.
- `overrides/prohibited-patterns.yaml` defines initial DA design prohibitions.
- `standards/` contains the core Dockery website, interface, accessibility, and responsive standards.

## Governing Priority

When recommendations conflict, apply this priority order:

1. approved client scope and legal requirements
2. client brand standards
3. Dockery Automations standards and governance
4. approved platform constraints
5. UI UX Pro Max recommendations

## Runtime Flow

```text
Website Delivery execution package
        ↓
Validate against design input schema
        ↓
Apply DA context, governance, standards, and overrides
        ↓
Invoke UI UX Pro Max design intelligence
        ↓
Validate against design output schema and completion contract
        ↓
Return governed design specification to the next Website Delivery stage
```

## Source of Truth

- Broad UI/UX engine: `src/ui-ux-pro-max/`
- DA usage governance: `da/`
- Company-wide Website Delivery authority and routing: Dockery Automations Company Brain

This repository is a specialized execution component. It does not replace the Company Brain.
