---
name: treshnanda-taste
description: Treshnanda's personal UI/UX taste profile — soft, premium, pastel, shader-textured, generously-rounded surfaces with bold, kinetic, Awwwards-tier motion. Invoke when building or redesigning ANY app or website UI, designing animations/microinteractions, or making layout/visual/copy decisions — and whenever Treshnanda references "their taste," "high taste," "premium," "feels good," "magic," or "make it WOW."
---

# Treshnanda's UI/UX Taste

Distilled from building quickboard (a premium macOS app) through hundreds of iterations, plus 33 hand-picked reference designs. Apply it to any app or website. The bar is always the same: **high taste, premium, feels good, and motion that makes people go "WOW."**

## Foundation — invoke these two skills FIRST, every time
This is the *personal taste* layer. It sits on top of two craft skills Treshnanda invokes on nearly every UI task — so **whenever this skill is active, automatically invoke `emil-design-eng` and `motion-design` too, without being asked.**
- **`emil-design-eng`** — craft micro-decisions: custom easing, springs, scale-on-press, blur-to-mask, concentric radii, never-scale-from-0.
- **`motion-design`** — motion theory: three layers (primary/secondary/ambient), Disney principles, personality archetypes, choreography, timing tables.

Order: **load both craft skills → then apply this taste lens on top.**

## The quality bar (grade by their words)
- Praise (on target): **"high taste," "premium," "tasteful," "feels good," "magic," "WOW," "awwards-tier," "unique," "FUCK YEAH."**
- Reject (fix it, don't defend it): **"off," "weird," "ugly," "ai slop," "not premium," "bare," "too subtle," "doesn't feel like magic," "not good enough."**
- **"Premium" is the constant target.** They will keep asking *"why doesn't this feel premium?"* until it does. Chase the *feeling*, not just correctness.
- **Magic / memorable / unique beats clean.** Polished-but-conventional reads as "not enough." If it could be any app, it isn't done.

## How they work (process)
- **Build directly. Relayout, don't reskin.** They distrust plan-first/reskin flows: *"im trusting your raw power."*
- **References = layout, not styling — by default.** Take the structure, not the fonts/colors — **UNLESS they explicitly say "copy this."** Then match it exactly.
- **Iterate fast off screenshots.** They paste a screenshot + "this is off / fix this / feels weird." *Feel* it and fix it; don't explain it away.
- **Give the why, verified** with current best practice. They say **"revert"** when something regresses — keep diffs reversible, never silently lose a thing they liked.

## Visual language (the look — confirmed across reference designs)
Their aesthetic is *consistent*, not per-brief. This is the universal look.

**Before building a specific surface, READ the matching file in `reference/` first** — each has the concrete, category-specific recipe (approximate hexes, radii, proportions) + its own premium-vs-slop guardrails:
- Landing page / hero / marketing → `reference/landing-pages.md`
- A single card / widget / modal / component → `reference/elements.md`
- Desktop app / dashboard / multi-pane UI → `reference/desktop-app.md`
- Mobile screen / iOS widget → `reference/mobile-app.md`

The sections below are the shared base all four build on.

**Canvas & color**
- **Off-white / warm-grey canvas** (~`#f0efed`), not pure white. Often a subtle **dot-grid** texture on flat panels.
- **Pastel, soft, light — never neon.** ONE minimal accent per product (green / orange / blue / violet), used sparingly.
- **"Ink"** (near-black, e.g. `#1f2024`) for primary text + CTAs — pure, no warm tint.
- Ship **both light and dark.** Dark = charcoal/near-black (or a true-black hero with a single colored radial glow), same pastel + shader treatment — **never a flat grey dark mode.**

**Surfaces — texture over flat (their signature move, and the #1 place builds turn to slop)**
- Where a default reaches for a solid fill or CSS gradient, **reach for a real shader/generative gradient** (ShaderGradient / Three.js / WebGL / Framer-shaders / mesh / dithered-halftone). **A gradient MUST be: (1) saturated and committed to its hue, (2) directional with a clear focal light source / bloom, (3) a multi-stop MESH, not a 2-stop ramp, (4) carrying visible film grain / noise.** Quarantine it to ONE focal object; keep everything else neutral so it reads as a jewel, not wallpaper.
- **The test:** if the gradient could be mistaken for a Tailwind `from-purple-100 to-blue-100`, it is slop — saturate it, give it a light source, add grain, or replace it with real photography. **A pale, evenly-lit, grain-free blur is the single most common slop tell** (it's what sank the first test build).
- **Nature photography & painterly illustration** as emotional surfaces — meadows, mountains, clouds, sunsets, golden-hour, real depth-of-field. Calm, aspirational, fresh; never stocky or CGI. On photo cards, fade the bottom to a color *sampled from the image*, not black.
- **Glassmorphism** for floating overlays only (frosted blur + a top highlight) — a garnish, never the whole surface.

**Shape & depth**
- **Generously rounded** everything; strong **iOS-widget squircle** language for self-contained cards.
- **Pills** for buttons, nav, tags, status badges, filter chips. **Floating pill nav** (active item = an ink pill).
- **Soft, diffuse shadows** (floating-card-on-off-white) + a 1px hairline ring.

**The signature card: image/shader header + content panel**
- The dominant pattern across the refs: a card whose **top is a shader or photo** and whose **bottom is a clean white/ink info panel** — flights, real estate, trails, widgets, onboarding, pricing, modals all use it.
- Variant: a photo **fills the card and fades into a solid color** (green/dark) with white text overlaid.
- **Card-on-card / merged shapes:** nested cards (white outer → photo inner → info panel), and the "two regions, one continuous silhouette" widget shape (a panel with a notch/tab cut). **The card IS the object** — don't slap an icon on it when the card already is the icon.

**Typography**
- Big bold sans for most (SF Pro-ish), tight tracking.
- Signature display treatment: **mixed serif-italic + sans** headlines (a playful editorial mix), with **colored rounded-rect "tag" highlights** boxing key words.

**Components & details**
- Recognizable **app/brand icons as small rounded tiles** (integrations, agent cards).
- Small colored **% pills** for stats (+18%); **circle-check checklists** for "what you get" / onboarding.
- **Ghost + ink button pairs** (secondary ghost pill / primary ink-or-accent pill).
- Colorful rounded **avatars**. **Icons, not emoji**, in the UI.

**Mood:** premium, calm, soft, optimistic — modern SaaS *with personality*. Never brutalist, never cluttered, never dark-tech-hacker, never AI-slop.

## Motion & animation (the heart of it)
Their loudest signal — **"a LOT of animations, microinteractions, *micro*animations."** But the goal is precise: make the product feel **alive**, under one hard constraint — **alive, never *in the way*.** Motion should be *felt* on almost everything, yet never block, gate, delay, or distract from what the user is actually doing. The target isn't "more motion," it's **"more *life*, zero friction."**

**Two registers — always run both:**
1. **The alive layer — abundant, tiny, non-blocking.** Pervasive micro-motion + ambient life on nearly everything: hover responses, press/tap scale, focus glows, **idle float / breathing / gentle gradient drift**, micro-feedback on every action, smooth state + layout transitions. Fast (~100–200ms), interruptible, *off the critical path*. **The ambient/idle layer is the secret to "alive"** — it's passive and in the background, so it adds life without ever obstructing.
2. **The WOW layer — rare, earned setpieces.** The big, infrequent moments (an important confirmation, onboarding, a milestone). Full Disney impact: anticipation → squash/stretch → follow-through/overshoot — committed and dramatic. Rarity is what *earns* the drama. **Which** setpiece you build depends entirely on the product (see the palette below) — **never transplant one product's signature moment into another.**

**The golden rule — never disturb usage:**
- **Frequency scales motion:** the more often something is seen/done, the *shorter and subtler* it gets (down to near-instant for repeated/keyboard actions). 100×/day → barely there; once → a setpiece. This is exactly how "a lot of motion" and "not disruptive" coexist — the *volume* comes from the ambient + micro-feedback layer, **not** from slowing down the things people do constantly.
- **Never block, gate, or delay input.** Typing, clicking, keyboard nav stay instant; a reveal/stagger must never make the user wait to act. **Interruptible** — a flicked or redirected motion keeps its velocity, never "finish first."
- **Never distract during a task** — no looping attention-grabbers beside where the user is working; nothing that re-triggers annoyingly on every pass.
- **Snappy. No input lag from motion.** Always honor `prefers-reduced-motion`.

**Craft (how, not whether):**
- **Motion does the work** — it should be the #1 thing making an interaction *feel* like what it is (opening feels like opening; discarding feels like discarding).
- **Three layers, always** (primary + secondary + ambient). Flat = unfinished.
- **Crossfade + BLUR**, never a bare crossfade. (WebKit: end at `blur(0.01px)` + `will-change`.)
- **Commit fully** — timid motion that "barely moves" reads as "off." Spring physics for "alive," with real overshoot reserved for the rare big moments.
- **Setpiece palette to reach for** (pick what fits the product; never force one): kinetic / char-by-char typography, materialize-from-a-point-of-light, shared-element / morph transitions, 3D tilt + cursor spotlight, zoom-through "camera" moves, a celebratory impact-confirmation (anticipation → slam/squash/flash → settle), a self-playing looping demo. **A setpiece must fit the product's purpose and register** — a focus-timer hero does not need a save-stamp; a calm reading app does not need confetti.
- **Drag-out should feel like *taking the real thing*** — when an element stands for a file / image / value, dragging it out should feel like lifting that thing out of its place (it emerges from its slot), not a detached ghost spawning on the cursor. Settle with bounce/pop; no tilted remnant.
- **Onboarding** = fun, tasteful, memorable, a *story* — never a plain slideshow.
- Bar = **Awwwards-tier.** "Still not good enough" → add ONE signature moment that *fits the product*, not more motion everywhere.

### Shared motion vocabulary
Treshnanda describes motion with a precise glossary (terms like *shared element transition, morph, rubber-banding, stagger, origin-aware, follow-through, squash & stretch, crossfade, layout animation, idle / float, momentum, asymmetric easing*). **The full glossary is in `animation-vocabulary.md` — read it when interpreting a motion request or proposing motion.** When they name a pattern, build exactly that; when you propose motion, name it with these terms so you're speaking the same language.

## Copy
- **No em dashes. No emoji.** Clean, plain, confident sentences.

## UX correctness (they care a lot)
- **Must make sense for a real, first-time user.** They catch logic holes: *"a new user's board is empty," "a new user doesn't have an environment."* Design the real empty/entry state.
- **Keyboard ↔ mouse arbitration done right.** Default to the top item with keyboard nav; a stationary cursor must not hijack selection; rows scrolling under the cursor must not jump it. Last *intentional* input wins.
- **Spotlight/Raycast behaviors:** dismiss on click-away; non-activating panel for global summon; mouse-first but fully keyboard-capable.
- **Cover every scenario** — confidential items, multi-select mixes, cancel-a-drag. Reference real best-in-class apps (macOS Paste, Spotlight, Raycast, Arc, Linear).

## The "never" list
Flat default fills (use a shader) · pure-black dark mode (use charcoal) · neon/LED color · generic left-accent indicators, stock dropdowns, AI-purple glows, three-equal-cards (all read as AI slop) · square-everything (round it) · timid/half-committed motion · bare crossfades (always blur) · em dashes · emoji in UI · reskin-without-relayout.

## Case study: quickboard (one expression — DON'T copy the specifics)
For a premium macOS desktop *clipboard utility*, the DNA expressed as: a "Soft Paper" pastel palette + ink `#1f2024`, baked ShaderGradient card surfaces, **items as list rows** (not cards), **"environments"** as workspaces, a Spotlight-style **summon** panel + floating **tray**, denser/smaller **desktop** fonts, the stamp-of-approval + pop-from-row animations. The IA and feature-shapes there are *app-specific* — take the instincts, not these decisions. (e.g. a marketing site or a mobile app gets bigger type, more whitespace, and totally different IA — but the same soft/pastel/shader/rounded *language*.)

---

**When in doubt:** make it softer, more textured (reach for a shader, not a flat fill), more rounded, and *far* more animated — then ask *"does this feel premium and magic?"* If not, it isn't done.
