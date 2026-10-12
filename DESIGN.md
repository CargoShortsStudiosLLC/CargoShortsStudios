---
name: Cargo Shorts Studios
description: Quiet umbrella site for a small Minnesota studio's tabletop and card game apps.
colors:
  rust-thread: "#9a4318"
  rust-thread-dark: "#e08a5c"
  charcoal-twill: "#1c1b19"
  bone-canvas: "#ece8df"
  faded-denim-grey: "#5f5a52"
  faded-denim-grey-dark: "#a39b8c"
  seam-line: "#d9d4ca"
  seam-line-dark: "#3a3833"
  pocket-lining: "#f3f1ec"
  pocket-lining-dark: "#262521"
  paper-white: "#ffffff"
  cargo-khaki: "#c2a878"
typography:
  display:
    fontFamily: "Roboto, -apple-system, BlinkMacSystemFont, Segoe UI, sans-serif"
    fontSize: "2rem"
    fontWeight: 700
    lineHeight: 1.2
    letterSpacing: "-0.015em"
  headline:
    fontFamily: "Roboto, -apple-system, BlinkMacSystemFont, Segoe UI, sans-serif"
    fontSize: "1.15rem"
    fontWeight: 700
    lineHeight: 1.6
  title:
    fontFamily: "Roboto, -apple-system, BlinkMacSystemFont, Segoe UI, sans-serif"
    fontSize: "1.15rem"
    fontWeight: 500
    lineHeight: 1.6
  body:
    fontFamily: "Roboto, -apple-system, BlinkMacSystemFont, Segoe UI, sans-serif"
    fontSize: "16px"
    fontWeight: 400
    lineHeight: 1.6
  label:
    fontFamily: "Roboto, -apple-system, BlinkMacSystemFont, Segoe UI, sans-serif"
    fontSize: "0.95rem"
    fontWeight: 500
    lineHeight: 1.6
  caption:
    fontFamily: "Roboto, -apple-system, BlinkMacSystemFont, Segoe UI, sans-serif"
    fontSize: "0.85rem"
    fontWeight: 400
    lineHeight: 1.6
rounded:
  none: "0"
  screenshot: "8px"
  icon-sm: "12px"
  icon-md: "14px"
spacing:
  xxs: "4px"
  xs: "6px"
  sm: "8px"
  md: "12px"
  base: "16px"
  row: "18px"
  lg: "24px"
  xl: "32px"
  xxl: "40px"
  xxxl: "56px"
components:
  site-header:
    backgroundColor: "{colors.paper-white}"
    textColor: "{colors.charcoal-twill}"
    typography: "{typography.body}"
    height: "52px"
    padding: "10px 16px"
  nav-link:
    textColor: "{colors.faded-denim-grey}"
    typography: "{typography.label}"
  nav-link-active:
    textColor: "{colors.charcoal-twill}"
  text-link:
    textColor: "{colors.rust-thread}"
  sheet-label:
    textColor: "{colors.faded-denim-grey}"
    typography: "{typography.label}"
    width: "172px"
    padding: "18px 32px 18px 0"
  sheet-value:
    textColor: "{colors.charcoal-twill}"
    typography: "{typography.body}"
    padding: "18px 0"
  app-icon:
    rounded: "{rounded.icon-md}"
    size: "64px"
  app-icon-title:
    rounded: "{rounded.icon-sm}"
    size: "56px"
  screenshot-thumb:
    rounded: "{rounded.screenshot}"
    width: "120px"
  store-badge-appstore:
    rounded: "{rounded.none}"
    width: "120px"
    height: "40px"
  table-header-cell:
    textColor: "{colors.faded-denim-grey}"
    typography: "{typography.caption}"
    padding: "8px 12px 8px 0"
  legal-table-header-cell:
    backgroundColor: "{colors.pocket-lining}"
    textColor: "{colors.charcoal-twill}"
    padding: "8px 10px"
  footer:
    textColor: "{colors.faded-denim-grey}"
    typography: "{typography.caption}"
    padding: "16px"
---

# Design System: Cargo Shorts Studios

## Overview

**Creative North Star: "The Pocket Ledger"**

The site is a ledger kept in a cargo pocket: compact, ruled, practical, with everything filed where you'd expect it. Every page is a single 720px column of hairline-ruled rows. A narrow muted label sits on the left and the facts sit on the right, the way you'd jot an inventory in a pocket notebook. Nothing floats, glows or lifts off the page. Structure comes from the ruling lines and the label column, never from boxes.

The personality comes in two ways only: the **copy** ("Hot singles in your commander deck?") and the **app art** (icons, screenshots, store badges). The UI chrome stays plain and workmanlike: text links, warm greys, one rust accent. That's the wink. A utilitarian frame that takes itself seriously holds a joke that doesn't. Light and dark modes are equal citizens and follow the system setting. Both are warm (bone and charcoal, never blue-grey).

The system rejects three things outright. **SaaS landing tropes**: hero gradients, oversized CTA buttons, feature-card grids, testimonial carousels. **Fantasy/MTG pastiche**: parchment textures, mana-symbol ornament, gilded frames. **Elevated cards and drop shadows.**

**Key Characteristics:**
- One centered 720px column; density over spectacle.
- The **sheet**, a 172px muted label column beside wide content, separated by 1px hairlines, is the signature pattern on every non-legal page.
- A single warm accent (rust) used only for links. The logo's khaki stays inside the logo.
- One typeface (Roboto) in three weights: 400, 500 and 700.
- Completely flat. Depth is only ever a hairline rule.
- App icons, screenshots and official store badges are the only color-rich elements.

## Colors

A warm, low-chroma workwear palette (charcoal twill, bone canvas, faded denim, seam thread), with one rust accent stitched through it. Every color has a light and dark pair, swapped wholesale under `prefers-color-scheme: dark` via CSS custom properties (`--bg`, `--fg`, `--muted`, `--rule`, `--link`, `--code-bg`) in `style.css`.

### Primary
- **Rust Thread** (light `rust-thread`, dark `rust-thread-dark`): the only accent in the UI. It's used for in-content links (`--link`) and nothing else. No button fills, no headline color, no background tints. The dark variant is lifted and softened so it reads on charcoal.

### Neutral
- **Charcoal Twill** (`charcoal-twill`): body text in light mode (`--fg`), page background in dark mode (`--bg`). It's also the stroke color in the logo artwork.
- **Bone Canvas** (`bone-canvas`): body text in dark mode. It's a warm off-white, never pure white on charcoal.
- **Paper White** (`paper-white`): page background in light mode.
- **Faded Denim Grey** (light `faded-denim-grey`, dark `faded-denim-grey-dark`): secondary text (`--muted`). Used for sheet labels, ledes, meta lines, nav links at rest, table headers, fine print and the footer.
- **Seam Line** (light `seam-line`, dark `seam-line-dark`): every hairline (`--rule`): header and footer borders, sheet row dividers, table rows, legal section dividers.
- **Pocket Lining** (light `pocket-lining`, dark `pocket-lining-dark`): the only tinted surface (`--code-bg`). Used for legal-document table header cells.

### Brand asset (not a UI color)
- **Cargo Khaki** (`cargo-khaki`): the shorts fabric in `assets/logo.svg` and `assets/icon.svg`. It's recorded here so the logo is never recolored, but it is **not** a UI token.

### Named Rules
**The One Thread Rule.** Rust is the only accent, and it only marks links. If something rust-colored isn't clickable, it's wrong.

**The Khaki-Stays-in-the-Pocket Rule.** Cargo Khaki lives inside the logo SVGs. It never becomes a background, border, button, highlight or focus color.

**The Warm Greys Rule.** Every neutral leans warm (hue ~80–90°, low chroma). Never introduce cool or blue-grey neutrals, in either theme.

## Typography

**Display Font:** Roboto (with -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif)
**Body Font:** Roboto (same stack)

**Character:** A single workhorse sans in three weights, loaded from Google Fonts (400, 500, 700, and 400 italic). Plain enough to disappear, so the copy does the talking. Hierarchy comes from weight and the muted color, not from size jumps. The whole scale spans just 0.85rem to 2rem.

### Hierarchy
- **Display** (700, 2rem, 1.2, -0.015em tracking): one `h1` per page, the page or app name. On app pages it sits in a title row beside the 56px app icon.
- **Headline** (700, 1.15rem): generic `h2` section heads outside the sheet. In legal documents it grows to 1.2rem with a hairline and 24px padding above.
- **Title** (500, 1.15rem): app names inside an app row (`h3`).
- **Body** (400, 16px, 1.6): all running text; the 720px column keeps lines near 75ch. Legal articles loosen to 1.65 line-height.
- **Label** (500, 0.95rem, Faded Denim Grey): sheet row labels (which are `h2` elements restyled), and nav links.
- **Caption** (400–500, 0.85rem–0.9rem, Faded Denim Grey): table headers, fine print, footer, breadcrumbs, document meta lines.

### Named Rules
**The Three Weights Rule.** Roboto 400, 500 and 700 only. No light weights, no black weights, no second typeface.

**The Muted-Not-Smaller Rule.** Secondary information gets demoted by Faded Denim Grey first and size second. Labels stay near body size (0.95rem) so they're still readable on a phone.

## Layout

A single centered column: `max-width: 720px`, 16px side gutters, full-width at phone size. The page is a vertical flex stack (header, `main` that grows to fill, footer), so the footer always sits at the bottom on short pages. `main` has 40px top and 56px bottom padding.

The **sheet** is the core layout primitive: a two-column CSS grid (`172px 1fr`) with a hairline above the first row and below every row. Each row has 18px of vertical padding, and the label column has 32px of right padding. At **≤600px** the sheet collapses to one column, and each label stacks above its content with no divider between them. At **≤480px** the nav gap tightens from 20px to 14px, and legal tables scroll horizontally instead of squeezing.

Spacing follows a loose 4/8 rhythm: 4–8px inside clusters (badges, link rows), 12–18px between items in a row, 24–40px between blocks, 56px before the footer. Inline clusters (store badges, link lists, footer nav, screenshots) all use `flex-wrap` with a smaller row gap than column gap, so they reflow to a phone without media queries.

## Elevation & Depth

The system is completely flat. There are no `box-shadow`s, no layered surfaces, no blur, and no z-stacking. Depth is only ever expressed through **1px Seam Line hairlines**: under the header, above the footer, between sheet rows, between table rows, and above legal sections. The one tonal surface is Pocket Lining, used only for legal table header cells.

### Named Rules
**The Ruled-Not-Raised Rule.** If a group needs separating, draw a hairline. Never a box, never a shadow, never a background card.

## Shapes

The UI chrome is square-edged. Hairlines run edge to edge and nothing in the layout is rounded. Rounding is reserved for **imagery**, so it echoes the shape the image has on a device:

- App icons get iOS-style rounding at roughly 22% of their size: 14px on the 64px home-page icon, 12px on the 56px title-row icon.
- Screenshot thumbnails get a soft 8px corner, like a phone screen.
- Official store badges stay at 0px rounding, because they already carry their own artwork shape. Never round or clip them.

## Components

Utilitarian with a wink: components are plain, labelled and honest about what they do. The personality lives in copy and app art, not in chrome.

### Site Header
- **Structure:** logo (24px) plus "Cargo Shorts Studios" in bold on the left (declared as 600 but rendered as 700, because only 400/500/700 are loaded), primary nav on the right. At least 52px tall, with a Seam Line hairline beneath. It wraps to two lines on narrow phones instead of hiding behind a menu.
- **Nav links:** Faded Denim Grey at rest, with no underline. On hover and on the current page (`aria-current="page"`) they switch to full-strength text color. There's no underline or pill indicator; the color shift is the only signal.

### Links
- **In-content links:** Rust Thread with the browser-default underline. They're the only interactive treatment in the system, since there are no styled buttons. There's no custom hover or focus style; the browser defaults apply.
- **Link rows** (`.links`): related links wrap in a row at 0.95rem with a 16px gap (Privacy Policy, Terms of Service).
- **Footer links:** muted rather than rust, so the footer recedes.

### Sheet (signature component)
- **Label cell:** a semantic `h2` restyled to 0.95rem, weight 500, Faded Denim Grey, in the 172px column.
- **Value cell:** body text, any content: app rows, badges, screenshots, a facts list, or fine print.
- **Rules:** a hairline on top of the sheet and under every cell, so labels and values are ruled together.
- **Usage:** on every studio and app page, holding "Apps", "Contact", "Get the app", "What it does", "Screenshots", "Details", "Legal" and "Help". This is how a new app page should be built.

### App Row
- A 64px rounded icon beside a stack of the app name (Title, linked), a one-sentence description, store badges, then a link row for legal pages. This is the studio home's unit of listing. Add one row per app.

### Store Badges
- Official Google Play and App Store artwork only, unmodified, with their accessible alt text. They're laid out in a wrapping flex row with an 8px × 16px gap.
- Google's PNG carries built-in clear space, so it's rendered at 156×60 with a −10px margin. That makes it optically match Apple's 120×40 SVG. Keep this trim whenever badges are added or resized.

### Facts List
- A two-column definition list (`max-content 1fr`, with a 6px × 24px gap): muted `dt` keys and plain `dd` values. Used for at-a-glance specs: status, platforms, price, ages, accounts.

### Tables
- **Standard** (Support page): full-width, 0.95rem, hairline under each row, muted 0.85rem weight-500 headers, no vertical rules.
- **Legal documents:** a full grid of hairlines with Pocket Lining header cells. The table scrolls horizontally at ≤480px.

### Screenshots
- 120px-wide thumbnails with 8px rounding, in a wrapping row with a 12px gap. Each one links to the full-size image. They're lazy-loaded and their alt text describes the screen.

### Footer
- A hairline above, then 0.85rem muted text: the copyright on the left and Privacy / Terms / Support on the right. The two sides wrap apart on phones.

### Legal Document
- The body carries `class="legal"`. It has a breadcrumb, an `h1`, a muted version/date meta line, then the article copied verbatim from source. Each article `h2` sits under a hairline. The styling is plain and stays joke-free.

## Do's and Don'ts

### Do:
- **Do** build every new app or studio page from the sheet: a 172px muted label column, hairline rows and 18px row padding.
- **Do** keep Rust Thread exclusively for links, and swap to `rust-thread-dark` in dark mode through the `--link` custom property.
- **Do** define any new color as a light/dark pair in the `:root` custom properties. Never hard-code a hex in a rule.
- **Do** round imagery only: app icons at ~22% of their size, screenshots at 8px, store badges at 0.
- **Do** let app icons, screenshots and store badges carry the page's color and personality, and keep the chrome around them neutral.
- **Do** keep official store badges unmodified and optically equal in height, using the Play badge's −10px trim.
- **Do** keep wit in the copy (ledes, descriptions) and keep legal pages visually and verbally plain.

### Don't:
- **Don't** add SaaS landing tropes: hero gradients, big filled CTA buttons, feature-card grids, testimonial carousels.
- **Don't** add fantasy or MTG pastiche: parchment textures, mana-symbol or card-frame ornament, gilded borders, or any Wizards of the Coast trademark used as decoration.
- **Don't** use shadows, elevated cards or background-tinted containers to group content. Rule it with a Seam Line hairline instead.
- **Don't** use Cargo Khaki anywhere outside the logo and icon SVGs.
- **Don't** introduce a second typeface or Roboto weights outside 400/500/700.
- **Don't** introduce cool or blue-grey neutrals. Every grey in the system is warm.
- **Don't** round, recolor, restyle or crop the store badges beyond the documented clear-space trim.
