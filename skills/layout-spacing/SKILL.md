---
name: layout-spacing
description: >
  Practical layout and spacing system for interface design. Covers the box model, grids
  and containers, implicit grids, negative space, alignment, optical vs mathematical spacing,
  high vs low density, scale and visual weight, affordance, and interactive layouts. Use
  whenever making layout decisions, spacing adjustments, alignment choices, or structuring
  interface components. Trigger on: layout, spacing, padding, margin, grid, alignment, gap,
  negative space, whitespace, density, proportion, container, box model, responsive, position.
---

# Layout & Spacing

The tri-factor of beautiful design is good typography, good negative space, and good alignment. Layout is where most interfaces feel "off" without anyone being able to articulate why.

Read `references/layout-knowledge.md` for detailed analysis and examples.

## The Box Model Mindset

Every interface element is a box. Master the box model and you master layout:
- **Content** — The actual text, image, or element
- **Padding** — Space between content and its container edge
- **Border** — The container boundary (visible or not)
- **Margin** — Space between this container and neighboring elements

Consistency in these values across your interface is more important than the specific values chosen.

## Grids and Containers

Use grids as guides, not prisons. The implicit grid — alignment edges that emerge naturally from your content — is more important than a formal column grid.

**Key principles:**
- Establish strong left and right edges early
- Content within a container can create a new indented left edge to show ownership (parent-child relationship)
- Align everything to as few vertical rules as possible
- When elements share an alignment edge, the eye groups them as related

## Negative Space

Negative space is not empty space — it's a design tool.

- **Between related items:** Keep tight. Labels and values, icons and text should feel coupled (8-12px).
- **Between unrelated sections:** Keep generous. Make grouping obvious (24-48px+).
- **Around primary content:** More space = more importance. Give key elements room to breathe.
- **Inside containers:** Balance padding so content feels centered or slightly top-aligned, never bottom-heavy.

The ratio between inner spacing and outer spacing communicates hierarchy. Items with tight internal spacing and generous external spacing read as cohesive groups.

## Alignment

### Left-edge alignment
The most critical alignment in interface design. A strong left edge:
- Creates a visual anchor the eye returns to
- Groups related content
- Makes scanning efficient

Break the left edge intentionally to show hierarchy: indent child elements 16-20px from their parent title to indicate ownership.

### Optical vs mathematical alignment
Sometimes mathematically centered elements look off-center. Trust your eyes over the numbers. Common cases:
- Triangular play icons need to shift right slightly to look centered
- Text with descenders may need visual adjustment
- Icons with asymmetric shapes need optical centering

Always verify alignment visually at 100% zoom.

## Density

### High density
For power users, data-heavy interfaces, dashboards:
- Tighter spacing between rows (32-40px row height)
- Smaller type sizes (13-14px)
- More information visible without scrolling
- Use borders/dividers to maintain clarity at tight spacing

### Low density
For consumer apps, first-time experiences, content-focused:
- Generous spacing (48-64px+ row height)
- Larger type (16-18px)
- More breathing room
- Let content hierarchy do the heavy lifting

Match density to context. A messaging app needs different density than a stock trading platform.

## Scale and Visual Weight

- Larger elements carry more visual weight and draw attention first
- Dark elements weigh more than light ones
- Saturated color weighs more than desaturated
- Elements with borders/shadows weigh more than flat elements
- Use weight intentionally to direct the user's eye

## Affordance

Make interactive elements look interactive:
- Buttons should look tappable (sufficient size, contrast, depth)
- Input fields should look like you can type in them (inset appearance, placeholder text)
- Links should be distinguishable from static text
- Minimum touch target: 44×44pt on mobile

When in doubt about whether something looks interactive, it probably doesn't. Add more visual differentiation.

## Practical Spacing System

Use a consistent spacing scale. Common base: 4px or 8px.

- **4px** — Micro adjustments, icon-to-label gaps
- **8px** — Tight coupling, internal component spacing
- **12px** — Default small gap
- **16px** — Standard internal padding
- **24px** — Section separation within a container
- **32px** — Between distinct sections
- **48px+** — Major section breaks, page-level separation

Pick values from your scale. Avoid arbitrary spacing like 13px, 21px, 37px.
