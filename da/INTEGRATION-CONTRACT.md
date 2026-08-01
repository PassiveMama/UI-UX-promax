# DA UI/UX Design Intelligence Integration Contract

## Purpose

This contract defines how the Dockery Automations Company Brain invokes the DA UI/UX Design Intelligence capability during Client Website Delivery.

The original UI UX Pro Max engine supplies broad design intelligence. The `da/` layer governs how Dockery Automations uses that intelligence.

## Authorized Invokers

This capability may be invoked by:

- the Dockery Automations execution engine
- an approved Website Delivery workflow
- an authorized human operator acting through the DA work interface
- an approved testing workflow using non-production client data

Direct ad hoc invocation that bypasses the Company Brain is not approved for production work.

## Invocation Point

The capability is invoked after:

1. the client has been uniquely identified
2. approved scope has been retrieved
3. required client context has been assembled
4. Website Delivery Process DNA has reached the design-intelligence stage
5. readiness requirements for this stage have been satisfied

It is invoked before:

- final wireframe production
- visual design production
- production website build

## Required Input

Every invocation must validate against:

`da/schemas/design-input.schema.json`

Required inputs include:

- execution ID
- client ID
- client business context
- audience context
- approved scope and pages
- client brand rules
- governing Dockery standards
- approved implementation target
- known constraints and prohibited patterns

If required context is missing, the capability must return a structured blocked result. It must not invent missing client facts.

## Processing Rules

The capability must:

1. preserve the client’s approved brand requirements
2. apply Dockery standards before generic design recommendations
3. search only the design domains required for the request
4. exclude prohibited patterns and conflicts
5. explain material recommendations
6. return a structured design specification
7. include validation evidence and unresolved decisions

Priority order:

1. approved client scope and legal requirements
2. client brand standards
3. Dockery Automations standards and governance
4. approved platform constraints
5. UI UX Pro Max recommendations

## Required Output

Every successful invocation must validate against:

`da/schemas/design-output.schema.json`

The output must include, as applicable:

- selected page pattern
- recommended visual direction
- page and section structure
- color and typography specification
- component recommendations
- responsive rules
- accessibility rules
- interaction guidance
- prohibited patterns
- implementation target
- validation checklist
- unresolved decisions requiring human review

## Output Destination

The execution engine stores the runtime output in the active Website Delivery job record and records:

- repository name
- capability version
- branch, tag, or commit SHA used
- input schema version
- output schema version
- generated artifact location
- validation result

The Company Brain stores the authoritative capability relationship and approved version reference. Client-specific outputs remain with the client job and designated artifact storage unless preservation rules require a governed summary.

## Downstream Handoff

The structured output may be passed to approved downstream operators, including:

- Figma design workflow
- Base44 website build workflow
- GoHighLevel website or funnel workflow
- approved frontend development agent
- independent QA workflow

Downstream operators may implement the specification but may not silently override its governing constraints.

## Failure States

Supported failure states:

- `blocked_missing_context`
- `blocked_conflicting_requirements`
- `failed_input_validation`
- `failed_engine_execution`
- `failed_output_validation`
- `requires_human_decision`

Every failure must return:

- failure state
- reason
- affected requirement
- whether work may continue elsewhere
- assigned next action
- required resumption input

## Approval Rules

The capability may autonomously produce recommendations and draft specifications within approved authority.

Human approval is required when:

- client brand requirements conflict with Dockery standards
- the scope is ambiguous
- a major visual direction materially affects approved positioning
- legal, accessibility, payment, domain, or production risk is involved
- the requested result requires an unapproved tool or pattern

Production publishing is outside this capability’s authority.

## Versioning

Every execution must pin the approved capability version and repository commit SHA. New executions use the latest approved version. In-progress executions remain on their pinned version unless an authorized migration is recorded.

## Completion

The invocation is complete only when:

- input validation passes
- required design intelligence is generated
- DA standards and overrides are applied
- output validation passes
- unresolved decisions are clearly identified
- the result is stored and handed to the correct downstream stage
