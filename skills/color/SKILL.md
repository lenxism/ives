---
name: color
description: >
  Practical color system for interface design. Covers color selection methods, contrast and
  accessibility, structural vs interactive color, primary and secondary colors, color amount
  and modification, gradients, mastering grays, near-whites, and dark UI. Use whenever making
  color decisions, choosing palettes, checking contrast, designing dark mode, or working with
  grays. Trigger on: color, palette, contrast, accessibility, WCAG, dark mode, dark UI, gray,
  grey, gradient, accent color, brand color, background color, theme.
---

# Color

Color is powerful but dangerous. A few wrong grays can undermine an entire interface. Master the principles, and color becomes your strongest tool.

Read `references/color-knowledge.md` for detailed gray analysis and dark UI techniques.

## Color Selection Methods

Start with one of these approaches:
- **HSB method** — Pick a hue, then adjust saturation and brightness for variants. Most intuitive for creating cohesive palettes.
- **Brand-first** — Start with the brand's primary color, derive everything else from it.
- **Reference-first** — Find an interface you admire, extract its palette, then adapt.

## Contrast and Accessibility

Non-negotiable minimums:
- **Body text (16px regular):** 4.5:1 contrast ratio (WCAG AA)
- **Large text (18px regular, 14px bold):** 3:1 contrast ratio (WCAG AA Large)
- **Interactive elements:** Must be distinguishable without color alone (add icons, weight, underlines)

Placeholder text is a gray area: AA-large (3:1) is often the right balance — dark enough to read, light enough to not look pre-filled.

## Structural vs Interactive Color

**Structural colors** define the interface skeleton: backgrounds, containers, borders, dividers. Keep these neutral.

**Interactive colors** signal action: buttons, links, selected states, focus rings. Keep these vibrant and consistent.

Never let structural colors compete with interactive colors. If your background is colorful, your buttons lose their signal.

## The Gray System

The most critical color skill. Most interfaces need 3-5 carefully chosen grays:

1. **Dark text** — Primary content (e.g., #333 or a dark with slight hue)
2. **Medium gray** — Secondary text, icons, metadata
3. **Light gray** — Dividers, borders
4. **Lighter gray** — Backgrounds, hover states
5. **Near-white** — Subtle background differentiation

### Critical rule: keep grays in the same hue family

Twitter's grays all sit around hue 208-210 (cool blue). Pinterest uses warm, desaturated grays that complement their red brand. Gmail uses a scattered mix of warm and cool grays — and it shows.

**Never use fully desaturated grays (#999, #666, etc.) alongside colors.** Add a tiny amount of your primary hue's saturation to every gray. At 5-10% saturation, grays feel cohesive without looking tinted.

### Gray on colored backgrounds

Never place a fully desaturated gray on a colored background. Instead:
- Use the same hue as the background with adjusted saturation/brightness
- Or use black/white with reduced opacity so the background color bleeds through

## Primary and Secondary Colors

- **One primary accent** used sparingly for CTAs and focus. Consistency is more important than vibrancy.
- **Secondary colors** for status (green/success, red/error, yellow/warning) — choose versions that pass AA contrast.
- **Avoid** using more than 2-3 distinct hues in an interface. Fewer colors = more cohesion.

## Amount and Modification

Less color = more impact. When everything is colorful, nothing stands out. Use color as punctuation, not wallpaper.

To modify a color for different contexts (hover, pressed, disabled):
- **Darken** — Reduce brightness 10-20% for hover states
- **Lighten** — Increase brightness, decrease saturation for backgrounds
- **Opacity** — 10-20% opacity of your accent makes a subtle highlight background

## Gradients

- Subtle gradients (5-15% brightness difference) add depth without distraction
- Keep gradients in the same hue family — shifting hues creates a rainbow effect
- Light-to-slightly-less-light on backgrounds creates subtle dimensionality
- Bold gradients work for CTAs and hero elements, not structural backgrounds

## Dark UI

All the same principles apply but everything is harder. Read the reference file for detailed techniques.

**Key rules:**
- Don't just reverse colors. Dark mode requires a complete rethink.
- Pure black (#000) backgrounds rarely work outside OLED displays
- Use very dark grays with slight hue saturation (e.g., #161416 — removing green from hex creates a subtle purple-gray)
- Nail typography and layout FIRST, then tune colors. Dark backgrounds amplify every flaw.
- Reduce contrast: white text on dark backgrounds vibrates more than dark text on light. Use off-white (#E5E5E5 range).
- Borders and dividers show up dramatically on dark backgrounds — go much more subtle than you think.
- Less visual contrast between structural elements, MORE contrast for interactive/data elements.
