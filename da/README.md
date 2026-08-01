# Dockery Automations UI/UX Design Intelligence

This directory defines how Dockery Automations uses the existing UI UX Pro Max engine as a governed capability inside the DA Company Brain.

The underlying engine remains in `src/ui-ux-pro-max/` and continues to provide broad design intelligence, searchable rules, palettes, typography guidance, landing-page patterns, stack guidance, and UX recommendations.

The DA layer controls:

- what business and client context may be supplied
- which Dockery standards govern the work
- how client-specific information overrides general recommendations
- which tools and implementation targets are approved
- what the capability may and may not decide
- the required output structure
- the definition of done

## Responsibility boundary

This capability is responsible for transforming approved website context into a governed design system and UI/UX specification.

It is not responsible for:

- identifying or authenticating the client
- approving scope or pricing
- managing the full website-delivery workflow
- storing live job state
- publishing a production website
- changing canonical Dockery standards

## Source of truth

- General design intelligence: `src/ui-ux-pro-max/`
- DA governance and operating contract: `da/`
- Client-specific context: supplied at runtime by the DA Company Brain execution package

## Operating sequence

1. Receive a validated DA design request.
2. Validate required context against `CONTEXT-REQUIREMENTS.md`.
3. Query the underlying design-intelligence engine.
4. Apply Dockery standards, client brand constraints, and DA overrides.
5. Produce output matching `schemas/design-output.schema.json`.
6. Validate the result against `COMPLETION-CONTRACT.md`.
7. Return the governed design package to the website-delivery workflow.

## Governing files

- `CAPABILITY.md`
- `CONTEXT-REQUIREMENTS.md`
- `GOVERNANCE-RULES.md`
- `COMPLETION-CONTRACT.md`
- `schemas/design-input.schema.json`
- `schemas/design-output.schema.json`
- `overrides/prohibited-patterns.yaml`
