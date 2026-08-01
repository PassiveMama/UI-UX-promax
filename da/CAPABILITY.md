# Capability: DA UI/UX Design Intelligence

## Capability ID

`da-ui-ux-design-intelligence`

## Purpose

Transform approved client, business, website, brand, audience, and implementation context into a governed UI/UX design system and page-level design specification that can be executed by approved human or AI operators.

## Trigger

This capability is invoked by the Client Website Delivery process after:

- the client has been resolved
- the website scope is approved
- required business and audience context has been retrieved
- applicable Dockery and client standards have been identified

## Inputs

Inputs must conform to `schemas/design-input.schema.json`.

## Outputs

Outputs must conform to `schemas/design-output.schema.json`.

## Core responsibilities

1. Interpret the approved design brief.
2. Search the underlying UI/UX intelligence domains.
3. Select an appropriate page pattern, visual direction, typography approach, color usage, component strategy, interaction guidance, and accessibility requirements.
4. Apply client brand constraints before general recommendations.
5. Apply Dockery standards and prohibited-pattern rules.
6. Produce implementation guidance for the approved build platform.
7. Return validation criteria for downstream design, build, and QA work.

## Non-responsibilities

This capability must not:

- invent missing client facts
- change approved scope
- select a client without a verified client ID
- approve claims, pricing, legal language, or production publishing
- override client brand requirements without an explicit conflict record
- alter canonical Company Brain knowledge directly
- create or manage the top-level workflow

## Relationship to the Company Brain

This capability is an executable component of the DA Company Brain. It supplies governed design intelligence to the Client Website Delivery Process DNA. The workflow engine may invoke it, but the workflow engine does not define its methods, authority, or completion criteria.

## Success condition

The capability succeeds when it produces a complete, traceable, platform-aware design package that satisfies `COMPLETION-CONTRACT.md` and can be used by downstream design and build operators without inventing the design system themselves.
