# Reference — Elements (cards, widgets, modals)

Use when building a single standalone component: a card, widget, modal, popover, or small self-contained piece.

## Signature moves
- **The "header-lid + info-drawer" split** — a short textured/photo/shader header on top; a solid info panel tucks UNDER it with a small step/notch (like a manila folder tab or an iOS widget whose content drawer peeks below the image). This nested z-stack is THE most repeated move.
- **Squircle everything, generously** — continuous-curvature cards ~20–36px, fully-pill buttons; inner elements echo the outer radius concentrically.
- **One real photo or one real shader per card — never a flat fill.** The image carries personality; the rest of the card is calm neutral around it.
- **Calm neutral chrome around exactly ONE vivid focal point** (the photo, the shader header, the green analytics bar, the accent button). Restraint is the premium signal — not rainbow dashboards.
- **Light + charcoal-dark shown as twins**, both fully resolved.

## The card anatomy (three dominant patterns)
1. **Header-lid + info-drawer** (most common): top ~35–45% is the textured/photo/shader lid; a solid panel (white / `#1A1A1A`) tucks under it with a small offset step; title top-left of the drawer; a big number anchors a bottom corner ("05 Doc / 1270 Notes", "9:30 AM").
2. **Full-photo card + gradient-fade-to-color overlay**: one photo fills the whole card; bottom third darkens via a scrim **tinted to a hue sampled from the image** (olive, forest, warm-brown); white title + grey subtitle + icon-stat pairs (Bed/Bath/Sqft) on the scrim; pill price chip + full-width rounded CTA at the bottom.
3. **Inset modal / popover**: background app desaturated/blurred; crisp white-or-charcoal rounded modal floats centered with a soft shadow; inside = small photo banner → title → one-line description → checklist of labelled icon-rows → two-button footer (ghost "Close" + filled dark/accent primary).

Padding ~16–24px, text left-aligned, CTAs full-width or bottom-anchored, stat columns evenly spaced with hairline dividers.

## Color & palette
- Light canvas: warm off-white `#EDEDED`–`#F4F2EE`, sometimes a tinted wash (peach `#FBE9DE`, lilac `#EFEBF4`) echoing the shader. Card surface near-white `#FFFFFF`–`#FCFBF9`.
- Dark canvas: charcoal `#0E0E10`–`#1A1A1A` (not navy). Card `#1C1C1E`–`#222`; nested rows `#2A2A2C`.
- Text: ink `#1A1A1A` / pure-white; secondary `#8A8A8E`; tertiary `#B0B0B0`.
- Accents (one per card, saturated): iOS blue `#0A84FF`, success green `#34C759`/`#5FA044`, the signature warm peach→coral→lilac→periwinkle gradient. Bitcoin-orange / AI-violet only when the content demands it.

## Surfaces — gradients / shaders / imagery (where slop dies)
- **Mesh blooms, not linear washes** — multi-stop with a clear focal light source (a bright bloom in one quadrant fading through 3–4 hues).
- **GRAIN is mandatory** — visible film grain / noise dithering over nearly every shader. This is the single biggest separator from AI-slop; it kills banding and adds paper/print texture.
- **Saturated + directional** — real chroma, a sense of light direction. NOT the washed-out evenly-pale centered radial blur.
- **Color-tinted dark scrims** sampled from the photo (text sits on a color that belongs to the picture).
- **Art-directed photography** — golden-hour, natural light, real depth-of-field bokeh; never stock-flat or CGI.

**Failure test:** if a card has no image AND no grainy directional bloom, it has already failed.

## Typography
- System/SF-family grotesque sans. Title 16–20px semibold ink → description 13–14px grey → labels 11–12px grey, sometimes ALL-CAPS tracked for section heads.
- **Oversized hero numerals** as the anchor ("$125,824.36", "9:30 AM"), tabular figures, unit/symbol set smaller and lighter beside.
- Mixed-weight inline emphasis in casual copy ("start **delegating tasks**, now go **carpe diem**").

## Shape, radius & depth
- Squircles: cards ~20–32px, app-icon-tile widgets ~28–36px, modals ~20–24px; buttons full pills. Nested radius echoes the parent.
- Shadow: soft, low, wide, single (`0 20–40px 60px rgba(0,0,0,0.06–0.12)`). In dark, depth comes from a hairline + the lid/drawer overlap, not shadow.
- Hairlines 1px `rgba(0,0,0,0.06)` / `rgba(255,255,255,0.08)` between stat columns and rows.
- **Chunky white "tray" bezel** (~8–12px) wrapping inner dark content gives a physical iOS-widget feel.
- Glass sparingly — frosted pills/headers over imagery, not whole-card glass.

## Components
Filter/status pills (solid-dark = selected, white/outline = not) · `+18%` green percentage badges (often `label | value`) · app-icon tiles (Slack/Notion/Figma/WhatsApp) floating on the shader header · overlapping avatar clusters + `+N` · status dots · segmented/paired controls · monoline outline icons (consistent stroke) · primary filled-dark/accent pill + ghost-outline secondary · tiny route/sparkline graphics (one highlighted green bar + a dot on a dashed avg line).

## Premium vs slop
**Premium:** a real focal image or grainy directional saturated shader · ONE color event per card, rest neutral · the layered lid/drawer z-stack + chunky white widget bezel for tactile depth · oversized tabular numerals + tiny labelled captions · squircles + soft single shadow + hairlines · light/dark as deliberate twins.

**Slop to avoid:** pale evenly-lit gradients with no focal light / no grain · a card that's all flat fills + text (no image, no real shader) · too many competing accents · centered-everything with equal weights and no anchor · tight corners / heavy shadows / navy-blue "dark mode" · glass on everything.

**One-line rule:** *squircle card + ONE vivid surface (real photo or grainy directional mesh) + calm neutral chrome + oversized tabular numerals + a layered lid/drawer or photo-scrim, in true light or charcoal — if the surface is a pale flat gradient with no grain and no photo, redo it.*
