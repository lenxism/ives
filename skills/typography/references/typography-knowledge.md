# Typography Deep Knowledge

Detailed analysis and examples for the typography skill.

## Table of Contents
- Real-world type size analysis
- Font weight patterns
- Combining text styles
- Callouts and definitions
- Interactive text patterns
- Alternate font guidance

## Real-World Type Size Analysis

### Instagram
The entire home screen uses one type size (15pt) for everything: titles, descriptions, usernames, likes, comments. The only variation is 12pt under stories. Differentiation comes purely from weight and color.

### Twitter/X
Three type sizes for the entire timeline:
- 17pt heavy for display name
- 16pt in bold, medium, and regular for username, timestamp, tweet body, interaction labels
- A slightly smaller size for engagement counts

Three different styles at 16pt (bold dark name, regular gray username, regular dark body) create clear hierarchy without adding sizes.

### iOS Settings
Internal pages often use just TWO sizes:
- 17pt for the back button, page title, list items, and definition values
- A smaller metadata size for helper text and section headers (in all caps)

Same 17pt serves as title, list item, and value — distinguished by weight, color, and position.

### Facebook Messenger (main screen)
Three sizes only: large title, search/list items, and smaller metadata for stories and timestamps.

### Facebook Discover (cautionary example)
Five to six different type sizes create a scattered, unfocused feel. The page lacks cohesion primarily because of excessive type size variation. Tabs in all caps at one size, titles at another, "See more" at yet another, metadata at another. The sheer number of sizes is the biggest visual culprit.

## Font Weight Patterns

### Instagram's subtle weight system
Instagram uses incredibly subtle weight changes to indicate actionable profile names versus body text. Hashtags and mentions use color (blue) instead of weight because they're user-generated input, distinct from the Instagram design system.

### iOS Settings weight + color system
Title (bold, dark) and action link (regular, blue) share the exact same size. Meaning changes entirely through weight and color. Definition values on the right side are same size, lighter color, right-aligned — three properties (weight, color, position) create completely different meaning at identical sizes.

## Combining Text Styles

When you need variety without more sizes:
1. Weight changes (bold vs regular vs medium)
2. Color changes (dark vs gray vs blue vs red)
3. Position changes (left vs right aligned, inline vs stacked)
4. Case changes (sentence case vs ALL CAPS)
5. Decoration (underline, background pill, strikethrough)

These five modifiers on 3-4 base sizes give you 20+ distinct text styles — more than enough for any interface.

## Callout Patterns

Callouts (alerts, notices, tips) should:
- Use the same base type sizes as the rest of the interface
- Differentiate through background color, left border, or icon — not type size
- Keep callout body text at the same size as regular body text
- Use weight (bold/semibold) for the callout title, not a larger size

## Interactive Text

Text that invites interaction (links, buttons, tappable labels):
- On mobile, there is no hover state — interactive text must be discoverable through color, weight, or decoration alone
- Blue is the universal "this is tappable" color, but brand colors work if consistent
- Underlines are strong affordances on web; less common on mobile
- Ensure tappable text areas have generous hit targets (minimum 44pt on mobile)

## Alternate Font Guidance

When choosing a non-system font:
- Test it on numbers. Odd number forms (unusual 4s, 6s, 9s) can undermine an otherwise good choice.
- Check it at the sizes you'll actually use (15-17pt body, not just large display)
- Verify weight availability — you need at least regular, medium, and bold
- Consider loading performance on web — each weight is additional download
- One custom display font + system body font is often the ideal balance

Custom fonts for app-based interfaces are trickier than web because the system font is so deeply ingrained in the platform experience. Web has more room for typographic expression.
