---
name: style-direction
description: >
  Practical style and visual direction for interfaces. Covers design direction, subtlety,
  corner radius as personality, borders, depth and shadows, opacity, buttons, and the
  relationship between form and function. Use when establishing visual direction, choosing
  component styles, deciding on depth/shadow strategy, designing buttons, or defining the
  overall look and feel. Trigger on: style, direction, look and feel, shadow, border, radius,
  corner radius, depth, button design, visual treatment, aesthetic, mood, personality.
---

# Style & Direction

Style is about art direction — how you want your designs to feel. Every visual choice (radius, shadow, border, opacity) communicates personality.

## Design Direction

Before choosing any visual treatments, define what you're going for:
- What adjectives describe the desired feel? (Bold, calm, playful, technical, luxury)
- What existing products share this energy?
- What typeface style fits? (Serif = established, geometric sans = modern, humanist = friendly)

Design a few key components in different directions before committing. The same layout in four different typefaces and color schemes can feel completely different.

## Subtlety

The difference between amateur and professional design is often subtlety:
- Shadows that are barely visible but create depth
- Hover states that shift 5% rather than 50%
- Color differences between sections of 2-3% brightness, not 20%
- Transitions at 200-300ms, not 500ms+

If a visual treatment is the first thing you notice, it's probably too strong. The best treatments are felt, not seen.

## Corner Radius as Personality

Corner radius is a spectrum from technical to friendly:
- **0-4px** — Sharp, precise, authoritative, technical
- **8-12px** — Balanced, modern, approachable (most common)
- **16-20px** — Soft, friendly, contemporary
- **Full rounding** — Playful, conversational, pill-shaped

**Mixing:** Fully rounded buttons and pills for friendliness + medium radius on content cards is a valid strategy. Sharp icons inside rounded containers create balanced tension.

**Consistency:** Whatever you choose, apply it systematically. Mixed radii without intention looks accidental.

## Borders

- Borders add visual weight. The thinner, the better (1px is usually sufficient).
- Use borders consistently or not at all within a section.
- Consider whether spacing alone creates sufficient separation — often it does.
- On dark backgrounds, borders become much more visible. Reduce opacity or eliminate.
- Border color should be a very light gray from your gray system, not a random value.

## Depth and Shadows

Choose a depth strategy and commit:

**Subtle shadows** (most common, safest):
- Small y-offset (2-4px), tight blur (8-16px), low opacity (5-15%)
- Creates gentle lift without weight
- Works for cards, dropdowns, modals

**Elevation system** (Material-influenced):
- Multiple shadow levels for different elevations
- Higher elements: larger offset, wider blur, slightly more opacity
- Consistent across all elevated elements

**No shadows** (flat/modern):
- Rely on background layers and spacing for depth
- Cleaner, lighter feel
- Requires stronger spacing system to maintain hierarchy

**Shadow mistakes to avoid:**
- Large blur + low opacity = muddy haze
- Mixing shadow and stroke on the same element without intention
- Different shadow values on peer-level elements
- Shadows on dark backgrounds (they barely work — use lighter borders or glow)

## Opacity

Opacity creates layering and subtle relationships:
- 10-20% of your accent color makes a highlight background
- 50-70% opacity text creates clear secondary hierarchy
- Overlay on images: 40-60% dark overlay makes text readable on any photo
- Disabled states: 40-50% opacity of the normal state

## Buttons

Buttons are the most interacted-with component. Get them right:

**Primary:** Strong fill with the accent color. High contrast text. This is your main CTA — one per section maximum.

**Secondary:** Outline/ghost style or lighter fill. Clearly less prominent than primary.

**Tertiary:** Text-only or minimal style. For less important actions.

**Rules:**
- Horizontal padding should be 2-3× vertical padding
- Text should be centered with comfortable breathing room
- Minimum touch target: 44×44pt on mobile
- Don't mix too many button styles on one screen
- Full-width buttons on mobile for primary CTAs in forms

## Form and Function

Form serves function. A beautiful button that doesn't look clickable fails. A readable label that looks like a button confuses.

- Interactive elements must look interactive
- Read-only elements must look static
- The visual treatment should match the behavioral expectation
- When form and function conflict, function wins every time

Every stylistic decision should be defensible: "I chose rounded corners because this is a consumer-friendly product" not "I just thought it looked nice."
