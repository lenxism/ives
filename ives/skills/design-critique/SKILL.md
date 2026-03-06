---
name: design-critique
description: >
  Structured framework for reviewing and critiquing interfaces. Provides specific, tangible
  observations across four lenses: visual design, interface design, interaction consistency,
  and user context. Use when reviewing, critiquing, auditing, giving feedback on, or
  self-evaluating any UI — components, pages, apps, dashboards, or visual artifacts.
  Also activate for self-critique before presenting any design output. Trigger on words like:
  review, critique, feedback, audit, evaluate, improve, what's wrong, how to make better,
  polish, refine, assess quality.
---

# Design Critique

The goal is specific, tangible observations — not vague feedback. Every observation includes: what you see, why it matters, and what it could be instead.

## Step 1: Establish Context

Before diving in:
- What is this product/feature? Who uses it?
- What emotional or functional job is it doing?
- What platform? (iOS, web, Android — each has different standards)
- What's the intended quality bar? (MVP, production, premium?)

## Step 2: First Impressions (30 seconds)

Look at it as a user would on first encounter:
- What's the immediate emotional reaction? Trust, confusion, delight, anxiety?
- Where does your eye go first? Is that the right place?
- Does this feel like it belongs on its platform?
- Does it meet the industry standard bar?

## Step 3: Systematic Review — Four Lenses

### Lens 1: Visual Design

**Typography**
- Is there a clear typographic scale with intentional hierarchy?
- Are headline and body fonts well-chosen for context?
- Limit to 3-4 type sizes maximum. More signals a lack of system.
- Are numbers using tabular figures where values change?
- Is letter-spacing appropriate? (Tighter for large display, looser for small caps)

**Color**
- Is color used intentionally, or scattered without purpose?
- Too many colors competing? Could you achieve the same with fewer?
- Sufficient contrast for readability?
- One clear accent color, or multiple vying for attention?
- Are grays consistent in hue? (All warm, all cool — not mixed randomly)

**Spacing & Proportion**
- Is padding balanced within containers?
- Are gaps between related elements tight enough to show relationship?
- Are gaps between unrelated sections large enough to show separation?
- Do containers feel proportionally balanced?

**Visual Weight & Noise**
- Are border strokes heavier than necessary?
- Are shadows muddy or crisp? Do they serve a purpose?
- Is there unnecessary visual containment?
- Are decorative elements earning their place?

**Consistency**
- Icon styles consistent? (Don't mix filled and outline)
- Stroke widths consistent across the interface?
- Corner radius language consistent and intentional?
- Dividers used consistently or arbitrarily?

### Lens 2: Interface Design

**Hierarchy & Focus**
- Clear visual entry point?
- Layout has a narrative — a clear reading order?
- Primary actions emphasized over secondary ones?

**Information Density**
- Right amount of information for this altitude/context?
- Summary views stuffed with detail that belongs in detail views?
- Could progressive disclosure reduce overwhelm?

**Language & Labels**
- Labels clear and human, or clinical and jargon-heavy?
- Language warm and supportive where context demands it?
- Section headers descriptive without being verbose?

**Redundancy**
- Redundant labels, titles, or descriptions?
- Could any text be removed without losing meaning?
- Duplicate visual treatments saying the same thing?

### Lens 3: Interaction Consistency

- If icons are established in one area, are they carried through to related areas?
- Similar data shown in similar ways?
- If one table has dividers, do peer tables?
- How many implicit alignment rules? Could they be reduced?

### Lens 4: User Context

- Does the interface match the emotional context?
- Does the user know what to expect (time, effort, next steps)?
- Does this feel native to its platform?

## How to Frame Observations

Every observation has three parts:

1. **What you see** — Specific, concrete observation
2. **Why it matters** — Impact on user or perceived quality
3. **What it could be** — Specific, actionable alternative

**Good:** "The card shadows use a large blur radius creating a hazy look. Reducing blur to 8px with a tighter y-offset of 2px would create crisper depth."

**Bad:** "The shadows don't look good."

## Industry Standards

The apps people use daily — Instagram, Notion, Linear, iOS, Figma — form an invisible bar. If your interface doesn't meet it, people discount it immediately.

- Start with how iOS or shadcn+Tailwind would design it, then improve
- The industry standard is the **floor**, not the goal
- Family, Raycast, Linear — products that respect platform standards then exceed them

## Prioritizing Issues

After review, identify **top 3-5 opportunities** ranked by impact:
1. Issues that undermine trust or first impressions
2. Issues that create confusion or overwhelm
3. Issues that feel below industry standard
4. Polish opportunities that elevate from good to great

## Self-Critique

After building anything, run this framework on your own output before presenting. Ask: if someone with exceptional taste looked at this, what would they notice? Fix at least one thing before sharing.
