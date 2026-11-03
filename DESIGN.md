---
name: berlines.es
description: Tours de Berlín en español, hechos por un guía local.
colors:
  forest-ink: "#0B3B2E"
  forest-ink-soft: "#4A6B52"
  notebook-paper: "#F4EFE6"
  paper-shade: "#EBE4D5"
  hairline: "#D9D0BE"
  ink: "#1A1A1A"
  ink-soft: "#4A4A42"
  pencil: "#696559"
typography:
  display:
    fontFamily: "Fraunces, serif"
    fontSize: "92px"
    fontWeight: 700
    lineHeight: 0.98
    letterSpacing: "-3px"
  headline:
    fontFamily: "Fraunces, serif"
    fontSize: "64px"
    fontWeight: 700
    lineHeight: 1
    letterSpacing: "-1.5px"
  headline-sm:
    fontFamily: "Fraunces, serif"
    fontSize: "48px"
    fontWeight: 700
    letterSpacing: "-1px"
  title:
    fontFamily: "Fraunces, serif"
    fontSize: "24px"
    fontWeight: 600
    lineHeight: 1.15
    letterSpacing: "-0.3px"
  figure:
    fontFamily: "Fraunces, serif"
    fontSize: "20px"
    fontWeight: 600
  lead:
    fontFamily: "Inter, sans-serif"
    fontSize: "20px"
    fontWeight: 300
    lineHeight: 1.55
  body:
    fontFamily: "Inter, sans-serif"
    fontSize: "17px"
    fontWeight: 400
    lineHeight: 1.7
  label:
    fontFamily: "Inter, sans-serif"
    fontSize: "11px"
    fontWeight: 600
    letterSpacing: "3px"
  button:
    fontFamily: "Inter, sans-serif"
    fontSize: "13px"
    fontWeight: 600
    letterSpacing: "1.5px"
rounded:
  none: "0px"
spacing:
  gutter-mobile: "20px"
  gutter-desktop: "48px"
  card: "32px 28px"
  section-mobile: "80px"
  section: "120px"
  section-lg: "140px"
components:
  button-primary:
    backgroundColor: "{colors.forest-ink}"
    textColor: "{colors.notebook-paper}"
    typography: "{typography.button}"
    rounded: "{rounded.none}"
    padding: "14px 28px"
  button-primary-hover:
    backgroundColor: "{colors.forest-ink-soft}"
  button-inverse:
    backgroundColor: "{colors.notebook-paper}"
    textColor: "{colors.forest-ink}"
    rounded: "{rounded.none}"
    padding: "16px 36px"
  button-inverse-hover:
    backgroundColor: "{colors.paper-shade}"
  nav:
    backgroundColor: "{colors.notebook-paper}"
    height: "72px"
  tour-card:
    backgroundColor: "{colors.notebook-paper}"
    rounded: "{rounded.none}"
    padding: "{spacing.card}"
  tour-card-hover:
    backgroundColor: "{colors.paper-shade}"
---

# Design System: berlines.es

## Overview

**Creative North Star: "The Guide's Field Notebook"**

The site reads like the personal notebook of a local guide. It uses warm cream paper, near-black ink, a single forest-green pen and thin ruled lines. Information is written down, not advertised: the tour name in a confident serif, the logistics (duration, schedule, price) set out as a small ruled ledger beneath it, and one clear way to get in touch. Nothing floats, glows or rounds off. The page sits flat like paper, and hierarchy comes from type size, weight and ruled lines.

Density is generous. Sections breathe at 120px or more, featured tours each get a full viewport, and the secondary catalog becomes a tight hairline grid, like a list at the back of the notebook. Tour photography supplies the colour and life. The interface stays quiet so the photos and the facts carry the page.

The look must never slide toward a generic tour-agency site (stock-photo heroes, shouting orange "Book now!" buttons, star-rating clutter) or toward touristy Berlin kitsch (Ampelmännchen, bears or flags used as decoration).

**Key Characteristics:**
- Cream paper ground, near-black ink, one green accent
- Fraunces serif for anything you'd write by hand: names, headings, prices
- Inter in small, wide-tracked uppercase for labels and buttons
- Square corners, no shadows, 1px hairline rules for structure
- Full-bleed tour photography alongside text (a split-screen layout)

## Colors

Warm, low-saturation paper tones with a single deep green that does all the pointing.

### Primary
- **Forest Ink** (`forest-ink`): The guide's pen. Used for primary buttons, eyebrow and tag labels, the italic accent in the hero headline, the dot in the "berlines.es" wordmark, and as the full background of the booking (contact) section. It is the only colour that means "act here".
- **Forest Ink, Soft** (`forest-ink-soft`): Hover state for Forest Ink buttons only. It is never used at rest.

### Neutral
- **Notebook Paper** (`notebook-paper`): The page ground, nav background and card surface. Also the text colour on Forest Ink.
- **Paper Shade** (`paper-shade`): A slightly darker page. Used as the background of the "Más tours" band, as photo placeholders, and for card and inverse-button hover.
- **Hairline** (`hairline`): Every rule and border: nav bottom, section dividers, the ledger rows above and below tour facts, and the 1px gaps between catalog cards.
- **Ink** (`ink`): Headlines, wordmark, tour titles and prices.
- **Ink, Soft** (`ink-soft`): Body copy and lead paragraphs.
- **Pencil** (`pencil`): Secondary info: fact-label keys, schedules, small price notes, footer links and copyright. Darkened from #8A8578 so it passes WCAG AA on both papers (5.1:1 on Notebook Paper, 4.6:1 on Paper Shade). Don't lighten it.

### Named Rules
**The One Pen Rule.** Forest Ink is the only chromatic colour in the interface. Colour beyond it comes from photography, never from new UI hues. (A `--wa` WhatsApp green is declared in the CSS but deliberately unused. Keep it that way.)

**The Green Room Rule.** Forest Ink fills a whole section only once per page: the closing booking block. Anywhere else it stays at button or label scale.

## Typography

**Display Font:** Fraunces (with serif fallback), weights 600–800
**Body Font:** Inter (with sans-serif fallback), weights 300–600

**Character:** Fraunces is the handwriting: soft-edged and literary, with an italic that adds warmth to a single word in the hero line. Inter is the printed form: small, uppercase and widely tracked for labels, light and roomy for prose.

### Hierarchy
- **Display** (Fraunces 700, 92px → 54px on mobile, line-height 0.98, -3px): The hero headline only. One word or phrase may be set in Fraunces italic 600 in Forest Ink.
- **Headline** (Fraunces 700, 64px → 44px under 900px, line-height 1.0, -1.5px): Featured tour names. The booking section uses a 72px → 48px variant.
- **Headline, Small** (Fraunces 700, 48px → 36px, -1px): Section headers such as "Resto del catálogo".
- **Title** (Fraunces 600, 24px, line-height 1.15): Catalog card tour names.
- **Figure** (Fraunces 600, 20–22px): The values in fact rows and prices. Logistics are set in the serif so they read as hand-noted facts, with small Inter 12px Pencil annotations alongside.
- **Lead** (Inter 300, 20px → 17px, line-height 1.55, max ~580px): Hero and booking intro paragraphs.
- **Body** (Inter 400, 17px, line-height 1.7, max ~440px): Tour descriptions.
- **Label** (Inter 600, 11px minimum, 2–3px tracking, uppercase, Forest Ink): Eyebrows, tour-type tags and fact keys (keys use Pencil). Never below 11px.

### Named Rules
**The Serif-for-Facts Rule.** Anything a traveller needs to note down (tour name, duration, time, price) is set in Fraunces. Inter handles labels, explanations and actions.

**The Whisper Label Rule.** Labels are tiny, uppercase and widely tracked (≥1.5px). They never grow into headings and never appear in sentence case.

## Layout

- **Container:** Content is capped at 1100px and centred, with side gutters of 48px on desktop and 20–24px on mobile.
- **Hero intro:** Left-aligned, never centred. Padding is 120px above and 80px below.
- **Featured tours (signature):** Two equal columns at a minimum of 100vh. The photo column is sticky under the 72px nav while the text column scrolls, and sections alternate photo-left and photo-right (`reverse`). Under 900px the layout stacks to one column with the photo first at 60vh, and text padding drops to 60px/32px.
- **Catalog:** An auto-fill grid with columns of at least 300px. Cards are separated by 1px Hairline gaps (the grid background shows through), framed by a 1px Hairline border.
- **Section rhythm:** Vertical padding is 120px for standard sections and 140px for the booking block, dropping to 80–90px under 600px. Each section is separated by a 1px Hairline top border.
- **Breakpoints:** 900px (split layouts stack) and 600px (type and padding step down).

## Elevation & Depth

The system is completely flat. There are no box-shadows anywhere. Depth comes from tone (Notebook Paper against Paper Shade against Forest Ink) and from 1px Hairline rules. The only overlay is a faint diagonal Forest Ink wash (0–15% opacity) on the bottom-right corner of tour photos, which ties the photography to the palette.

### Named Rules
**The Flat Page Rule.** Surfaces never lift. Hover changes the paper tone (to Paper Shade) or the ink tone (to Forest Ink, Soft), never elevation.

## Shapes

All corners are square (0px). Buttons, cards, photo panels and the booking block are rectangles cut from the page. Structure is drawn with 1px Hairline lines rather than with boxes: ruled rows above and below the tour facts, a rule above each catalog price, and rules between sections. A thin 40px line after the "Tours ↓" scroll cue is the one decorative line.

## Components

### Buttons
Small and printed, like a stamp. Never loud.
- **Shape:** Square corners (0px). Inline-flex, with a 10px gap before a trailing arrow (→).
- **Primary:** Forest Ink background with Notebook Paper text, using the uppercase button label (Inter 600 13px, 1.5px tracking). Padding is 14px 28px in tour sections and 11px 22px in the nav.
- **Hover:** The background shifts to Forest Ink, Soft over 0.2s, and the trailing arrow moves 4px right (`transform 0.2s`).
- **Inverse:** On the Forest Ink booking block, the button flips to a Notebook Paper background with Forest Ink text (Inter 600 14px, 2px tracking, 16px 36px), and hovers to Paper Shade.
- **Focus:** No focus-visible style is defined yet. This is a known gap: add a Forest Ink outline that is visible on both cream and green.

### Fact Ledger (signature)
A row of duration, schedule and price under each featured tour, set between two 1px Hairline rules with 20px vertical padding and 32px gaps between items. Each item has a Pencil uppercase key (11px, 2px tracking) above a Fraunces 600 20px value, with an optional small Inter Pencil annotation.

### Cards / Containers (Catalog cards)
- **Corner Style:** Square (0px).
- **Background:** Notebook Paper, hovering to Paper Shade.
- **Shadow Strategy:** None (see Elevation & Depth).
- **Border:** None of their own. They are separated by the grid's 1px Hairline gaps.
- **Internal Padding:** 32px 28px. From top to bottom: a Forest Ink type label (11px), then the Fraunces title, then a Pencil 13px schedule line, then the price row pinned to the bottom above a Hairline rule.
- **Booking:** The whole card is a WhatsApp link with a pre-filled message naming the tour. The price row ends in a Forest Ink uppercase "Reservar →" (Inter 600 12px), and the arrow moves 4px right on hover and focus. On keyboard focus the card shows a 2px Forest Ink outline inset inside its edges. The price row wraps when it runs out of room.

### Navigation
- A sticky top bar, 72px tall, on Notebook Paper with a 1px Hairline bottom border.
- The "berlines.es" wordmark is set in Fraunces 700 24px with the dot in Forest Ink, and a single primary "Reservar" button sits at the right.
- On mobile the side padding drops to 20px. There is no hamburger on the landing page.

### Footer
Centred on Notebook Paper with a Hairline top border. It contains the wordmark repeated at 22px, uppercase Pencil links (12px, 1.5px tracking) that hover to Ink, and an 11px copyright with a legal line.

## Do's and Don'ts

### Do:
- **Do** keep Forest Ink as the single interface accent and let tour photography supply all other colour.
- **Do** set tour names, logistics and prices in Fraunces, and labels and buttons in uppercase tracked Inter.
- **Do** draw structure with 1px Hairline rules and tonal shifts between Notebook Paper and Paper Shade.
- **Do** keep corners square and surfaces flat.
- **Do** give every featured tour a real photo of that tour, at full bleed.
- **Do** end every page with one clear WhatsApp booking action.

### Don't:
- **Don't** make it look like a generic tour agency: no stock-photo heroes, no bright orange or red "Book now!" buttons, no star-rating or badge clutter.
- **Don't** use touristy Berlin kitsch (Ampelmännchen, bears, flags, the TV tower as an icon) as decoration.
- **Don't** add drop shadows, glows or elevation on hover.
- **Don't** introduce a second accent hue, including WhatsApp green on buttons.
- **Don't** centre the hero intro. Only the booking block and footer are centred.
