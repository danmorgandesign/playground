# Brand & Style Guidelines: Neo-Brutalist

## Aesthetic Identity
High-impact, disruptive web visual language. Rejects subtle gradients and soft shadows in favor of hard black strokes, deliberate offset drop-shadow blocks, raw primary colors, and high-energy contrast.

## Color System & Roles
- **Canvas (`surface`):** `#fef08a` — High-saturation Canary Yellow canvas.
- **Card Surface (`surface-container`):** `#ffffff` — Pure white container blocks.
- **Text & Stroke (`on-surface`):** `#000000` — Pure pitch black used for all typography, icons, and container borders.
- **Accent (`primary`):** `#ff66cc` — Neon Magenta for CTA buttons.
- **Accent Foreground (`on-primary`):** `#000000` — High-contrast black text on magenta.

## UI Rules
- **Borders:** Thick, hard `3px` solid black borders (`border-3 border-black`) on every container, card, and button.
- **Shadows:** Hard 2D offset box-shadows (`box-shadow: 4px 4px 0px #000000`). No blur radius allowed.
- **Interactions:** On button press/hover, translate the element diagonally (`transform: translate(2px, 2px)`) while collapsing the offset shadow.
