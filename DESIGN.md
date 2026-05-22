<!-- SEED: re-run /impeccable document once there's code to capture the actual tokens and components. -->

---
name: Alan Portfolio
description: Warm, restrained craft-forward portfolio for recruiters — warm stone neutrals, humanist sans, responsive motion.
---

# Design System: Alan Portfolio

## Overview

**Creative North Star: "The Craft Ledger"**

A hiring-facing portfolio that reads like a calm, intentional product page, not a resume PDF or a framework starter. Warm stone neutrals carry most of the surface; a single ink accent appears only where action matters (project links, contact). Typography is one warm humanist sans family used with clear weight steps, not a display/body split. Motion responds to interaction and scroll position without choreographed spectacle.

This system explicitly rejects the default Next.js / Vercel template look (zinc boilerplate, Geist-as-default, "Deploy Now" hero patterns) and any drift toward ElevenLabs-style editorial clones (pastel gradient orbs, licensed display serifs). The goal is product-marketing polish with human warmth, not SaaS cliché or AI slop.

**Key Characteristics:**
- Restrained palette: tinted warm stone canvas + near-black ink accent ≤10% of any screen
- Single warm humanist sans for all roles; hierarchy via scale and weight, not a second display face
- Responsive motion: transitions and hover feedback; no scroll choreography on v1
- Project-first layout rhythm; marketing chrome stays quiet
- AA baseline with AAA where easy; reduced motion honored strictly

## Colors

**The Restrained Accent Rule.** Tinted neutrals own the canvas. The ink accent appears on primary CTAs, active nav, and key links only. If more than ~10% of a viewport reads as accent, the screen is too loud.

**The Warm Stone Rule.** Neutrals tint toward warm stone (cream canvas, warm gray body, near-black ink). Pure `#000` and `#fff` are forbidden; even near-neutrals carry a subtle warm hue.

Palette direction (values resolved at implementation):

- **Canvas** `[to be resolved]`: Off-white / warm cream page floor
- **Ink** `[to be resolved]`: Near-black primary text and accent actions
- **Body** `[to be resolved]`: Warm mid-gray for supporting copy
- **Muted** `[to be resolved]`: Labels, meta, timestamps on case studies
- **Hairline** `[to be resolved]`: Dividers between project rows and sections
- **Surface card** `[to be resolved]`: Project cards and media frames on canvas

## Typography

**Font pairing:** `[warm humanist sans to be chosen at implementation — e.g. Inter, Source Sans 3, or similar]`

**Character:** Readable, friendly, and precise. Feels like a product UI, not a magazine masthead. No second display serif in v1.

### Hierarchy
- **Display** (semibold, large scale, tight tracking): Hero name or one-line positioning only
- **Headline** (semibold, section titles): "Selected work", case study titles
- **Title** (medium, card titles): Project names in grids and lists
- **Body** (regular, 16px, ~1.5 line-height, max 65–75ch): Case study summaries, about copy
- **Label** (medium, small, optional uppercase tracking): Section labels, tech tags

**The Single-Voice Rule.** One family end-to-end. Differentiate with size and weight, not by introducing a display face for "personality."

## Elevation

Flat-by-default on a warm canvas. Depth comes from hairline borders and subtle surface shifts (canvas → card), not stacked shadows. **The Responsive Lift Rule.** A single soft shadow tier may appear on hover for project cards only; shadows never define the brand at rest.

Shadow vocabulary: `[to be resolved during implementation]`

## Components

_No component tokens yet — project is pre-implementation. Re-run `/impeccable document` in scan mode after the first real UI ships._

Expected primitives to document next pass: top nav, project card, text link/CTA, section divider, footer.

## Do's and Don'ts

### Do
- Keep the ink accent scarce; let project imagery and type hierarchy carry the page
- Use warm stone neutrals on every surface and border
- Honor WCAG AA minimum; push contrast and focus to AAA where straightforward
- Respect `prefers-reduced-motion` for all transitions

### Don't
- Don't ship the create-next-app starter aesthetic (default Geist hero, zinc palette, template CTAs)
- Don't clone ElevenLabs editorial (Waldenburg-style display, pastel gradient orbs)
- Don't add hero metrics, identical icon-card grids, or purple-gradient dark mode
- Don't use gradient text, glassmorphism decor, or side-stripe accent borders
- Don't introduce a second display typeface until the single-sans system is fully expressed
