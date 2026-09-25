# Korongo — Design Notes

Source: [korongo.co.uk](https://korongo.co.uk/) (captured 2026-09-25)

Korongo is a no-jargon web design agency for startups, creatives, and small-to-medium
businesses. The design language is friendly, plain-spoken, and built around a "crane"
(korongo is Swahili for crane) — "so if you need a lift..." mascot/motif.

## Site structure

1. Header — logo + nav (`Home`, `Services`, `About`, `Contact`) + `Book a Call` button
2. Hero — logo, crane illustration/SVG, tagline, repeated `Book a Call` CTA
3. Three-part pitch, framed as questions:
   - **What?** — "Here at Korongo we offer tech support for small and medium sized
     businesses to develop their online presence. Whether just beginning or needing
     an update, Korongo provides jargon free advice and simple solutions for you."
   - **How?** — "After an initial conversation, we will lay out a clear pathway for
     getting you to where you want to be. You will be in the loop from day one
     ensuring that the end result is the online vision that you want to portray."
   - **Why?** — "We come from a diverse background and understand that sometimes we
     can't do everything and sometimes you need a lift. That's where Korongo can
     step in and help with some of the tech stuff in a simple, intuitive and
     problem solving kind of way."
4. CTA band — "Start Your Website Today / It only takes a friendly chat to begin
   your journey!" + `Book a Call` button (card-style section on a light grey surface)
5. Footer (orange background) — logo, "Important Stuff" (Privacy Policy), Company
   links (Services, About, Contact, Book a Call), social (Facebook, Instagram),
   copyright

## Color palette

Extracted from the site's CSS custom properties:

| Token | Value | Usage |
|---|---|---|
| `--theme-bg` | `#FFFFFF` | Page background |
| `--theme-on-bg` | `#000000` | Body text on white |
| `--theme-primary` | `#FF5B3E` | Brand accent (coral/orange) — footer background, primary actions |
| `--theme-primary-hover` | `hsl(0, 0%, 20%)` (~`#333333`) | Hover state for primary elements |
| `--theme-on-primary` | `#1A1A1A` | Text/icons on the orange primary surface |
| `--theme-surface-1` | `#F2F2F2` | Light grey section background (e.g. CTA card) |
| `--theme-on-surface-1` | `#000000` | Text on surface-1 |
| `--theme-surface-2` | `#FFD84D` | Secondary accent (yellow) |
| `--theme-on-surface-2` | `#000000` | Text on surface-2 |

**Palette mood:** warm, high-contrast, playful — punchy coral/orange as the brand
color, yellow as a secondary accent, everything else kept to black/white/light grey
so the two accent colors do the work.

## Typography

- **Sans (body / UI):** `"Supreme", -apple-system, BlinkMacSystemFont, sans-serif`
- **Display (headings):** `"Khand", -apple-system, BlinkMacSystemFont, sans-serif`
  — Khand is a condensed, geometric display sans, loaded via Google Fonts
  (`weights: 400, 500, 600, 700`)

**Fluid type scale** (CSS `clamp()`, scales between mobile and desktop viewport):

| Token | Range |
|---|---|
| `--font-size-sm` | 14.4px → 15px |
| `--font-size-base` | 18px → 20px |
| `--font-size-md` | 22.5px → 26.66px |
| `--font-size-lg` | 28.13px → 35.54px |
| `--font-size-xl` | 35.16px → 47.37px |
| `--font-size-xxl` | 43.95px → 63.15px |
| `--font-size-xxxl` | 54.93px → 84.17px |

Line height: `1.5` on `html`/`body`.

## Layout & spacing

- `--container-max-width`: `1440px`
- `--container-max-width-narrow`: `960px`
- `--container-padding`: `0 1rem`
- `--section-margin`: `7.5rem` (generous vertical rhythm between sections)
- `--theme-blog-post-header-width`: `1200px`
- Multi-column text sections use a responsive column grid: 3 columns on desktop,
  2 columns on tablet, collapsing to 1 column at the `768px` breakpoint.

## Shape & motion

- `--theme-button-border-radius`: `3rem` — fully pill-shaped buttons
- `--theme-shape-radius`: `clamp(1rem, 2rem, 3rem)` — large, soft rounding on
  cards/sections
- `--theme-transition`: `.2s ease-in-out` — standard hover/interaction timing

## Imagery

Custom SVG illustration of a crane (the "Korongo" mascot), used in the hero.
Otherwise the page is largely typographic — no photography, leaning on color,
whitespace, and the crane motif to carry brand personality.

## Voice & tone

Conversational, first-name-friendly copy that avoids jargon by design ("jargon
free advice and simple solutions"). Short sentences, direct address ("you"),
consistent single CTA throughout: **Book a Call**.

## Takeaways for reuse

- Two-accent-color system (coral `#FF5B3E` + yellow `#FFD84D`) on a neutral
  black/white/light-grey base reads as friendly and modern without needing a
  large palette.
- Pairing a condensed display font (Khand) for headings against a plain
  geometric sans (Supreme) for body text gives headings punch while keeping
  body copy easy to read.
- Pill buttons (`3rem` radius) + soft, large corner radii on cards reinforce the
  "friendly, approachable" brand feel.
- One repeated, unambiguous CTA ("Book a Call") throughout the page rather than
  competing calls to action.
