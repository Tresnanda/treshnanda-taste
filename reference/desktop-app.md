# Reference — Desktop App

Use when building a desktop application UI: dashboard, multi-pane app, sidebar, command palette, settings.

## Signature moves
- **The floating inset app window** — the whole app is one large rounded panel (~20–28px radius) floating on a flat, slightly-darker canvas with a generous outer margin (~24–48px). The gap around it IS the design (the "two-card" feel at the top level).
- **Functional surfaces stay clean; gradients are quarantined to ONE hero object** — ~90% of pixels are neutral white/charcoal panels with crisp data. Saturated shader appears in exactly one place per screen (a feature thumbnail, a billing banner, an empty-state, a highlighted insight). Never washed across the UI.
- **Generously rounded shell, dense core** — outer window ~24px, cards ~16–20px, pills 999px, inputs ~10–12px; yet type inside cards is small and dense.
- **One accent, decisive** — a near-black primary button + ONE chromatic accent (Finexy orange `#F0531C`, coral `#F2685E`, green `#18C964`). Status dots are the only place multiple hues appear.
- **Pill segmented nav in the header** — tabs inside a rounded pill container, active tab a solid black (or white-on-dark) filled pill; search is a long pill; icon buttons are circles.

## App shell & layout
- **Three-pane for content apps** (inbox/CRM/tasks): icon+label sidebar rail → list column → detail pane, separated by thin low-contrast hairlines (NOT heavy borders or big gaps); each scrolls independently.
- **Dashboard = bento of rounded cards** on the inset window, ~16–20px gaps, grouped by function; no card touches the window edge; consistent inner padding (~24–32px).
- **Sidebar** ~200–240px, sectioned with tiny muted labels; items icon + label ~13px, ~36–40px rows; active = soft accent-tinted pill (accent bg ~8–12% + accent text), NOT a heavy fill. Collapsed = centered icons in a ~56px rail.
- **Density**: body ~13–14px, labels ~11–12px, big bold figures only for the key metric; tables ~44px rows, 5–8 visible.
- **Separation hierarchy**: (1) window radius + canvas gap; (2) card radius + gap; (3) hairlines for rows/panes. Almost no heavy borders.

## Color & palette
- Light: canvas warm/cool grey `#EFEFEF`–`#F4F4F5` (sometimes faintly accent-tinted); window/cards `#FFFFFF`/`#FCFCFC`; hairlines `#ECECEC`; text `#16181C` / `#6B7280` / `#9CA3AF`; primary button black `#111`.
- Dark: canvas `#0A0A0B`–`#141414`; panels `#1A1A1D`–`#1F1F22` (one step lighter than canvas = the elevation); hover `#26262A`; hairlines `#2A2A2E`; text `#F5F5F5` / `#A0A0A8`; selected card gets a 1px accent ring.
- Status dots: green `#22C55E`, amber `#F59E0B`, rose `#EF4444`, blue info.

## Surfaces — gradients / shaders
- **Where they live**: feature-post thumbnails, the "current plan" billing banner (the hero of an otherwise flat settings page), integrations empty-state banner, one highlighted insight card.
- **Style (make-or-break)**: RICH, saturated, multi-stop shader with real color travel (blue→teal→magenta, indigo→violet→amber), a glossy/liquid 3D quality (baked-ShaderGradient look), often a soft diagonal light sweep. "Soft" means *smooth transitions*, NOT desaturated.
- **Quarantine it** to ONE rounded card so it reads as a jewel, not wallpaper; keep the rest neutral.
- No nature photography here; imagery = real circular avatar photos + brand logos. Abstract shader substitutes for hero imagery.

**Avoid:** pale low-saturation two-stop linear ramps with a blur · gradient bled across the whole background · uniform blur as a substitute for real shader depth.

## Typography
- Clean grotesque sans (Inter/Geist/SF-like), no serifs.
- Scale: greeting ~28–32px semibold; big data figures ~28–36px bold; card titles ~15–16px medium; body/labels ~13–14px; meta ~11–12px.
- Weights mostly Medium/Semibold; big numbers Bold; no thin weights.
- Hierarchy via size+weight+color, not boxes. **Tabular numbers everywhere** for money/stats/dates; deltas with up/down arrows + green/red.

## Shape, radius & depth
- Radius ladder: window 20–28px → cards 16–20px → inner/inputs 10–12px → pills/chips 999px → avatars circles.
- Depth is whisper-soft: shadows large/low-opacity/neutral (`0 8px 24px rgba(0,0,0,0.04–0.06)`), only to lift the whole window or a popover; inner cards often have NO shadow (fill + radius + gap separate them). Dark mode = near-zero shadow; elevation via lighter-charcoal panels.
- Hairlines over borders; selected = soft tinted fill or thin accent ring, never a 2px hard border. No glass as a primary surface.

## Components
Nav items (lucide-style stroke icon + label, active = tinted pill) · top segmented pill nav + accent rounded-square logo tile · search/command pill with `⌘K`/`⌘F` hint chip · tables (tiny grey caps headers, ~44px rows, leading checkbox, app icon + name, right-aligned tabular amounts, dot+label status pill, trailing `⋯`; hairlines, no zebra) · status pills (dot + text, tinted-soft) · soft grey tag chips · buttons (black pill primary / grey or hairline-outline secondary; circle icon buttons) · circular real-photo avatars in stacked clusters · pill toggles · mini card-art objects (credit cards) · clean two-tone bar/line charts + sparklines, no chartjunk.

## Premium vs slop
**Premium:** restraint + one decisive accent · the single saturated shader as a focal jewel against neutrals · consistent radius ladder + consistent icon weight · real tabular data, real avatars, real density (looks like a working product) · floating inset-window framing · soft tinted-pill active states.

**Slop to avoid:** pale desaturated two-stop gradients with blur · gradient washed across the whole bg · rainbow of accents · colliding nav/elements with no grid · empty-space maximalism OR over-stuffed clutter (aim dense-core/soft-shell) · heavy shadows + 2px borders · uniform mid-grey text at one size · mobile-sized fonts blown up.

**One-line rule:** *inset rounded app-window on a neutral canvas + disciplined panels/hairlines + ONE saturated shader jewel + one accent + a real size/weight/color hierarchy with bold tabular numerals — desktop density, whisper shadows, tinted-pill active states.*
