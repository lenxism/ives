---
name: imagery
description: >
  Guide for using imagery in interfaces — photos (static and dynamic), icons, illustrations,
  and app icons. Covers photo selection, dynamic image handling, icon design and usage,
  creating simple illustrations, and app icon design. Use when working with images, icons,
  illustrations, or any visual assets in an interface. Trigger on: image, photo, icon, icons,
  illustration, avatar, thumbnail, app icon, stock photo, imagery, visual assets, favicon.
---

# Imagery

Imagery has a massive impact on aesthetics, mood, and perceived quality. Whatever kind you use — photos, icons, illustrations — they must match the overall direction.

## Static Photos

Photos you control (stock, curated, photo shoots):
- **Avoid cliché stock** — Happy salad-eating people, businessmen jumping with briefcases. These trigger negative emotions. Search for authentic, candid, moody imagery.
- **Consistency** — All photos in a set should have similar treatment (color temperature, exposure, style).
- **Quality** — A mediocre photo undermines an otherwise excellent interface. Better to use no photo than a bad one.

## Dynamic Images

User-generated content (avatars, posts, uploads) that you can't predict:
- Design for the worst case — screenshots, dark photos, text-heavy images
- Use consistent aspect ratios and cropping
- Avatar fallbacks: initials or generic icon, never a broken image
- Consider how a grid of random images looks together, not just individually

## Icons

### Using existing icons
- Choose ONE icon set and stick with it (Feather, Lucide, SF Symbols, Phosphor)
- Never mix icon sets — inconsistent stroke widths and styles are immediately noticeable
- All outline OR all filled, not mixed
- Consistent size: common sizes are 20px, 24px, or 28px. Pick one for each context.
- Icon color should come from your gray system, not arbitrary values

### Creating icons
- Start with a consistent grid (24×24 or 32×32)
- Uniform stroke width (typically 1.5-2px)
- Consistent corner radius on line caps and joins
- Optical alignment — visually center within the grid, not mathematically
- Test at actual size, not just zoomed in

### When icons become illustrations
Icons are small, symbolic, single-purpose. Illustrations are larger, environmental, mood-setting. The transition is about complexity and context size. If it needs a scene or environment, it's an illustration.

## Simple Illustrations

You can create effective illustrations with basic shapes in any design tool:
- Rounded rectangles with gradients for objects
- Circles with linear gradients for lighting
- Drop shadows for grounding
- Layer opacity for depth
- Noise texture overlay (3-5% opacity) for character

## App Icons

If designing a mobile/desktop app:
- Design the app icon LAST — after you know your interface colors, iconography style, and visual language
- Start at 1024×1024, then scale down and adjust details for smaller sizes
- Simplicity wins — a clear symbol beats a cramped wordmark
- Test in context: screenshot your home screen and place the icon among real apps
- Consult platform guidelines (Apple HIG, Material) for required sizes and safe areas
- On very small sizes, you may need to manually simplify details that get lost
