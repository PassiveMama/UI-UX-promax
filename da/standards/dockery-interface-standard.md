# Dockery Interface Standard

## Purpose

Define the minimum interaction and interface quality required for Dockery Automations digital experiences.

## Governing Principle

The interface must help the user understand what is happening, what they can do, and what will happen next.

## Clarity

Every screen must have:

- one clear purpose
- a visible primary action when action is required
- labels that describe outcomes rather than internal system language
- clear status and feedback
- consistent terminology

Avoid exposing technical implementation details unless the user’s role requires them.

## Interaction States

Interactive elements must provide, where applicable:

- default state
- hover state
- focus state
- active or selected state
- disabled state
- loading state
- success state
- error state

No action may fail silently.

## Forms

Forms must:

- use persistent labels
- group related fields
- explain unusual requirements before submission
- identify required fields
- validate as close to the affected field as practical
- preserve user-entered data after recoverable errors
- confirm successful submission

Do not use placeholder text as the only field label.

## Buttons and Links

Buttons perform actions. Links navigate.

Labels must describe the result, such as:

- Submit Request
- Save Draft
- Approve Design
- Open Staging Site

Avoid ambiguous labels such as “Click Here,” “Continue” without context, or multiple identical actions with different results.

## Status and Progress

Long-running work must display:

- current status
- completed stages
- blocked conditions
- assigned next action
- approval requirements
- last meaningful update

The interface must distinguish between:

- not started
- in progress
- waiting for information
- waiting for approval
- failed
- completed

## Errors and Recovery

Error messages must state:

1. what happened
2. what was affected
3. what the user can do next
4. whether their prior work was preserved

Do not display raw system errors to general users when a clear operational explanation can be provided.

## Confirmation and Risk

Require confirmation before destructive, irreversible, financial, production, domain, or publishing actions.

Confirmation must name the actual consequence.

## Consistency

The interface must use consistent:

- terminology
- component behavior
- spacing logic
- status language
- navigation patterns
- icon meaning
- date and time presentation

## Accessibility

All interface components must comply with the Dockery Accessibility Standard.

## Prohibited Patterns

Do not use:

- hidden critical actions
- inaccessible custom controls when a native control works
- color as the only status indicator
- unexplained icons without accessible labels
- forced motion for essential understanding
- modal chains that trap the user
- success messages that disappear before they can be understood
