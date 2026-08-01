# Completion Contract

The DA UI/UX Design Intelligence capability is complete only when every required condition below is satisfied or explicitly marked as blocked with an assigned next action.

## Required output sections

- validated request summary
- client and project identifiers
- design rationale
- recommended page or landing-page pattern
- page-level structure
- visual style direction
- color system
- typography system
- component guidance
- interaction and motion guidance
- responsive behavior
- accessibility requirements
- prohibited patterns and anti-patterns
- implementation guidance for the approved platform
- downstream validation checklist
- source and decision traceability

## Required validations

- output matches approved scope
- client brand constraints are honored
- Dockery standards are applied
- client-specific rules take precedence over general recommendations
- text and interface contrast requirements are defined
- keyboard, focus, reduced-motion, and responsive requirements are addressed
- all scoped pages or interface areas are covered
- no unsupported client facts or approvals are invented
- no prohibited design pattern is included
- output conforms to `schemas/design-output.schema.json`

## Completion states

### Passed

All required sections and validations are complete.

### Conditionally passed

The package is usable for approved downstream work, but clearly identified later-stage inputs or approvals remain outstanding.

### Blocked

A required input prevents a reliable design package. The response must identify:

- the missing item
- why it is required
- the stage it blocks
- the responsible person or system
- the action needed to resume

### Failed

The output violates governance, cannot be traced to approved context, or does not satisfy the required schema.

## Evidence

The completion record must include:

- validation results
- unresolved items
- approvals required
- capability and source versions
- generated artifact location
