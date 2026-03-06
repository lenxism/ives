# Elements Deep Knowledge

## Input Field Details

### Placeholder contrast
The placeholder text contrast is contentious. WCAG AA requires 4.5:1, but that makes placeholders look pre-filled. AA-large (3:1) at 16px with a slightly heavier weight is a practical middle ground. Use hex #767676 as the lightest gray that passes AA on white backgrounds.

### Input sizing trick
Use half the input field height (e.g., 24px for a 48px input) as the size for checkboxes and radio buttons. Creates proportional harmony. Make the entire row (input field height) a tap target, not just the small checkbox.

### Float labels
Shopify's checkout uses float labels — the label starts as a placeholder inside the field, then animates above when focused. Great for space-constrained forms. Ensure the floated label maintains AA contrast.

### Prefixed inputs
For usernames (@), currency ($), URLs (https://), domains (.com) — show the prefix as read-only styled differently from the editable area. Clear delineation between input and decoration.

### Conditional inputs
When a toggle or checkbox reveals additional options, contain the parent and children in a shared background color to show the relationship visually.

## Form Patterns

### Progressive forms
For complex processes (signup, checkout, onboarding):
- Show one section at a time, not everything at once
- Collapse completed sections to reduce overwhelm
- Show progress (step 2 of 4) but don't make the total count demoralizing
- Validate inline when possible rather than on submit

### Mobile keyboard consideration
On mobile, the keyboard covers ~40% of the screen. Place the active input and its submit button above the keyboard. Auto-scroll to the focused field.

## List and Card Details

### List-to-detail transitions
- **Spotify:** Standard slide right to detail. Image gets larger, more metadata appears.
- **iOS Mail:** Standard slide. Preview text in list, full content in detail.
- **Facebook:** Full-width card → detail expands actions, shows comments.
- **App Store:** Card grows in place with spring animation. Beautiful for browsing.
- **Calcbot:** List modifies detail view in place — no transition, the list controls the detail.

### When to use which transition
- **Standard slide:** Most cases. Efficient, expected, zero friction.
- **Expanding card:** Exploratory browsing (app stores, media galleries).
- **Modal/sheet:** Focused tasks (compose, quick edit, filter).
- **In-place update:** Utility contexts (calculators, toolbars).

## Modal Nuances

### iOS permission pre-prompt
iOS only lets you request notification/location permission ONCE. If declined, the user must go to Settings manually. Solution: design a custom pre-prompt modal in your app's style first. "Would you like notifications?" → If yes, trigger the real iOS prompt. If "not now," you preserve your one chance.

### Action sheets vs alerts
- Alerts interrupt: "Are you sure?" — requires response before continuing
- Action sheets contextualize: "What do you want to do with this?" — options from a specific trigger
- Alerts should be rare. If users see too many "Are you sure?" dialogs, they start blindly confirming.

## Settings Page Patterns

Settings pages follow a consistent structure:
- Grouped sections with clear headers
- Toggle switches for on/off states
- Drill-down rows for sub-settings (right chevron indicates navigation)
- Value display on the right side of the row
- Destructive actions (logout, delete) at the bottom in red
- Search bar at top for large settings pages

## Profile Page Patterns

Profiles combine identity (avatar, name, bio) with actions and content:
- Large avatar, possibly editable
- Primary info (name, handle) with clear hierarchy
- Stats displayed horizontally (followers, posts, etc.)
- Primary action button (Edit Profile, Follow)
- Content tabs below (posts, media, likes)
- The profile header may shrink/collapse on scroll
