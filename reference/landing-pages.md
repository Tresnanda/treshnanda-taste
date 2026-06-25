# Reference — Landing Pages

Use when building a marketing / landing page, hero, or marketing section (SaaS, consumer, agency).

## Hero layout — pick ONE architecture (THIS is what builds get wrong)
The hero visual is an **architectural ZONE**, not a small contained card. The texture either **fills a whole half and bleeds to the viewport edges**, or **is the entire background**. Pick one:

**A. Asymmetric split** (most common — Luma, Gamma, Verdant). The page splits into two big zones:
- a **text zone** on the plain dotted off-white canvas (eyebrow pill → big mixed-script headline → one-line sub → CTA row → trust avatars), and
- a **texture zone** — a large shader/photo panel that **FILLS its ~45–50% half and bleeds to the top, outer, and bottom viewport edges.** It is big, rectangular, architectural. Round only the *inner* corner, if any. A product/app UI may float OVER it, half-cut-off.

**B. Full-bleed atmospheric** (Andy, Sync, Lucen, Verdant-full). The **entire hero background IS the texture** — edge-to-edge nature photo / painterly art, or a dark charcoal field with ONE radial glow (amber rising from the bottom, blue arc from the top). Floating pill nav + centered headline + CTA sit ON it; a product mock floats at the bottom, half-cut-off; trust logos along the bottom.

**C. Minimal centered** (Neura). Off-white, floating pill nav, a centered headline with generous air, ONE faded accent element (e.g. a greyed icon grid), a single CTA, trust logos at the bottom. Restraint is the design.

**THE ANTI-PATTERN (keeps happening — do not):** rendering the hero visual as a **small contained, rounded, (cursor-)tilted card** sitting in a grid column with margins around it, a tiny app-mock nested inside. That's an *app/element* instinct, NOT a landing layout. On a landing page the texture is a **bleeding half-zone or the background** — big and architectural — never a floating widget. (If you show a product UI, it's a *static* screenshot floating OVER the texture and half-cut-off by an edge, not a tilted card you nest a mock inside.)

## Page structure & rhythm
- **Nav = floating pill**, top-center or top-left, detached (margin all around): logo + 3–5 links + one dark/accent CTA. NEVER a full-bleed bar overlapping hero content.
- **Calm section rhythm** — one idea per band, big vertical breathing room. At least 4 different layout families across the page; never repeat a section layout back-to-back.
- **Whitespace is intentional counterweight** — a blank quadrant balances a heavy texture zone; it's never "ran out of content."
- **Trust-logo row** — quiet, monochrome, directly under the hero (its own band), never inside the hero copy row.

## Signature moves
- **Warm off-white canvas + ONE rationed accent** (grass `#2FBF6B`, blue `#2E7DF6`, orange `#F26B2A`, violet `#7C5CFC`). Never a rainbow on the chrome.
- **The textured surface IS the centerpiece** — a big bleeding shader/photo zone (see layout above), grainy + saturated + directional with a focal glow.
- **Mixed-script display headline** — big near-black headline where ONE phrase switches to accent color, an *italic serif*, or a highlighted pill-tag word with a tiny inline glyph.
- **Squircle + pill everything** — pill nav, pill buttons, ~24px cards in the body. No sharp 4px corners.

## Color & palette
- Canvas (light): warm off-white `#F2F1EE` / `#F4F3F0` (not pure `#FFF`); often a faint dotted grid on the text side.
- Ink: charcoal `#1A1A1A`–`#222` for headlines + primary buttons; body grey `#6B6B6B`. One saturated accent per page.
- Dark: charcoal `#161616`–`#1E1E1E` (not black); dark heroes get ONE radial glow, single light source, deep falloff. Dark is a first-class twin.

## Surfaces — gradients / shaders / imagery (make-or-break)
- A gradient MUST be **saturated, directional, multi-stop MESH with a focal bloom, and carry film grain.** If it could be a Tailwind `from-purple-100 to-blue-100`, it's slop.
- Or **real / painterly nature imagery, edge-to-edge** (golden-hour, atmospheric, real depth-of-field) with a bottom scrim for legible white text. Never stocky.
- The texture is big and architectural (a half or the whole bg) — not a small accent.

## Typography
- Geometric/grotesk sans; headlines large + heavy + near-black, ~2 lines, tight leading. Restrained body, one short sentence.
- Signature accents: italic-serif swap mid-headline; highlighter pill-words (soft colored chip + tiny glyph); accent-color word swap.
- Stats: big tabular metric + tiny grey label.

## Shape, radius & depth
- Body cards ~24px squircle; pills on nav/buttons/badges. Soft, low, diffuse shadows (`0 20px 40px rgba(0,0,0,0.06)`). Hairline borders ~6–10%. Glass only on overlay panels.

## Components
Pill nav · dark primary pill (often `→`/`↗`) + ghost secondary · eyebrow/tag pill above headline · body feature cards (mini visual + bold title + one grey line) · `+18%` green stat deltas · static product screenshot floating over the texture, half-off an edge · monochrome trust-logo strip · small rounded app-icon tiles inside body cards.

## Premium vs slop
**Premium:** ONE rationed accent · warm off-white canvas · the texture as a big *bleeding architectural zone* or full-bleed bg · grainy directional saturated gradient (or real imagery) · calm composition with counterweighted negative space · floating pill nav · dark mode as an equal twin.

**Slop to avoid:** the **contained tilted card hero** (the recurring miss) · pale evenly-lit grain-free gradient blobs · text-on-flat-tint hero with no texture · nav colliding with hero text · over-stuffed maximalism / multiple bright colors · pure `#FFF` + pure black + sharp corners + hard shadows.

**One-line rule:** *warm dotted canvas + ONE accent + the texture as a big BLEEDING half-zone or full-bleed background (never a contained tilted card) + a mixed-script headline + floating pill nav + calm one-idea-per-band sections.*
