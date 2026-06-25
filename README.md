# treshnanda-taste

A personal **UI/UX taste skill** for Claude Code (and other agents): a soft, premium, pastel, shader-textured, generously-rounded aesthetic paired with **bold, kinetic motion that's alive but never in the way**.

It's the *personal taste* layer that sits on top of two craft skills it **auto-loads** — [`emil-design-eng`](https://animations.dev) (craft details) and `motion-design` (motion theory). One invocation pulls the whole stack.

## Install

```bash
npx skills add Tresnanda/treshnanda-taste
```

Then start a **new** session and invoke it:

```
/treshnanda-taste
```

It automatically pulls in `emil-design-eng`, `motion-design`, the shared motion vocabulary, and the per-context visual references, then applies the personal taste lens on top.

## What's inside

- **`SKILL.md`** — the taste profile: quality bar + vocabulary, how I work, the **visual language** (canvas, color, the make-or-break shader/gradient rule, the image-header card, squircles, type), the **motion doctrine** (alive-not-disruptive, two registers, frequency-scaling), copy rules, UX-correctness, and a consolidated **"never" list**.
- **`reference/`** — per-context visual recipes, each with concrete specs (approximate hexes, radii, proportions) **and** its own premium-vs-slop guardrails, so the look is precise per surface instead of a blurry average:
  - `landing-pages.md` · `elements.md` · `desktop-app.md` · `mobile-app.md`
- **`animation-vocabulary.md`** — a shared glossary of animation patterns (e.g. *shared element transition, morph, rubber-banding, stagger, follow-through, squash & stretch*) so motion requests are unambiguous.

## Use it anywhere

Built to apply to **any app or website**, not one product. Distilled from hundreds of real build iterations plus a segmented library of reference designs (landing pages, elements, desktop apps, mobile).

---

*A living skill — it sharpens every time it's used on a real project.*
