# Color Deep Knowledge

## Gray Analysis: Real-World Examples

### Twitter (Good)
Five grays total: brand blue, dark text, medium gray for metadata/icons, light gray for dividers, lighter gray for section backgrounds. All hues within 208-210 range (cool blue family). Saturation and brightness vary to create hierarchy, but the consistent hue creates cohesion.

Key insight: the large divider block and thin divider line use the exact same hex code — the block looks darker only because there's more of it. Same color, different perception based on area.

### Pinterest (Excellent)
Only THREE grays: dark text (#333), medium gray for icons/secondary nav, and a lighter gray for backgrounds and metadata. Nearly everything is accomplished with these three values. Warm, desaturated grays complement the red brand color.

One concern: their lightest gray (8E8E) doesn't pass AA contrast at small sizes (3.28 ratio). They could add one more mid-gray between their medium and light values.

### Gmail (Cautionary)
A chaotic mix of warm and cool grays. Some at hue 0 (pure neutral), some at 180 (teal), some at 200+ (blue). The inconsistency creates a subtle but pervasive sense of visual discomfort. The inbox area uses warm gray text on a cool gray background — an odd pairing.

Likely caused by multiple teams working on different features over many years without a unified gray system. This is what happens when you don't define your grays upfront.

### Facebook
Slightly muted palette (no pure white background). Uses border + same background color to create visual separation — one color serves double duty. All grays sit in the same hue family as their brand blue.

## Dark UI Techniques

### The hex code technique
For dark UI grays, try removing green from balanced hex values:
- Balanced (desaturated): `#161616`, `#494949`
- With character (remove green): `#161416`, `#494749`

This creates a subtle purple-warm quality that's richer than flat gray. The resulting HSB values land around hue 300 (purple range).

### Dark UI workflow
1. Design typography and layout first in light mode or neutral gray
2. Get spacing, hierarchy, and content right
3. THEN apply dark color treatment
4. Fine-tune borders, dividers, and shadows (they need to be much more subtle)

### Common dark UI mistakes
- Pure black backgrounds (use dark charcoal with slight hue instead)
- Too much saturation (Twitter's "Dim" mode has overly saturated blues)
- Full white text (use off-white, ~95% brightness with slight hue tint)
- Visible borders that were fine in light mode but scream in dark mode
- Not adjusting shadow strategy (shadows barely work on dark backgrounds — use lighter borders or subtle glow instead)

### The OLED exception
Pure black (#000000) works on OLED displays because pixels physically turn off, blending with the device bezel. But even on OLED, content cards and sections should use dark grays, not pure black — you need layers of depth.

## Near-White Techniques

Pure white (#FFF) should be reserved for primary content areas. Use near-whites for:
- Page backgrounds: #FAFAFA, #F8F8F8, #F5F5F5
- Card backgrounds on gray pages: #FFFFFF (white pops against near-white)
- Hover states: 2-3% darker than the base
- Alternating table rows: 1-2% difference is sufficient

The interplay between white and near-white creates subtle depth without shadows or borders.
