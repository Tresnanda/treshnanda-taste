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

## Visual language (the look — confirmed across 33 references)
Their aesthetic is *consistent*, not per-brief. This is the universal look.

**Canvas & color**
- **Off-white / warm-grey canvas** (~`#f0efed`), not pure white. Often a subtle **dot-grid** texture on flat panels.
- **Pastel, soft, light — never neon.** ONE minimal accent per product (green / orange / blue / violet), used sparingly.
- **"Ink"** (near-black, e.g. `#1f2024`) for primary text + CTAs — pure, no warm tint.
- Ship **both light and dark.** Dark = charcoal/near-black (or a true-black hero with a single colored radial glow), same pastel + shader treatment — **never a flat grey dark mode.**

**Surfaces — texture over flat (their signature move)**
- Where a default reaches for a solid fill or CSS gradient, **reach for a real shader/generative gradient**: mesh gradients, vertical-blur, dithered halftone, grainy gradients — ShaderGradient / Three.js / WebGL / Framer-shaders style, usually with subtle **grain/noise**.
- **Nature photography & painterly illustration** as emotional surfaces — meadows, mountains, clouds, sunsets. Calm, aspirational, fresh; slightly grainy when illustrated.
- **Glassmorphism** for floating overlays (frosted blur + a top highlight).

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
Their loudest signal. **"A LOT of animations and microinteractions"** is a literal, repeated instruction.
- **Every interaction earns motion** — "all the small things that make the user feel praised / congratulated / welcomed" — PLUS **big WOW setpiece moments.**
- **Motion does the work** — "the animation should be the #1 worker" of making something *feel* like what it is.
- **Disney impact lands hardest:** anticipation → squash/stretch on impact → follow-through/overshoot. The "stamp of approval" (badge slam + card squash + shockwave + particles) earned *"AMAZING BRO FUCK YEAH."*
- **Three layers, always** (primary + secondary + ambient). Flat = unfinished.
- **Crossfade + BLUR**, never a bare crossfade. (Watch WebKit: end at `blur(0.01px)` + `will-change` to avoid flicker on large surfaces.)
- **Snappy. No input lag from motion** — typing/keyboard stay instant.
- **Commit fully.** Timid motion that "barely moves" reads as "off." Big, decisive, springy. Spring physics for "alive."
- **Signature setpieces that landed:** kinetic typography (char-by-char), zoom-through "camera" beat transitions, materialize-from-light, 3D tiltable cards w/ cursor spotlight, a card-as-character through-line, a self-playing looping demo (type → stamp → repeat).
- **Drag-out must feel like *taking/grabbing*** the element — zero "separation." Winning effect: the content **"pops" out of the row** (*"OMG THATS IT"*). Style = **ghost + bounce/pop**, never a tilted remnant.
- **Onboarding** must be fun, tasteful, feel good, and *memorable* — unique experiences and a story, never a plain slideshow.
- Bar = **Awwwards-tier.** When they say "still not good enough, we want ANIMATIONS," add a *signature moment*, not more polish.

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
