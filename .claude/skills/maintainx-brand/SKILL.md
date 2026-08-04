---
name: maintainx-brand
description: Apply MaintainX brand guidelines to any output -- HTML/CSS components, copy, presentations, decks, or documents. Use whenever the task requires on-brand visual design, writing in MaintainX voice, or producing content that represents the MaintainX brand.
---

# MaintainX Brand System

## Overview

This skill encodes MaintainX's brand system: colors, typography, voice, writing rules, component patterns, logo usage, and photography direction. Apply it whenever producing anything that represents MaintainX externally or internally.

Sourced from: *MaintainX Brand Identity Guidelines (2025)*, *MaintainX Writing Style Guide*, the *Title Case Guidelines* (product/UX), the *EPD Onboarding Guide*, and the `Visual Library` Figma file already mirrored in this repo's `assets/` folder.

**Keywords**: MaintainX brand, on-brand, style guide, brand colors, typography, brand voice, CMMS, frontline workers, maintenance, components, copy, capitalization

---

## 1. Colors

### Primary Palette

| Token | Hex | Pantone | Use |
|---|---|---|---|
| Titanium White | `#FFFFFF` | White | Page backgrounds, card fills |
| MaintainX Blue | `#246CFF` | 2728 C | Primary brand color, CTAs, links |
| Hydraulic Blue | `#001E40` | 4146 C | Dark backgrounds, headers, footers -- MaintainX's dark surface color |

### Secondary Palette

| Token | Hex | Pantone | Use |
|---|---|---|---|
| Safety Green | `#2ED888` | 7479 C | Success states, secondary accent |
| Safety Orange | `#FFA945` | 804 C | Warning states, secondary accent |

The palette is intentionally inspired by MX users' day-to-day environments -- industrial signage, safety jackets -- to create trust and familiarity with frontline audiences.

### Extended UI Tokens

These extend the marketing palette above for product/UI and this design system; sourced from the `Visual Library` Figma file already in this repo.

| Token | Hex | Use |
|---|---|---|
| Blue-2 | `#6996FF` | Hover/active tint |
| Blue-3 | `#BED2FF` | Light backgrounds, disabled states |
| Blue-4 | `#E8EFFF` | Subtle section backgrounds |
| Blue-5 | `#F5F8FF` | Lightest tint |
| Secondary Dark Blue | `#003161` | Alternate dark surface |
| Grey-1 | `#4C6177` | Secondary text on light |
| Grey-2 | `#B4BBC5` | Borders, disabled |
| Grey-3 | `#E5E8EC` | Dividers, card borders |
| Red-1 | `#FB523C` | Error/destructive |
| Red-2 | `#FFEAE7` | Error background tint |
| CoPilot gradient | `#246CFF` -> `#2ED888` | MaintainX Assist / AI features only |

### Color Ratio

Lead with MaintainX Blue; use tints and shades for the rest of the palette to preserve visual hierarchy. Don't let secondary colors (green/orange) compete with blue for dominance.

### Recommended Text/Background Combinations

- Hydraulic Blue text on white background
- White text on MaintainX Blue background
- White text on Hydraulic Blue background
- Hydraulic Blue text on Safety Green / Safety Orange / light grey backgrounds

---

## 2. Typography

### Typeface: Inter

MaintainX uses **Inter** (free, open-source -- available via Google Fonts, no licensing needed) across logo, headlines, and body, varying only by weight:

| Use | Weight |
|---|---|
| Logo / wordmark | Inter Bold & Extra Bold |
| Headlines | Inter Bold |
| Body copy | Inter Regular & Medium |

### Spacing Specs

| | Leading | Letter spacing |
|---|---|---|
| Headlines | 110% | 0% |
| Body copy | 120% | 0% |

### CSS Quick Reference

```css
--font-sans: 'Inter', -apple-system, BlinkMacSystemFont, 'Segoe UI', Helvetica, Arial, sans-serif;

/* Headlines */
h1, h2, h3 { font-family: var(--font-sans); font-weight: 700; line-height: 1.1; letter-spacing: 0; }

/* Body */
p, li { font-family: var(--font-sans); font-weight: 400; line-height: 1.2; letter-spacing: 0; }
```

### Capitalization -- context matters, don't flatten this

**Marketing content** (website copy, ads, decks, emails, blog/press headlines) -- per the Writing Style Guide:
- Sentence case for H1, H2, subheads, and body: "Bring unplanned equipment downtime to zero"
- Title case for CTAs/buttons, blog post titles, and press release headlines
- Capitalize proper nouns and product names: "MaintainX CoPilot"
- Keep industry acronyms in caps: PM, CMMS, MTTR, OEE

**Product UI** (app screens, this design system, in-product copy) -- per the Title Case Guidelines, using simplified AP style:
- **Title case** for: page titles, section headers, nav items, buttons/CTAs (3 words or fewer), modal titles
- **Sentence case** for: body copy, helper text, tooltips, empty-state descriptions, error messages, links, CTAs (4+ words)
- Capitalize: nouns, verbs, adjectives, pronouns. Lowercase: articles, conjunctions, short prepositions. Default to lowercase when in doubt.
- **Functional terms are always capitalized as proper nouns** (exact term only, not descriptive variants): Asset, Work Order, Work Request, Procedure, Part, Parts Inventory, Purchase Orders, Locations, Vendors, Automations, Meters, MaintainX CoPilot, Report Builder, Asset Hub
  - Do: "Work Order" · Don't: "Maintenance Work Order"
- Don't stack multiple capitalized functional terms back-to-back in one sentence -- split into steps or use pronouns instead.
- Buttons: 2-4 words max, verb + noun format ("Create Work Order," not "Create a New Work Order for this Asset").

---

## 3. Voice & Tone

### Voice (constant across everything we write)

- **Authoritative** -- Knowledgeable, experienced, accurate, industry-savvy.
- **Helpful** -- Focused on solutions, empowering, supportive.
- **Professional** -- Clear, concise, reliable.
- **Relatable** -- Friendly, approachable, down-to-earth.

### Tone (shifts by context, voice stays constant)

- **Informative** -- Educational, insights-driven, data-focused.
- **Direct** -- Straightforward, no-nonsense, action-oriented.
- **Empathetic** -- Understands user challenges, celebrates the customer as the hero.
- **Optimistic** -- Future-focused, confident in better tools.
- **Conversational** -- Friendly, engaging, easy to understand.

### Mission & Vision

- **Mission**: To equip frontline professionals with modern tools that streamline maintenance, maximize equipment uptime, and drive operational excellence across physical-asset-driven industries.
- **Vision**: A world where equipment downtime is a thing of the past -- achieved through AI-driven solutions, optimized workflows, and interconnected data that elevate frontline worker efficiency and safety.

### Values

1. **Entitled to Nothing, Grateful for Everything** -- no one owes us anything; we put in the work.
2. **Excellence Is Our Standard** -- brilliance, effort, and ownership.
3. **Collaboration Over Ego** -- strong opinions, weakly held.
4. **Embrace Challenges, Find Opportunity** -- calculated risks, learn fast, stay optimistic.

### The CA3 Framework for Writing

Every piece of content should be **Clear, Accurate, Actionable, and Discoverable**:

- **Clear**: Simple, human language. Active voice always. Short words over long ones ("start" not "initiate," "show" not "demonstrate," "help" not "assist"). Be humble -- share knowledge like a peer, not a lecture.
- **Accurate**: Get maintenance terminology right -- readers will spot mistakes immediately. Don't overclaim: say "decrease unplanned downtime," never "eliminate downtime." Use real field examples, not generic stock scenarios.
- **Actionable**: Every piece ends with a clear next step (try a feature, read more, take an implementation step).
- **Discoverable**: Structure for search, connect related content, tag strategically.

### Do / Don't

| Do | Don't |
|---|---|
| "See exactly where downtime is costing you." | "Leveraging next-generation AI-powered solutions..." |
| "Transform your maintenance operations with smart PM scheduling." | "Our revolutionary system is the best you've never tried." |
| "Many maintenance teams see a 32% drop in unplanned downtime with a PM schedule." | "Trust us, we've built the most advanced algorithms in the industry." |

Banned pattern: don't position MaintainX as smarter than the reader, or dismiss their current practices. Partner with them, don't lecture them.

---

## 4. Grammar & Punctuation

- American English spelling and grammar.
- **Oxford (serial) comma**: "bearings, seals, and gaskets." (This is the one deliberate deviation from standard AP style.)
- **Em dash** for breaks -- no spaces around them.
- One space after periods.
- Colons introduce lists.
- **Numbers**: spell out one through nine ("three bearings"); numerals for 10+ ("15 machines"); always numerals for measurements with units ("50 psi," "3 inches," not "½ inch" -- use decimals). Dates: MM/DD/YYYY.
- **Quotes**: present tense ("says," "explains") for timeless statements; past tense ("said," "explained") for specific events -- stay consistent within one piece. Double quotes for direct quotes, single for quotes within quotes.
- **Trademark**: MaintainX® on the first / most prominent use per page or piece of collateral (don't stress over every instance).

---

## 5. Logo Usage

- Logo is left-aligned -- works best placed in a left corner.
- Maintain generous clear space around the logo on all sides (see the Figma Foundations file for the exact measurement).
- **Never**: stretch, rotate, apply effects, recolor to one flat color, flip the X, outline, move/rearrange elements, or apply gradients to the logo itself.
- Actual logo files (black, white, and the MaintainX Assist / AI sub-brand lockups) live in `assets/logos/` and `assets/assist/` in this repo.

---

## 6. Photography & Imagery

- Real people are the heroes of the story -- diverse across industries, ages, genders, ethnicities, so the audience sees themselves in the content.
- Locations should be real industrial/manufacturing environments -- organized, efficient, safe -- ideally showing the product in context.
- **Never**: forced/unnatural posing, unrealistic photo collages, untidy environments, competitor apps visible on any screen, generic disconnected stock photography.

---

## 7. Components

Component patterns as implemented in this repo's design system page (`index.html` / `styles.css`) -- rounded, friendly, not sharp-cornered:

```css
/* Primary button -- pill shaped */
.btn-primary {
  background: #246CFF; /* MaintainX Blue */
  color: #fff;
  border: none;
  border-radius: 999px;
  padding: 9px 16px;
  font-weight: 600;
}
.btn-primary:hover { background: #003161; } /* Secondary Dark Blue */

/* Cards */
.card {
  background: #fff;
  border: 1px solid #E5E8EC; /* Grey-3 */
  border-radius: 14px;
  padding: 18px;
  box-shadow: 0 1px 2px rgba(0,30,64,0.06);
}

/* Dark surface (heroes, footers, nav) */
.surface-dark { background: #001E40; color: #fff; } /* Hydraulic Blue, never a blue-black substitute */
```

- Pills/tags: rounded (`border-radius: 999px`), not sharp -- MaintainX's visual language is rounded and approachable, unlike sharp-cornered competitor systems.
- Hover states: subtle lift (`translateY(-2px to -4px)`) + soft shadow increase, consistent with the "Relatable/Helpful" voice -- interactions should feel responsive, not aggressive.

---

## 8. Iconography

- MaintainX's icon language favors sharp angles that echo the logo's own geometry, even though components/buttons are rounded.
- Base library: 3,000+ icons (Streamline, organized into 56+ categories per the `Visual Library` Figma file already indexed in this repo).

---

## 9. Devices & UI Mockups

- Use clay-style 3D device mockups for product shots.
- iOS devices are the default; use Android-styled devices only for Android-specific callouts.

---

## 10. Spacing

Not explicitly published with exact pixel tokens in the sourced docs -- this repo's design system uses a conventional 4px-based scale. Treat as a working default, not an official spec, until confirmed against the Figma `Foundations` file (`Colors, typography, spacing, elevation`).

```css
--space-1: 4px;  --space-2: 8px;   --space-3: 12px;  --space-4: 16px;
--space-6: 24px; --space-8: 32px;  --space-12: 48px; --space-16: 64px;
```

---

## How to Apply This Skill

**For HTML/CSS components**: MaintainX Blue as the lead color, Hydraulic Blue for dark surfaces (never a blue-black or near-black substitute), Inter for all type, rounded corners and pill buttons (not sharp), sharp-angled icons only. Reuse the logo/Assist assets already in `assets/`.

**For copy**: Voice is Authoritative + Helpful + Professional + Relatable, always. Tone shifts by context (informative, direct, empathetic, optimistic, conversational) but never becomes boastful or dismissive of the reader's experience. Apply CA3 (Clear, Accurate, Actionable, Discoverable). Use sentence case for marketing headlines/body, title case for buttons/CTAs and product UI headers -- see section 2 for the full split.

**For presentations/documents**: MaintainX Blue + Hydraulic Blue dominant, Safety Green/Orange as accents only, Inter throughout, real photography (never stock collages), logo left-aligned with clear space respected.

**For data viz** (not yet covered by a published MaintainX-specific spec): default to the same palette hierarchy above -- MaintainX Blue as the primary series, Safety Green/Orange as secondary/accent, Grey-2/Grey-3 for gridlines and inactive states -- until an official chart spec is published.
