---
name: Vincenzo Galiano Portfolio
description: A personal software portfolio with editorial typography and a calm forest palette.
colors:
  forest: "#132c29"
  ink: "#243c35"
  terracotta: "#a44b32"
  accent: "#edc59b"
  paper: "#f8f5ed"
  white: "#ffffff"
  muted: "#59665b"
  line: "#d4d6c9"
  work-surface: "#eceee3"
  button-surface: "#edc59b"
typography:
  display:
    fontFamily: "Manrope, Arial, sans-serif"
    fontSize: "clamp(58px, 6.65vw, 88px)"
    fontWeight: 450
    lineHeight: 1.05
    letterSpacing: "-0.04em"
  headline:
    fontFamily: "Manrope, Arial, sans-serif"
    fontSize: "clamp(34px, 3.8vw, 50px)"
    fontWeight: 450
    lineHeight: 1.17
    letterSpacing: "-0.035em"
  emphasis:
    fontFamily: "Newsreader, Georgia, serif"
    fontWeight: 400
    letterSpacing: "-0.025em"
  title:
    fontFamily: "Manrope, Arial, sans-serif"
    fontSize: "24px"
    fontWeight: 550
    lineHeight: 1.4
    letterSpacing: "-0.025em"
  body:
    fontFamily: "Manrope, Arial, sans-serif"
    fontSize: "16px"
    fontWeight: 400
    lineHeight: 1.75
  label:
    fontFamily: "Manrope, Arial, sans-serif"
    fontSize: "12px"
    fontWeight: 650
rounded:
  square: "0px"
  portrait: "160px 160px 8px 8px"
  portrait-mobile: "140px 140px 6px 6px"
  circle: "50%"
spacing:
  small: "16px"
  medium: "20px"
  large: "32px"
  column: "48px"
  section: "112px"
  section-tablet: "85px"
  section-mobile: "70px"
components:
  button-primary:
    backgroundColor: "{colors.button-surface}"
    textColor: "{colors.forest}"
    rounded: "{rounded.square}"
    padding: "15px 20px"
  button-primary-hover:
    backgroundColor: "{colors.white}"
  button-text:
    textColor: "{colors.ink}"
    padding: "8px 0"
  tag:
    textColor: "{colors.muted}"
    padding: "0 0 4px"
  contact-arrow:
    textColor: "{colors.paper}"
    rounded: "{rounded.circle}"
    width: "92px"
    height: "92px"
---

# Design System: Vincenzo Galiano Portfolio

## Overview

**Creative North Star: "Connected Editorial"**

Large, carefully spaced statements give the personal portfolio an editorial rhythm. A forest opening and contact section frame light reading surfaces; a personal portrait supplies the human focus. Manrope carries the practical voice, while Newsreader gives selected phrases a softer emphasis.

**Key Characteristics:**
- Forest framing with cream, white and pale terracotta reading surfaces.
- Sans-serif structure with upright serif emphasis.
- Open rows, fine dividers and generous section spacing.

## Colors

The palette pairs deep terracotta structure with cool accents and gently warm paper.

### Primary
- **Deep Forest:** Hero, header and contact backgrounds; primary button text.
- **Connection Terracotta:** Heading emphasis on light surfaces, skill illustrations and company names.

### Secondary
- **Soft Periwinkle:** Serif emphasis and link hover states on forest.

### Neutral
- **Warm Paper:** Main page background and text on forest.
- **Clean White:** Approach section, portrait backing and primary button hover.
- **Terracotta Ink:** Main text on light surfaces.
- **Slate:** Supporting prose and labels.
- **Mist Line:** Section, row and timeline dividers.
- **Pale Terracotta:** Work section background.
- **Frosted Terracotta:** Primary action background.

## Typography

**Display and Body Font:** Manrope, falling back to Arial and sans-serif.
**Emphasis Font:** Newsreader, falling back to Georgia and serif; upright, not italic.

The frontmatter captures the desktop hierarchy. Heading emphasis grows slightly relative to its parent: hero phrases (1.06em), section phrases (1.08em). Supporting prose usually uses smaller text (13–15px); introductory leads use a more spacious size (21px, line-height 1.6). Tags and captions sit at the smallest tier (11px). Fonts are hosted locally.

## Layout

The centered container is capped at (1184px), with desktop side space (48px). The hero uses a two-column ratio (1.28:1), with a gap (64px). Approach, work and career use related two-column grids. Skill rows align a title, description and line icon; the timeline aligns dates with role descriptions.

At widths up to (1000px), side space becomes (32px), gaps narrow and section spacing uses the tablet token. At widths up to (700px), side space becomes (20px), major grids stack, section spacing uses the mobile token, and navigation collapses into an expandable menu. Skill descriptions move below their title and icon. The portrait is centered and capped at (380px), with a wider crop. The hero title uses `clamp(49px, 10.8vw, 72px)` on mobile; section titles use `clamp(30px, 7.5vw, 42px)`.

At widths from (1400px), hero top space expands to (76px). Text widths remain constrained: hero description (510px), skill descriptions (540px), career and disclosure copy (65ch).

## Elevation & Depth

No shadows are used. Depth comes from full-width tonal sections, fine borders and the portrait silhouette. Hero copy and portrait enter from a small vertical offset on desktop when motion is allowed; reduced-motion preference removes animation and smooth scrolling.

## Shapes

Actions and content rows use square edges. The portrait is a transparent PNG cutout with no background or corner masking; the email arrow is circular. Fine line icons share rounded strokes. Borders divide content rather than enclosing it in cards.

## Components

### Buttons

The primary action is compact, pale terracotta and rectangular, with a right arrow and bold small text (12px, weight 750). Hover changes its background to white. Text actions use a thin underline and an arrow. Interactive elements share a visible terracotta focus outline (3px, offset 6px).

### Chips

Technology tags are static labels with a thin lower border, muted text and no filled capsule background. They wrap naturally across rows.

### Navigation

Compact Manrope labels sit opposite the two-line personal signature. Links turn apricot on hover. On mobile, a bordered Menu button reveals vertically stacked links with dividers; its expanded state is exposed to assistive technology.

### Skill Rows and Timeline

Skill rows are separated by top borders and use terracotta line illustrations. Career entries pair compact date/location metadata with a larger role title, terracotta company name and supporting prose. Both patterns stack on mobile.

### Project Entries

The projects section inherits the white surface, forest text and terracotta accents. Open entries pair a large project name (40–62px), category and contribution note with a summary, capability list and technology tags. Desktop columns use a 1:1.2 ratio with a 90px gap, reduced to 45px below 1000px. Below 700px each entry stacks with a 30px gap. Top rules separate projects; no elevated cards or new visual tokens are introduced.

### Work Disclosures

Native details elements use thin dividers and a plus that becomes a minus when open. The first disclosure starts open. Summary labels remain keyboard operable.

## Do's and Don'ts

### Do:
- Do pair Manrope structure with upright Newsreader emphasis.
- Do use the forest framing and light reading surfaces consistently.
- Do preserve visible focus and reduced-motion behavior.
- Do use the supplied local portrait as the personal image.

### Don't:
- Don't replace the open skill rows and timeline with raised cards.
- Don't add shadows to the established flat surfaces.
- Don't style static technology tags as interactive filters.

The portrait uses `assets/vincenzo-galiano-trasparente.png`, with a transparent container and `object-fit: cover` to give the subject a prominent scale, with transparent margins retained in the source. The original JPEG is retained. Project participation is labelled «Co-sviluppatore del progetto».

The header signature displays “Vincenzo” in upright Newsreader, 36px (32px on mobile), above “GALIANO” in 11px Manrope with .28em tracking. The first name is ivory and the surname apricot; no terminal dot.
