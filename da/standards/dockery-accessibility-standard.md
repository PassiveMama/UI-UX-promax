# Dockery Accessibility Standard

## Purpose

Define the minimum accessibility requirements for websites and interfaces produced through Dockery Automations.

## Governing Principle

Accessibility is a required quality condition, not an optional enhancement.

## Minimum Standard

Design and implementation should meet WCAG 2.2 Level AA unless a stricter contractual, legal, platform, or client requirement applies.

## Structure and Semantics

Every experience must:

- use semantic headings in logical order
- use landmarks and native elements where appropriate
- provide meaningful page titles
- preserve a logical reading order
- associate labels with form controls
- use tables only for tabular data

## Keyboard Access

All interactive functions must be operable by keyboard.

Requirements include:

- visible focus indicators
- logical focus order
- no keyboard traps
- keyboard access to menus, dialogs, forms, and controls
- skip navigation where repeated navigation materially affects use

## Color and Contrast

Text and essential interface elements must meet applicable contrast requirements.

Color must not be the only way information, status, validation, or required action is communicated.

## Images and Media

- Informative images require meaningful alternative text.
- Decorative images must be ignored by assistive technology.
- Video requires captions when speech or meaningful audio is present.
- Audio-only content requires an equivalent transcript when required.
- Autoplay with sound is prohibited.

## Forms

Forms must provide:

- persistent labels
- programmatic instructions
- clear required-field identification
- accessible error identification
- error recovery guidance
- confirmation of successful submission

## Motion and Timing

- Respect `prefers-reduced-motion`.
- Do not require animation to understand content.
- Avoid flashing content.
- Provide controls for time-sensitive interactions when applicable.

## Responsive Accessibility

Accessibility must be validated across required screen sizes and orientations. Reflow must not hide content, controls, labels, or focus indicators.

## Testing Evidence

Version 1 validation must include:

- automated accessibility scan
- keyboard review
- heading and landmark review
- color contrast review
- form label and error-state review
- responsive reflow review

Automated testing alone is not sufficient.

## Exceptions

Any known exception must record:

- affected criterion
- reason
- user impact
- mitigation
- responsible approver
- remediation plan when applicable

## Prohibited Patterns

Do not:

- remove focus outlines without an accessible replacement
- use text embedded in images as the only content source
- use inaccessible CAPTCHA without an alternative
- hide required information from assistive technology
- create controls without names, roles, or states
- publish known critical accessibility failures without authorized exception
