# GnR Pitch Visual Design System

## Canonical Use

Before any image generation or slide visual edit, read this file and state which rules are being applied. This file is the visual source of truth for `GnR_deck.html`.

## Palette

- Cream: `#fbf7ef`
- Ink: `#1a1612`
- Gold: `#b8954a`
- Blue: `#5B8FD4`
- Rust: `#c8462c`
- Muted gold: `#d4a853`
- Paper background fallback used in older slide CSS: `#f3ead8`
- Never green for hero imagery. Existing legacy green marks may remain only on structured/data slides where already present; do not introduce green into new visuals.

## Typography

Fonts currently loaded or used in the deck:

- Primary serif/display: `Fraunces`, `Playfair Display`, Georgia, serif.
- Editorial fallback serif: `Libre Caslon Display`, `Libre Caslon Text`, Georgia, serif.
- Primary sans/UI: `Manrope`, `DM Sans`, Inter, sans-serif.
- Mono/data: `JetBrains Mono`, monospace.

Scale guidance:

- Opener-scale thesis: `clamp(2.35rem, 4.25vw, 4.05rem)` when the image has enough quiet space. Use tight line-height `1.05` to `1.10`.
- Hero/mission headline: `clamp(2.4rem, 3.8vw, 4.0rem)`, line-height `1.08` to `1.16`.
- Internal slide headline: `clamp(1.9rem, 3vw, 3.2rem)`, line-height `1.10` to `1.18`.
- Body/supporting copy: `0.95rem` to `1.35rem`, line-height `1.35` to `1.60`.
- Eyebrow: top-left labels at `top:28px; left:48px`; Manrope uppercase, `.58rem`, `700`, `.22em` letter-spacing, gold `#b8954a` or rust `#c8462c`.

Emphasis treatment:

- `#1 predictor`: italic serif, deeper readable gold `#8a6420` or canonical gold `#b8954a` with subtle shadow.
- `giving`: blue `#5B8FD4`, bold enough to read against the painting.
- `receiving`: rust `#c8462c`, bold enough to read against the painting.
- If colored words fade into the image, add only `text-shadow: 0 1px 2px rgba(0,0,0,0.25)` or slightly deepen the color. Do not add boxes, backdrops, blur panels, or overlays behind hero type.

## Layout

- Hero, opener, mission, transition, and closer slides use full-bleed imagery. The painting is the slide.
- Title overlays sit inside a deliberately quiet zone, typically `left:6%` and `top:7%` to `8%`.
- Compose hero images with the upper-left third quiet unless the slide explicitly uses a different title location.
- Preserve the GnR mark in the upper-right when the slide family uses it.
- No image-in-a-box treatment on big-moment slides: no cream margins, max-width frame, border radius, box shadow, or centered-card crop.
- Structured slides, comparisons, data tables, and spec slides keep the clean editorial typographic treatment. Do not painterify them.

## Hero Image Aesthetic

- Warm editorial brush-and-wash painting.
- Andrew Wyeth x Adrian Tomine New Yorker cover register.
- Painterly soft edges, cinematic depth, mythic register, everyday American authenticity.
- Palette stays cream, gold, rust, muted blue, ink accents.
- The image should embody the claim at iconic scale, not literally illustrate a brochure scene.

## Permanent Banned Aesthetics

- Pickleball, racquet sports, courts, nets, paddles, balls, athletic gear on the first slide.
- Green in hero imagery.
- Mediterranean, villa, terra cotta, olive-tree, European-cafe register.
- Hallmark card, memoir cover, senior-living brochure, Anthropologie catalog, wellness-brand vibe.
- Stock-photo diversity staging or fake posed smiles.
- Photorealism, digital-flat illustration, cartoon.
- Paddle clusters, four-paddle flower compositions, paddle-only product shots.
- Transactional prop metaphors as emotional center: keys, envelopes, invitations, documents, contracts, gifts, phones.
- Melancholy sunset-as-ending.

## Image Generation Mode

SPECIFIC mode: Dave gives an explicit creative brief. Follow it as spec. Do not improvise against named constraints.

AUTONOMOUS mode: Dave says "make this great," "your best shot," "brainstorm and ship," or equivalent. Read this design system, identify the slide's strategic role, synthesize one strong concept, generate it, deploy it, and report what changed and why. Do not return a menu of options unless Dave explicitly asks for options.

Every prompt must include: slide role, strategic argument, composition/quiet-zone instruction, palette, style, and banned aesthetics.

## Slide Type Matrix

| Slide type | Treatment |
| --- | --- |
| Opener | Full-bleed mythic editorial painting; thesis type in quiet zone; universal human truth before wedge. |
| Mission | Full-bleed or near-full-bleed big human/network image; sparse type; emotional scale. |
| Problem | Editorial typographic structure, selective metaphor imagery only if it clarifies the pain. |
| Solution | Clean product/category frame; can mix diagram and restrained visual metaphor. |
| Market | Structured typographic/data treatment; no painterly hero unless it is a transition beat. |
| Traction | Data-first; faces or venue images only if they make proof more legible. |
| Ask | Clean, direct, investor-readable; avoid decorative imagery. |
| Transition | Full-bleed or monumental type; one conceptual turn per slide. |
| Comparison | Split editorial layout; strong contrast; no nested cards inside cards. |
| Data | High-contrast, scan-friendly charts/tables; preserve numeric trust over atmosphere. |
| Closer | Full-bleed or monumental brand image; emotional aftertaste; minimal words. |
