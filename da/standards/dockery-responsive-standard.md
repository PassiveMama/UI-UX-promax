# Dockery Responsive Standard

## Purpose

Define the minimum responsive behavior required for websites and interfaces produced through Dockery Automations.

## Governing Principle

The experience must remain understandable, usable, and complete across supported screen sizes. Responsive design is not a desktop layout reduced to fit a smaller screen.

## Required Validation Widths

At minimum, validate at representative widths near:

- 375px
- 768px
- 1024px
- 1440px

Additional breakpoints must be tested when the content, component behavior, platform, or approved client requirements demand them.

## Layout

Responsive layouts must:

- preserve content hierarchy
- avoid horizontal scrolling except for intentionally scrollable data regions
- prevent overlapping or clipped content
- maintain readable line lengths
- preserve adequate spacing
- adapt multi-column layouts intentionally
- keep primary actions visible and usable

## Navigation

Mobile and tablet navigation must:

- remain keyboard accessible
- expose its open and closed state
- provide a clear close mechanism
- preserve logical focus behavior
- prevent background interaction when a modal navigation pattern is used
- retain access to primary actions

## Typography

Text must remain readable without requiring horizontal scrolling or manual zoom for ordinary content.

Typography must scale intentionally. Large display text must not dominate smaller screens or push critical information below the fold without purpose.

## Images and Media

Images and media must:

- scale without distortion
- preserve essential content and focal points
- avoid unnecessary transfer size
- not cause layout shift that disrupts use
- provide responsive alternatives when a single crop cannot preserve meaning

## Components

Every component must define responsive behavior, including:

- cards
- forms
- tables
- dialogs
- navigation
- galleries
- hero sections
- calls to action
- data visualizations

Complex tables must use an approved responsive pattern rather than silently hiding important data.

## Touch Interaction

Touch targets must be large enough and spaced sufficiently to avoid accidental activation.

Hover-only information or actions are prohibited. Any hover behavior must have an equivalent touch and keyboard path.

## Content Priority

Content may be reordered or condensed only when meaning, required disclosures, and approved scope are preserved.

Critical content and primary actions must not disappear at smaller sizes.

## Testing Evidence

Responsive validation must record:

- widths tested
- browsers or rendering environments used
- orientation where material
- navigation result
- form result
- overflow result
- image and media result
- accessibility reflow result
- known exceptions

## Prohibited Patterns

Do not:

- hide required content to make a layout fit
- shrink controls below usable size
- rely on desktop hover interactions
- allow fixed-position elements to cover essential content
- use unexplained horizontal scrolling
- publish layouts with clipped text, overlapping elements, or inaccessible navigation
