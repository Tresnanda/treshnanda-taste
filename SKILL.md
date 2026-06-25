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

## Visual language — RESET (being remade)
The visual / aesthetic layer is intentionally **blank** right now. The previous canvas/color, surfaces, shape, typography, layout-architecture guidance and the per-context `reference/` files were cleared, to be rebuilt from better-curated references.

**Until it's rebuilt:** take all visual direction from the project's brief and the references the user supplies — do **not** invent a default aesthetic, and do not resurrect the old one. Everything else in this skill still applies as normal (quality bar, process, the motion doctrine, animation vocabulary, copy rules, UX correctness).

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
- **Setpiece palette — PORTABLE techniques only** (reach for one only when the context calls for it; the default is the calm alive layer, never a setpiece-by-default): kinetic / char-by-char typography, shared-element / morph transitions, scroll-reveal + stagger, a generic celebratory impact-confirmation for a genuinely big moment (anticipation → impact → settle). **A setpiece must fit the product's purpose and register** — a focus-timer hero doesn't need a save-stamp; a calm wind-down app doesn't need confetti or a twitchy hero.
- **Do NOT transplant quickboard's own signatures** (they live in the case study as examples, not defaults): cursor-interactive **3D tilt + spotlight**, materialize-from-a-point-of-light, the save-stamp, pop-from-row, the self-playing typing→stamp loop, zoom-through beat transitions. **Cursor-reactive 3D tilt is the one that keeps leaking — it is almost always wrong** on a landing page or a calm app (the hero twitches at the mouse and the mood breaks). For a floating product visual, use a *static, subtle* tilt or a straight floating card (what the references actually do), never a cursor-following one.
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
Flat default fills (use a shader) · pure-black dark mode (use charcoal) · neon/LED color · generic left-accent indicators, stock dropdowns, AI-purple glows, three-equal-cards (all read as AI slop) · square-everything (round it) · timid/half-committed motion · bare crossfades (always blur) · em dashes · emoji in UI · reskin-without-relayout · **cursor-reactive 3D tilt on a hero/landing/calm surface** (a quickboard transplant — use a static subtle tilt instead) · transplanting any quickboard signature setpiece onto a product it doesn't fit.

## Case study: quickboard (one expression — DON'T copy the specifics)
For a premium macOS desktop *clipboard utility*, the DNA expressed as a set of choices that are **specific to that product** — take the instincts, not these decisions:
- **Layout/IA:** "Soft Paper" pastel palette + ink `#1f2024`, baked ShaderGradient card surfaces, **items as list rows** (not cards), **"environments"** as workspaces, a Spotlight-style **summon** panel + floating **tray**, denser/smaller **desktop** fonts.
- **Motion signatures (do NOT transplant these):** the stamp-of-approval save, pop-from-row drag-out, **cursor-interactive 3D tilt + spotlight** on cards, materialize-from-a-point-of-light, the self-playing typing→stamp loop, zoom-through beat transitions. These fit a dense desktop utility you interact with directly; they are gimmicks on a marketing page or a calm app.

A marketing site or a mobile app gets bigger type, more whitespace, totally different IA, and *its own* fitting motion and visual styling — take the instincts, not quickboard's decisions.

---

**When in doubt:** make it feel *alive* (the calm micro-motion layer) and ask *"does this feel premium and magic?"* — and pull the **visual** styling from the project's references, since the visual layer here is being remade.
