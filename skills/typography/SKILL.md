---
name: typography
description: >
  Practical typography system for interface design. Covers the rule of four (limit type sizes),
  font weight as meaning, typographic hierarchy, titles and body text, truncation, callouts,
  interactive text, combining text styles, system fonts, and alternate fonts. Use whenever
  making typography decisions: choosing fonts, setting sizes, establishing hierarchy, designing
  text-heavy interfaces, or reviewing typographic quality. Trigger on: font, type, typography,
  text size, font size, heading, body text, type scale, font weight, typeface, hierarchy,
  readability, text style.
---

# Typography

Typography is the most critical part of interface design. Sloppy, inconsistent usage of font sizes, weights, and colors is the clearest signal that a designer doesn't know what they're doing.

Read `references/typography-knowledge.md` for detailed examples and analysis of real-world apps.

## The Rule of Four

Limit yourself to a maximum of four type sizes or less. This rule can be broken, but only when you understand why the boundaries exist.

**The evidence:** Instagram's home screen uses essentially one type size (15pt) with only a smaller 12pt for story labels. Twitter uses three sizes for its entire timeline. iOS Settings uses two sizes on internal pages. Facebook Messenger's main screen: three sizes.

When apps use 5-6+ sizes (like Facebook's Discover tab), they immediately look disorganized and lack cohesion.

### The four roles

Most well-designed interfaces combine:
1. **Title** — Page or section titles
2. **Body/Subtitle** — Primary content, list items, navigation
3. **Action items** — Buttons, links, interactive elements (often same size as body, differentiated by color/weight)
4. **Metadata** — Timestamps, helper text, secondary info

You can often collapse these to 2-3 sizes. The fewer sizes, the cleaner the interface.

## Extending Without Adding Sizes

Change meaning without adding sizes by varying:

- **Color** — Same size, different color: black for titles, gray for subtitles, blue for actions
- **Weight** — Bold for names, regular for body, medium for interactive (Instagram uses subtle weight changes for actionable profile names)
- **Position** — Right-aligned text reads as a value/definition of the left-aligned label (iOS Settings pattern)
- **Decoration** — Underlines, background colors, or pill shapes on action items
- **Case** — ALL CAPS at a smaller size can serve as a section divider without adding a new size

## Font Weight as Hierarchy

Weight controls emphasis and interactive meaning:
- **Bold/Heavy** — Primary titles, emphasis
- **Semibold/Medium** — Interactive elements, secondary emphasis
- **Regular** — Body text, descriptions
- **Light** — Use very sparingly. Thin weights at small sizes become unreadable.

Never use more than 3 weights in a single view.

## Hierarchy Principles

- Create contrast between heading and body sizes — if they're too close, hierarchy collapses
- The title should be unmistakably the title without relying on position alone
- Within body content, use weight and color to create sub-hierarchy, not more sizes
- Metadata should be noticeably smaller — it's supporting information, not primary content

## System Fonts

System fonts (SF Pro, Roboto, Segoe UI) are a legitimate, strategic choice:
- **Familiarity** — Users read them unconsciously, getting to content faster
- **Performance** — No extra font loading, especially critical on web
- **Quality** — Apple and Google invest heavily in these typefaces
- **Reduced decisions** — Focus energy on other design choices

Using system fonts doesn't make you less of a designer. Master the fundamentals (size, weight, spacing, hierarchy) before relying on custom fonts to carry the design.

## When to Go Custom

Venture outside system fonts when:
- The brand already has a specific typeface
- You need to convey a specific personality system fonts can't deliver
- You've mastered the fundamentals and want to differentiate
- The project is web-based (more opportunity for custom display fonts)

When going custom, test the font on numbers, not just words. Odd number forms undermine otherwise good choices.

## Practical Rules

- Body text on mobile: 15-17pt is the sweet spot
- Never go below 11-12pt for any interface text
- Line height: 1.4-1.6× for body text, tighter for headings
- Letter-spacing: tighten for large display text, default or slightly loose for body
- Use `tabular-nums` / monospace for numbers that change (prices, stats, timestamps)
- Truncate with ellipsis when space is constrained, but ensure the truncated version still communicates
