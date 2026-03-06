---
name: tactics
description: >
  Practical workflow tactics for interface design projects. Covers the no-stress design
  process, low-fidelity design (when and how to wireframe), responsive design, platform
  guidelines (iOS HIG and Material), organizing design files, design reviews, developer
  handoff, and prototyping strategy. Use when planning a design project, deciding on process,
  discussing wireframes, preparing for handoff, or thinking about responsive design.
  Trigger on: wireframe, low fidelity, process, workflow, handoff, responsive, prototype,
  organize, present, review, stakeholder, developer, iOS guidelines, material design,
  platform guidelines.
---

# Tactics

Practical workflow tactics for executing design projects effectively.

## The No-Stress Design Process

Don't start with a blank canvas and pray. Follow this:

1. **Ask questions.** Anything you can't confidently explain about the project means you're not equipped to design it. Know the stakeholders, who has final call, colors off-limits, what they hate about current design.

2. **Determine direction.** Based on what you've learned, experiment with typefaces, color moods, adjectives. Mock up the same component in 3-4 different type treatments. Typography sets the tone for everything.

3. **Focus on components, not pages.** Design the navigation, a card, a button, a header background — in abstract. Not a full homepage. These pieces establish the visual language without the pressure of a complete layout.

4. **Have conversations, not presentations.** Share early and often. "Here's a direction we could take" beats "here's the final design." Get gut reactions. Paint a picture of what *could be*, not what *is*.

This builds trust incrementally and avoids the terrifying big reveal that risks total rejection.

## Low Fidelity Design

### When to wireframe
- Project is big and complex with lots of moving parts
- Team is large with multiple stakeholders
- Functionality isn't clear yet
- You need developer input on feasibility before investing in visual design

### When NOT to wireframe
- Solid UI foundation already exists (you're extending, not creating)
- Functionality is straightforward
- You're doing a visual refresh on existing structure
- Time is extremely limited and the scope is clear

### How to do it well
- Call them "low fidelity designs" not "wireframes" — less baggage
- Use a vanilla system: one typeface, black/white/gray/one blue accent
- Make primary actions unmistakable (blue, bold, black borders if needed)
- Focus on layout, functionality, and flow — save typography/color/style for later
- Spend as little time as possible while gaining ground on functionality decisions
- Transition to high fidelity once the team agrees on what the thing does

## Responsive Design

- **Start mobile-first.** The constrained canvas forces prioritization.
- At each breakpoint, reconsider density and layout — don't just stretch.
- Common breakpoints: 375px (mobile), 768px (tablet), 1024px (small desktop), 1440px (desktop)
- Navigation transforms: bottom tabs (mobile) → sidebar (desktop)
- Cards reflow: single column → 2 → 3 → 4
- Typography may need slight size adjustments between mobile and desktop
- Test content at extremes — long names, empty states, maximum data

## Platform Guidelines

### iOS (Human Interface Guidelines)
- Tab bar at bottom for primary navigation
- Standard push/pop navigation with back button
- SF Pro as system font
- 44pt minimum touch targets
- Respect safe areas (notch, home indicator)
- Standard table views for settings and lists

### Material Design (Android)
- Bottom navigation (current) or top tab bars
- Floating Action Button for primary creation actions
- Roboto as system font
- More geometric, sharp components vs iOS's rounder feel
- Material elevation system with shadows

### Cross-platform
Many apps (Airbnb, Slack) use a hybrid approach — their own design language that feels comfortable on both platforms. This is increasingly common and acceptable.

## Developer Handoff

- Export at 2× minimum for retina; divide displayed size by 2
- Spec spacing, sizes, and colors explicitly — don't assume developers will measure
- Note all states: default, hover, focus, active, disabled, error, loading, empty
- Provide real content, not lorem ipsum — wrong content in handoff causes rework
- Consider whether assets should be rasterized (PNG), vector (SVG), or recreated in code
- For marketing sites, interactive elements may be worth recreating in CSS/JS

## Design Reviews

Present work in a format that invites productive conversation:
- Show work in context (on device, in browser) not just in the design tool
- Lead with the problem being solved, then the solution
- Point out what you're unsure about — it disarms critics and focuses feedback
- Request specific feedback ("Does this hierarchy feel right?") over open-ended ("What do you think?")
