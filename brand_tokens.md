# MUSU Brand Tokens

## Purpose

Use these tokens as the single source of truth for the MUSU landing page.
They translate the brand colour and typography guidance into implementation-ready values for HTML and CSS.

These tokens are intended for a static, minimal landing page for **musuwrap.com**.
The design should feel calm, spacious, poetic, and restrained.

---

## Brand Principles

- Quiet, minimal, editorial
- Museum-like whitespace
- No marketing hype
- No gradients
- No clutter
- Refined serif-led typography
- Soft contrast, not harsh black-and-white

---

## Colour Tokens

### Core Palette

| Token | Value | Use |
|---|---:|---|
| `--color-bg` | `#FFFFFC` | Main page background |
| `--color-heading` | `#000A02` | Logo, main heading, strongest text |
| `--color-body` | `#373C38` | Body copy, supporting text |
| `--color-line` | `#E5E2E4` | Hairlines, dividers, subtle secondary details |

### Colour Notes

- Default page background should be `--color-bg`
- Headings should usually use `--color-heading`
- Body copy should usually use `--color-body`
- Dividers and fine illustration details may use `--color-line`
- Do not introduce bright accent colours
- Do not use gradients or tinted overlays
- Prefer the specified near-black over pure black

---

## Typography Tokens

### Brand Type Roles

| Token | Suggested Value | Intended Use |
|---|---:|---|
| `--font-display` | `"Spectral", "Iowan Old Style", "Palatino Linotype", "Book Antiqua", Georgia, serif` | Logo and display text |
| `--font-body` | `"EB Garamond", Garamond, Baskerville, "Times New Roman", serif` | Body copy and supporting text |

### Japanese Type Roles

| Token | Value | Use |
|---|---:|---|
| `--font-jp` | `"Shippori Mincho", "Hiragino Mincho ProN", "Hiragino Mincho Pro", "MS PMincho", "Yu Mincho", serif` | Japanese text (all Japanese characters) |
| `--fs-jp` | `20px` | Default size for Japanese text |

### Type Scale

| Token | Value | Use |
|---|---:|---|
| `--fs-logo` | `42px` | MUSU wordmark / primary display |
| `--fs-h1` | `26px` | Main heading |
| `--fs-subhead` | `16px` | Short supporting serif line |
| `--fs-body` | `12.8px` | Body copy |

### Line Height

| Token | Value | Use |
|---|---:|---|
| `--lh-body` | `16.2px` | Body copy line height |
| `--lh-relaxed` | `1.6` | General fallback readable rhythm |
| `--lh-tight` | `1.2` | Headlines and short display lines |

### Letter Spacing

| Token | Value | Use |
|---|---:|---|
| `--ls-logo` | `0.20em` | MUSU wordmark |
| `--ls-h1` | `0.12em` | Main heading |
| `--ls-subhead` | `0.03em` | Supporting serif line |
| `--ls-body` | `0.02em` | Body copy |

### Typography Notes

- Use **Spectral Medium** for logo and main heading when self-hosted or available locally
- Use **Spectral Regular** for supporting serif lines when available
- Use **EB Garamond Regular** for body copy when available
- All Japanese characters should use **Shippori Mincho Regular** at **20px**
- Japanese text used as a headline or sub-headline should display **vertically**
- Japanese text used in body copy should display **horizontally**
- Do **not** load fonts from external services
- If the brand fonts are not bundled locally, use the fallback serif stacks above
- Do not substitute with trendy sans-serif fonts unless explicitly required

---

## Spacing Tokens

Use spacious vertical rhythm.
The page should breathe.

| Token | Value | Use |
|---|---:|---|
| `--space-1` | `0.25rem` | Micro spacing |
| `--space-2` | `0.5rem` | Tight spacing |
| `--space-3` | `0.75rem` | Small spacing |
| `--space-4` | `1rem` | Base spacing |
| `--space-5` | `1.5rem` | Comfortable spacing |
| `--space-6` | `2rem` | Large spacing |
| `--space-7` | `3rem` | Section spacing |
| `--space-8` | `4.5rem` | Generous vertical spacing |
| `--space-9` | `6rem` | Hero whitespace |

### Spacing Notes

- Prefer more space rather than more elements
- Keep text blocks compact, but separate them with generous vertical rhythm
- Avoid dense clusters of UI elements

---

## Layout Tokens

| Token | Value | Use |
|---|---:|---|
| `--page-max-width` | `1200px` | Overall page container |
| `--content-max-width` | `32rem` | Narrow text column |
| `--content-padding-x` | `1.5rem` | Mobile side padding |
| `--content-padding-y` | `3rem` | Mobile vertical padding |
| `--content-padding-y-lg` | `6rem` | Larger-screen vertical padding |

### Layout Notes

- Use a narrow content width for the main message
- Centered layout is preferred for the first version
- The page should feel closer to an invitation card than a product launch page

---

## Border and Surface Tokens

| Token | Value | Use |
|---|---:|---|
| `--border-subtle` | `1px solid #E5E2E4` | Hairline divider |
| `--radius-none` | `0` | Default corners |
| `--shadow-none` | `none` | No card shadows |

### Surface Notes

- Avoid cards unless explicitly requested
- Avoid heavy containers and boxed sections
- Let whitespace define structure

---

## Motion Tokens

For the landing page, motion should be absent or nearly absent.

| Token | Value | Use |
|---|---:|---|
| `--transition-soft` | `150ms ease` | Very subtle hover/focus transitions only |

### Motion Notes

- No decorative animation
- No parallax
- No auto-rotating elements
- No animated marketing effects

---

## Content Tokens

These are the approved core content lines for the initial landing page.

| Token | Value |
|---|---|
| `brand.name` | `MUSU` |
| `brand.jp` | `風呂敷` |
| `brand.tagline` | `Wrap once. Gift twice.` |
| `brand.status` | `Launching soon.` |
| `brand.origin` | `Authentic and made in Japan.` |

### Optional Supporting Copy

Use sparingly. One short supporting sentence is enough.

Approved direction:
- `A furoshiki is a traditional Japanese wrapping cloth.`
- `A quiet ritual of giving.`
- `The wrapping is part of the gift.`
- `Authentic and made in Japan.`

Avoid adding further marketing copy unless explicitly requested.

---

## CSS Starter Example

```css
:root {
  --color-bg: #FFFFFC;
  --color-heading: #000A02;
  --color-body: #373C38;
  --color-line: #E5E2E4;

  --font-display: "Spectral", "Iowan Old Style", "Palatino Linotype", "Book Antiqua", Georgia, serif;
  --font-body: "EB Garamond", Garamond, Baskerville, "Times New Roman", serif;

  --fs-logo: 42px;
  --fs-h1: 26px;
  --fs-subhead: 16px;
  --fs-body: 12.8px;

  --lh-body: 16.2px;
  --lh-relaxed: 1.6;
  --lh-tight: 1.2;

  --ls-logo: 0.20em;
  --ls-h1: 0.12em;
  --ls-subhead: 0.03em;
  --ls-body: 0.02em;

  --space-1: 0.25rem;
  --space-2: 0.5rem;
  --space-3: 0.75rem;
  --space-4: 1rem;
  --space-5: 1.5rem;
  --space-6: 2rem;
  --space-7: 3rem;
  --space-8: 4.5rem;
  --space-9: 6rem;

  --page-max-width: 1200px;
  --content-max-width: 32rem;
  --content-padding-x: 1.5rem;
  --content-padding-y: 3rem;
  --content-padding-y-lg: 6rem;

  --border-subtle: 1px solid #E5E2E4;
  --radius-none: 0;
  --shadow-none: none;

  --transition-soft: 150ms ease;
}
```

---

## Final Direction

When implementing the page:

- reduce before adding
- shorten before explaining
- leave space before introducing structure
- choose restraint over decoration

If a design choice makes the page feel like a generic startup teaser, simplify it.
