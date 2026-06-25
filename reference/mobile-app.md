# Reference — Mobile App

Use when building a mobile app screen or an iOS-style widget / card.

## Signature moves
- **The merged squircle "card-with-a-shelf"** — one rounded-rect silhouette split into two tone regions: a saturated/dark/photo top zone (balance, headline, image) continuing seamlessly into a lighter zone below (CTA, stats). One object, two materials; corners only on the outer hull, the internal seam is straight. THE hero shape.
- **One loud accent against a near-neutral world** — each screen commits to a SINGLE punchy hue (acid-lime, electric-violet, signal-red, warm-coral) on ONE element, surrounded by off-white/charcoal. Never two competing brights.
- **Oversized editorial display type as the focal point** — giant `$521,098.31`, serif `PARIS`/`BOOKS`, big 78%/33% stats. Type IS the hero.
- **Real texture, never flat fills** — dithered halftone renders, real landscape/food/book-cover photography, baked soft-cloud gradients. Every "empty" surface earns its keep.
- **Pill-shaped everything floating on roomy canvas** — buttons, segmented toggles, status chips, avatar rows, floating bottom tab bars, all generously spaced.

## Layout & composition
- **Structure**: light status bar → text header (small label + big display number/title) → hero card / merged widget → horizontal scroller (avatars / chips / cards) → list section ("History", "Upcoming") → floating bottom tab bar.
- **iOS-widget card language** — fat self-contained squircles with a mini-label top-left and value/CTA bottom; cards sit ON the canvas with ~16–20px gutters, not edge-to-edge.
- **Generous density** — big touch targets (44px+), tall list rows (avatar + two-line text + trailing value), lots of vertical air. Never cramped.
- **Floating tab bar** — 3–5 icons detached from the bottom edge, active icon in a filled accent circle.
- **Headers minimal** — back-arrow / small centered caption / trailing circle icon button; the title lives BELOW in big type, not in the bar.

## Color & palette
- Light canvas: warm/cool off-white `#F2F3F4`–`#F7F7F8`, sometimes tinted (peach `#F3E9E6`, sage-grey). Never pure flat `#FFF`.
- Dark: true near-black `#0E0E0E`–`#1A1A1C` cards/canvas; elevated surfaces a notch lighter `#222`. Accent stays vivid on black.
- Accents (ONE per screen): acid-lime `#C6F24E`, electric-violet `#6C4CF0`→`#8B5CF6`, signal-red `#E8412E`, warm-coral `#F26B3A`; soft pastel secondaries (butter `#F4E3A1`, sky `#9FE0E3`, lilac `#E9D5FF`) for chips only.
- Text: `#111` on light; `#FAFAFA`/`#9A9A9A` on dark.

## Surfaces — gradients / shaders / imagery (CRITICAL)
- **Saturated + directional + focal light source** — e.g. a deep violet→indigo diagonal with a brighter top-left bloom; a warm coral cloud-gradient with a *hot center* blooming into cream. Like a real ShaderGradient bake, NOT a CSS linear-gradient.
- **Grain / texture present** — subtle grain on gradients; explicit dithered halftone/point-cloud renders. Texture = premium signal.
- **Real photography is load-bearing** — landscapes, Eiffel Tower hero, actual book-cover art as the whole grid, real plated food. Imagery provides the color; chrome stays neutral around it.

**Failure mode:** pale, evenly-blurred pastel gradients with no focal point, no grain, no direction (the characterless AI blur). If a gradient has no hot-spot and no grain, it's wrong. Also avoid crisp-flat vector blobs masquerading as texture — use real grain/halftone/photo only.

## Typography
- **Extreme scale contrast** — tiny caption labels (~11–13px, muted, sometimes uppercase-tracked) against huge display values (40–64px). The contrast IS the hierarchy.
- **Big-number/money treatment** — balances/percentages are the largest thing on screen (weight 600–700), smaller superscript currency symbol, de-emphasized decimals, tabular figures for list alignment.
- **Display serif accents** — high-contrast serif (Playfair/Canela-like) for titles like `PARIS`/`BOOKS`, against geometric-sans body.
- Mixed-weight inline emphasis ("your overall score is **above average**").

## Shape, radius & depth
- Large radii: cards ~24–32px squircle, pills full (radius = half-height), avatars circles, inner tiles ~16–20px.
- The two-region one-silhouette widget (outer hull rounded, internal seam straight) is the cornerstone shape.
- Soft, low, diffuse shadows (large blur, low opacity, ~8–16px y) — gentle lift, NOT hard shadows or neumorphism. Stacked offset cards for depth. Glass only over imagery.

## Components
Segmented pill toggles (active = filled pill) · status chips ("Available", "⭐ 4.5", "Main card") · floating accent-circle tab bar · big time/number display widgets · overlapping avatar rows + `+N`/`+ Add` · thin consistent-stroke line icons in circle buttons (icons stay crisp even over textured surfaces) · the merged-panel widget with its CTA inside the colored region.

## Premium vs slop
**Premium:** commit to ONE saturated accent, let neutrals + imagery carry the rest · gradients with a real focal light source + grain, OR real photography · extreme type-scale contrast (giant numbers/serif titles as hero) · generous spacing, fat squircle radii, soft diffuse shadows, floating pill tab bars · the two-region merged-squircle hero card.

**Slop to avoid:** pale evenly-blurred pastel gradients with no focal point/grain (the #1 failure) · every surface a flat tint, no imagery · uniform mid-size type with no clear hero · multiple competing brights / cramped rows / too many cards fighting · hard heavy shadows, timid radii, edge-to-edge cards with no breathing room · crisp-flat vector blobs pretending to be texture.

**One-line rule:** *fat squircle cards on a roomy off-white-or-charcoal canvas + ONE saturated accent + a merged two-region hero card carrying a real photo or grainy directional gradient + extreme-contrast type (giant numbers / serif titles) + floating pill tab bar.*
