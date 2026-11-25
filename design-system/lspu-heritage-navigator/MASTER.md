# Design System Master File: GreenScape style

**Project:** LSPU Heritage Navigator · **Source:** the seven GreenScape reference screenshots (supersedes the earlier navy/gold Swiss design).

## Colour tokens


| Role                            | Hex                    | CSS variable               |
| ------------------------------- | ---------------------- | -------------------------- |
| Primary (buttons, links, icons) | `#4A7C2C`              | `--color-primary`          |
| Primary hover / link text       | `#3D6824`              | `--color-primary-dark`     |
| Forest (headings, footer)       | `#1A3D0F`              | `--forest`                 |
| Earth (secondary button)        | `#6B5744`              | `--earth`                  |
| Background (cream)              | `#F5F5F0`              | `--color-background`       |
| Badge / icon tint               | `#E8EDE0`              | `--tint`                   |
| CTA gradient                    | `#E9F5E9` to `#FDF7E7` | `--mint`, `--cream-warm`   |
| Body text                       | `#374151`              | &nbsp;                     |
| Muted text                      | `#4B5563`              | `--color-muted-foreground` |
| Footer text                     | `#D4E3C6`              | `--on-forest`              |
| Stars                           | `#FFB800`              | `--star`                   |


## Typography

Outfit (400, 500, 600, 700) is used throughout. Headings are 700 weight with tight tracking (−0.02em). Body text is 18px with 1.65 line height.

## Components

* **Header:** white with a soft shadow. Seal and wordmark, then links (green when active). No header button.
* **Buttons:** solid green, white outline (on photos), earth brown, and pill or XL pill for CTAs. 8px radius by default.
* **Badge:** a plain-text tinted pill above section headings. A glass version is used on photos.
* **Service card:** photo on top, bold title, muted text, and "Learn more →". 12px radius, lifts 6px on hover.
* **Testimonial card:** a round photo with a ring, a step label, an italic quote, a name and a green role. A thumbnail strip below has a green border on the selected item.
* **CTA band:** centred headline and an XL pill button.
* **Footer:** forest green with a wave pattern. Brand and email box, three link columns, a hairline divider and legal links.

## Motion and accessibility

Reveals use a 500ms fade with a 20px rise, staggered by 70ms (up to 8 items). Hovers take about 250ms. Pages fade in over 300ms. `prefers-reduced-motion` disables all of these. Text contrast is ≥4.5:1 everywhere, focus rings are visible (3px green, or gold on dark), and touch targets are at least 44px.

## Spacing

Text containers keep side margins of 48px on desktop, 32px at ≤1024px and 20px at ≤640px. Banner (hero) text stays inside the same container.

## Developers page

A 4-column grid (3 at ≤1024px, 2 at ≤768px) of cards: a square photo on top, then the name label and a role pill below. The Developer role uses a filled green pill and a green top border. Members use the tinted pill.