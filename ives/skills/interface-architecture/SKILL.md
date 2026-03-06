---
name: interface-architecture
description: >
  Guide structural interface decisions — the bones of a design before visual polish.
  Covers platform defaults, separation of concerns, information architecture, visual language
  definition (typeface, color, radius, icons, depth), and interaction model optimization.
  Use when building a new interface, choosing layouts, establishing visual languages, making
  structural decisions, or defining design direction. Trigger on: new project, architecture,
  layout, visual language, design system, design direction, structural, wireframe, information
  architecture, navigation structure, component structure.
---

# Interface Architecture

Getting architecture right means the interface feels intuitive even before it looks beautiful. Getting it wrong means no amount of polish saves it.

## Start with Defaults

Ask: "What would default iOS give us?" or "What would shadcn + Tailwind look like?"

This establishes the most conventional, familiar solution — then you optimize.

**iOS defaults:** Tab bars for peer destinations, table views for lists, push navigation for drill-down, sheets for focused tasks.

**Web defaults:** Sidebar navigation for apps, top nav for marketing, card grids for browsable content, modals for focused tasks.

The best products — Family, Raycast, Linear — show deep respect for platform conventions while innovating on every aspect. Understand the standard, match it, then exceed it.

## Separation of Concerns

Before diving in, identify what question you're answering, then go only as far as needed:

- **Architecture:** Right interaction model? (Don't need visual design yet)
- **Layout:** Information structure make sense? (Don't need final content)
- **Visual Language:** Colors, type, spacing convey right attributes? (Test on isolated components)
- **Polish:** Details refined? (Only after everything above is resolved)

Working on everything at once leads to rabbit holes and compounding rework. Slow is smooth, smooth is fast.

### Fidelity decisions

- **Testing interaction model:** White cards with shadows, no content. Just the interaction.
- **Exploring architecture:** Simple boxes and labels. Just the structure.
- **Refining visual language:** Component playground. Just the aesthetic.
- **Shipping:** Full fidelity. Everything considered.

## Information Architecture

### Reduce cognitive load through grouping
A flat list of 40+ items overwhelms. Group into phases, categories, or sections. Natural chunking makes the whole feel manageable.

### Progressive disclosure
- **Root level:** Show phases/categories, not all items
- **Drill-down:** Items within the selected group
- **Detail:** Full information for the selected item

Each level should feel like entering a focused workspace, not drowning in more.

### Adapt to user progress
- Auto-expand and scroll to current section
- Collapse completed work to reduce noise
- Emphasize "what's next" over "what's done"

## Establishing Visual Language

Before applying to full interfaces, define on isolated components. Play with attributes in a simple workspace.

### Define guiding attributes
Ask: what should the user *perceive*? Define 3-5 attributes specific to your product:

- Trust, Calm, Expertise (legal/financial app)
- Crafted, Fidgetable, Authentic, Inventive (creative tool)
- Fast, Precise, Minimal (developer tool)

These guide every visual decision.

### Typeface selection
**Body:** System standard (SF Pro, Segoe UI) often works best — familiar, "undesigned" in a good way. Use system fonts confidently. They're not a compromise; they're a strategic choice that removes one decision and lets you focus on others.

**Display:** Match your guiding attributes:
- Serifs → established, mature, trustworthy
- Geometric sans → modern, clean, technical
- Humanist sans → warm, approachable, friendly

Test your display font on numbers, not just words.

### Corner radius
- **Sharp (0-4px):** Precise, technical, authoritative
- **Medium (8-12px):** Balanced, modern, approachable
- **Full rounding:** Friendly, playful, conversational

You can mix: fully rounded CTAs for friendliness, medium radius on content cards.

### Icons
Icon style should complement, not mirror, container style. Soft containers + sharp icons = balanced. Consistency is critical: don't mix filled and outline, keep stroke widths uniform.

### Color
- Start with a warm or cool neutral palette for the emotional baseline
- Reserve one accent color used sparingly for focus and action
- Heavy use of off-whites allows pure white to signal focused content areas
- Avoid color as background everywhere — it becomes noise

### Depth strategy
Choose one and commit:
- **Strokes:** Clear boundaries, can feel heavy if overdone
- **Shadows:** Depth and elevation, can feel muddy if not crisp
- **Background layers:** Subtle, soft, avoids visual weight
- **Blur layers:** Modern, soft separation without hard edges

Don't mix strategies without intention.

## Interaction Models

**Sheets over pushes** for short, focused tasks — keeps user anchored, tighter feedback loop.

**Evaluate tab bars critically** — secondary features (settings, profile) often aren't true peers to the core flow. Consider header icons, inline inputs, fewer tabs.

**Collapse completed work** — once done, it doesn't need valuable space.

## Refine Language

Clinical labels create distance. Warm language creates support.
- Use "your" for ownership
- Use plain verbs over formal nouns
- Remove jargon from surface-level labels
- Add context: why a phase matters, time estimates, what they'll need

## Checklist

1. Start with platform defaults, then improve
2. Identify the concern you're resolving before diving in
3. Work at appropriate fidelity for the decision
4. Group and progressively disclose information
5. Define guiding attributes before choosing visual treatments
6. Test visual language on components before full interfaces
7. Optimize interaction models for your specific product
8. Warm up the language
