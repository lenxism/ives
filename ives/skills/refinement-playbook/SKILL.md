---
name: refinement-playbook
description: >
  Step-by-step process for iteratively improving an existing interface. Works through a
  specific sequence: remove redundancy, simplify visual treatments, tighten spacing, establish
  consistency, improve hierarchy, improve data visualization, refine interactions, and craft
  details. Use when improving, polishing, refining, or iterating on any existing UI. Trigger
  on: improve this, make this better, polish, refine, iterate, tighten up, clean up, push
  further, next level, before/after, ship quality, production ready.
---

# Refinement Playbook

Each change may seem small on its own, but through deliberate choices to remove redundancy, simplify treatments, and let content speak, the interface transforms.

## The Refinement Sequence

Work through these categories in order. Each builds on the previous.

### 1. Remove Redundancy

Start by eliminating what doesn't need to exist.

- **Redundant labels.** If the page title says "Analytics," the subtitle "Your analytics dashboard" adds nothing. Remove it.
- **Duplicate visual signals.** If color indicates state, you don't also need an icon and a label.
- **Unnecessary containers.** Four separate cards for four sibling metrics create noise. A single consolidated scoreboard reads better.
- **Verbose headers.** "Edition Performance" → "Performance." "Top Performing Links" → "Top Links."

**The test:** For every element, ask: "If I removed this, would meaning be lost?" If no, remove it.

### 2. Simplify Visual Treatments

- Reduce stroke weight — heavy borders add noise. Consider removing strokes entirely if spacing creates sufficient separation.
- Tighten shadow blur radius and y-offset for crisper depth.
- Reserve display typefaces for page titles only. Section headers work better in clean sans-serif.
- Establish a clear typographic scale: 2-3 sizes maximum for body content.
- Use dividers consistently or not at all. Often, spacing alone is sufficient.

### 3. Tighten Spacing and Proportion

This is where most interfaces feel "off" without people being able to articulate why.

- **Balance padding within containers.** Too much vertical padding at top creates top-heaviness.
- **Reduce gaps between related elements.** Labels and values, icons and text should feel tightly coupled.
- **Increase gaps between unrelated sections.** Make grouping obvious through spacing.
- **Equalize gaps between peer sections.** Inconsistent spacing between siblings feels uneven.
- **Optical alignment.** Elements sharing a left edge should *actually* share it — across nested containers.

### 4. Establish Visual Consistency

- **Icons:** Align stroke widths, align colors, use one style (all outline or all filled).
- **Color:** Reduce distinct colors. Align chart colors with overall language. Use color for meaning, not decoration.
- **Components:** If you use cards, use them the same way throughout. If badges, style consistently.
- **Dividers:** If one list has dividers, peer lists should too (or neither should).

### 5. Improve Information Hierarchy

- **Scoreboard metrics:** Move supporting values inline. Don't stack label→metric→value vertically when horizontal works.
- **Table columns:** At summary altitude, show only 3-4 most important columns. Details belong in detail view.
- **Charts:** Remove vertical dashed grid lines. Reduce x-axis labels to key dates. Simplify default state.

### 6. Improve Data Visualization

- Use row backgrounds to indicate relative performance instead of tiny compressed bars.
- Replace domain text with favicons for visual interest and faster scanning.
- Style category labels as tokens/badges to differentiate from user-entered text.
- Use monospace or `tabular-nums` so digits don't jump as values change.

### 7. Refine Interactions

Push beyond functional to exceptional. For any interactive component:

1. Consolidate separate elements into single containers
2. Make the entire surface the interaction target, not a tiny handle
3. Scale labels proportionally to control size
4. Add subtle affordances on hover that acknowledge interaction
5. Handle edge cases (value overlap, boundary behavior)
6. Add spring animation for state transitions
7. Consider making values directly editable on delay

Each refinement is small. Together, they create something exceptional.

### 8. Craft Details

The final layer — details that signal someone deeply cared:

- Dynamic sounds that cycle through variations
- Parallax effects that respond to cursor position
- Spring-based 3D rotation on interactive elements
- Spotlight masks that constrain effects to feel like real light
- Personalized touches for specific contexts

These aren't found in a PRD. They're breadcrumbs of care.

## The Refinement Mindset

**After each change, look again.** Every change shifts the balance. After tightening spacing, typography might feel too large. Refinement is continuous rebalancing.

**Name the before and after.** For each refinement: what was wrong, what you changed, why it's better.

**Small changes, compound effect.** Don't dismiss "too small to matter." The before/after should be dramatic even if no single step was.

**Know when to stop.** Stop when: every element justifies its existence, visual language is consistent, hierarchy is clear, spacing is balanced, and further changes feel preferential rather than objectively better.
