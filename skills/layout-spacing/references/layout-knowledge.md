# Layout Deep Knowledge

## Implicit Grid

Rather than adhering to a rigid column grid, establish implicit alignment edges that emerge from your content. Key technique: when you place a title at 20px from the left edge, child elements indented to 40px create a clear parent-child relationship without explicit visual separators.

Example from a camera product form: "Choose your sensor" at the left margin, with selectable options indented 20px creates unmistakable ownership without varying type size. The alignment alone communicates the relationship.

## Alignment as Concept

Alignment can reinforce design direction:
- Hard left/right edges feel bold, decisive, technical (matches blocky product design)
- Centered layouts feel calm, balanced, approachable
- Asymmetric layouts feel dynamic, editorial, contemporary

Choose alignment strategy based on the emotional direction, not just convention.

## Forms and Alignment

Forms need especially careful left-edge alignment:
- All labels left-aligned to the same edge
- Input fields aligned to the same left edge (or intentionally indented from labels)
- Buttons can align left (technical, direct) or full-width (mobile, emphasis)
- Checkboxes/radios indented from their parent creates clear ownership
- Error messages aligned with the input they reference

## Interactive Layouts

When designing layouts with scrollable lists, card grids, or feeds:
- Full-width cards maximize screen real estate on mobile
- Cards with padding create clear separation but use more space
- List items with consistent height create scannable rhythm
- Consider what happens when content length varies — test with long and short content

## Responsive Considerations

- Start mobile-first, then adapt to larger screens
- Don't just stretch — reconsider information density at each breakpoint
- Sidebar navigation appears at wider breakpoints; tab bar on mobile
- Card grids reflow: 1 column → 2 → 3 → 4 as width increases
- Maintain proportional spacing — don't let fixed margins create cramped layouts on small screens
