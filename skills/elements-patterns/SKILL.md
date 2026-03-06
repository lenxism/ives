---
name: elements-patterns
description: >
  Practical guide for designing common UI elements and patterns. Covers navigation, input
  fields, forms, profiles, settings, lists and cards, detail views, sort and filter, tables,
  modals, and design systems. Use when designing any standard UI element or pattern. Trigger
  on: navigation, nav, input field, form, login, signup, profile, settings, list, card, table,
  modal, dialog, dropdown, checkbox, radio, toggle, tabs, search, filter, sort, detail view,
  pagination, design system, component.
---

# Elements & Patterns

Every element is a stepping stone in the user's journey from point A to point B. Design each one through the lens of that experience.

Read `references/elements-knowledge.md` for detailed guidance on specific element types.

## Universal Principles

### Start with platform defaults
Before designing any element from scratch, look at how iOS (HIG) or the web (shadcn/Tailwind) handles it. Match the convention, then exceed it.

### Consistency over creativity
A consistent set of "good" components beats a mix of some "great" and some "mediocre." Every element should feel like it belongs to the same family.

### State coverage
Every interactive element needs ALL states designed:
- Default, Hover, Focused/Active, Disabled, Error, Success, Loading
- Empty states for lists, search results, data views
- Skeleton/loading states for async content

Missing states is the fastest way to look amateur.

## Navigation

- **Mobile:** Bottom tab bar for 3-5 primary destinations. More than 5? Reconsider information architecture.
- **Web app:** Sidebar for apps (collapsible), top bar for marketing sites.
- Highlight the active state clearly — color, weight, or indicator mark.
- Secondary navigation (settings, profile) can live in header icons rather than tabs.
- Test navigation labels at realistic lengths — "Activity" fits, "Transaction History" might not.

## Input Fields

The mighty input needs extensive design work:
- **Label:** Top-aligned, 8px gap to field, same or slightly smaller size as input text
- **Placeholder:** AA-large contrast (3:1) minimum — dark enough to read, light enough to not look pre-filled
- **Focus state:** Unmistakable. 2px colored border is the standard.
- **Error state:** Red border + icon + message. Color alone isn't accessible.
- **Helper text:** Below the field, 2pt smaller than input text, AA contrast
- **Sizing:** Match field width to expected content. Zip code doesn't need a full-width field.

### Input variants to design
Default, hover, focused, filled, error, success, disabled, password (with show/hide), multiline, dropdown, prefixed, character count, checkboxes, radio buttons, toggles.

## Lists and Cards

**Lists:** Best for scannable, text-heavy content. Consistent row height creates rhythm. Consider avatars, metadata, and right-side accessories.

**Cards:** Best for visual content, browsable collections. Consistent aspect ratios. Consider how they reflow at different screen sizes.

**The key question:** Does the user need to scan quickly (list) or browse visually (cards)?

## Detail Views

Every list/card links to a detail view. Design the transition intentionally:
- **Standard slide:** Simple, expected, efficient for most cases
- **Expanding card:** Fun, exploratory (App Store pattern) — only for browsing contexts
- **Modal/sheet:** For focused tasks that shouldn't lose parent context

On the detail view: expand what was truncated, add secondary information, provide actions that don't belong on the list view.

## Modals

Modals are conversations — small, contained interruptions:
1. **Clear title** that states what will happen
2. **Concise body** providing context
3. **Primary action** that answers the title's question
4. **Secondary action** (cancel) for a clear escape
5. **Overlay** keeping parent visible but inaccessible

**Copy is critical:** "Delete this video?" → "Yes, delete" / "Cancel" — never ambiguous. If the button labels could be confusing ("Cancel" on a cancellation dialog), rewrite them.

### Modal types
- **Alert:** Demands attention before continuing (delete confirmation, low battery)
- **Action sheet:** Contextual actions from a specific trigger (share, export options)
- **Popover:** Small contextual panel near its trigger (formatting options, date picker)
- **Interstitial:** Full-screen bridge between flows (check your email, onboarding step)

## Tables

- Summary altitude: 3-4 columns maximum. Details belong in detail view.
- Sort indicators should be subtle but clear.
- Use `tabular-nums` for all number columns.
- Alternating row backgrounds: 1-2% contrast difference is sufficient.
- Header text: lighter weight or smaller size than body rows.

## Design Systems

When you've designed enough individual elements, systematize:
- Document every component with all states
- Establish naming conventions
- Define spacing tokens, color tokens, type tokens
- Make components composable — inputs that work inside cards inside modals
- The system should make the next page faster to design, not slower
