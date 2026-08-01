# Context Requirements

## Required before invocation

The capability must not begin until these values are present and verified:

- client ID
- client display name
- approved website scope
- primary website goal
- approved page list or page requirements
- business type or industry
- primary audience
- approved build platform

## Required before final design package

- client brand profile
- approved logo or logo status
- approved brand colors or explicit permission to recommend colors
- voice and tone guidance
- services, programs, products, or offers represented on the website
- required calls to action
- accessibility requirements
- required integrations
- legal or compliance constraints that affect interface design

## Optional context

- competitor or inspiration references
- prior website analytics
- customer research
- photography or illustration preferences
- content inventory
- existing component library
- approved motion preferences
- localization requirements

## Context precedence

When sources conflict, apply this order:

1. approved client-specific requirements
2. approved contract or scope
3. Dockery governance and accessibility standards
4. approved client brand standard
5. Dockery website and interface standards
6. DA overrides in this repository
7. general UI UX Pro Max recommendations

The conflict must be recorded when a higher-precedence source overrides a lower-precedence recommendation.

## Missing-information behavior

- Do not invent missing facts.
- Classify each missing item as blocking, required before a later stage, optional, or safely inferable under governance.
- Return a structured missing-information response when a blocking item is absent.
- Continue only with stages that are not blocked.

## Retrieval boundaries

Load only the client and Company Brain context required for this capability. Do not load unrelated clients, capabilities, draft standards, deprecated files, or unrestricted communication history.
